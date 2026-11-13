# 5/27/26

Reading over the paper after the rejection, listing everything I want to change here.
Also see the EC feedback for more TODO.

# Fundamental assumptions

### Potentially promising
- Markov chain with nonnegative drift implies submartingale implies
expected valuations increasing. Could assume one of these.
$$
V^z_{i} = \sum_{k=1}^i \xi_k^z, ~\mathbb{E}[\xi_k^z]\geq 0
\quad
\Rightarrow
\quad
\mathbb{E}[V^z_{i+1} | \mathcal{F}^z_i]\geq\mathbb{E}[V^z_{i}]
\quad
\Rightarrow
\quad
\mathbb{E}[V^z_{i+1}]\geq\mathbb{E}[V^z_{i}]
$$.

- Rule out dumb and pathological welfares by assuming
$W(x,y)$ is non-decreasing, and $x_1,y_1<x_2,y_2$ implies $W(x_1,y_1)<W(x_2,y_2)$.
Although this rules out $W(x,y)=1_{x,y\geq 0}(x+y)$.

- For the IC setting, could assume that $U^a(x,y)=V^a(x)-\alpha V^b(y)$.
We can throw lots of model assumptions at the IC setting.

# Major

- Define ex-interim IR and write a proposition showing it is equivalent to the IC definition. Maybe even just change IC to being called ex interim IR throughout?

- Revisit if there's a way to make the definitions cleaner and not deal with
the boundary explicitly.

# Writing

## Ideas

- Could add a figure to show examples of valuations trending upwards 
but not strictly increasing.

- Be more careful with welfare examples? E.g. for Nash should ensure always
positive.

## To edit

- Writing in second paragraph of 3.1 isn't great.

-  "An algorithm consists of a stopping
rule and an exchange recommendation rule." Make sure terminology of stopping
rules and algorithms is consistent.

- " We show that under a simple assumption for 𝑊 , that
a non-negative expected welfare implies non-negative expected utilities, the resulting optimal
algorithm is also individually rational."

- "are independent sequences drawn from priors 𝐷
𝑎
, 𝐷𝑏
, 𝑈
𝑎
,𝑈𝑏
,𝑊 : R
2 → R are"

## Nits

- $s_T$ looks weird.

- The prime notation is kinda clunky in Def. 2.3 and other places.

- Add "measurable" to Def. 2.2 for both sequences, its used in the equivalence proof.