.PHONY: all
all:
	@set -eu; build_dir=$$(mktemp -d /tmp/ic-existence-build.XXXXXX); \
	trap 'rm -rf "$$build_dir"' EXIT; \
	pdflatex -interaction=nonstopmode -halt-on-error -output-directory="$$build_dir" existence.tex >"$$build_dir/compile.stdout" 2>&1 || { cat "$$build_dir/compile.stdout"; exit 1; }; \
	pdflatex -interaction=nonstopmode -halt-on-error -output-directory="$$build_dir" existence.tex >"$$build_dir/compile.stdout" 2>&1 || { cat "$$build_dir/compile.stdout"; exit 1; }; \
	if grep -E '(^!|LaTeX Warning:|Overfull)' "$$build_dir/existence.log"; then exit 1; fi; \
	cp "$$build_dir/existence.pdf" existence.pdf
