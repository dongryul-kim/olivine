+++
title = "Mathematics"
taxonomies.tags = ["olivine", "adic-spaces"]
+++

This is a demo for writing mathematics on Olivine.
[MathJax](https://www.mathjax.org/) can be enabled by setting the option
`extra.olivine.mathjax = true` and diagrams can be enable by setting
`extra.olivine.tikzjax = true`. The version of TikZJax that we use comes from
[benrbray/tikzjax](https://github.com/benrbray/tikzjax). The mathematics itself
is based on [Ian Gleason](https://ianandreigf.github.io/Website/)'s thesis.

## The olivine spectrum

A point in the adic spectrum is by definition a multiplicative valuation on the
ring. A point in the olivine spectrum is supposed to be a pair of two
valuations $(v^h, v^a)$ where
- $v^a$ is rank-$1$,
- $v^a$ is a vertical generalization of $v^h$.

<div class="olivine-admonish">

**Warning.** A trivial valuation is also regarded as a rank-$1$ valuation.

</div>

By definition, there is a continuous map $$ \operatorname{Spo}(R, R^+) \to
\operatorname{Spa}(R, R^+); \quad (v^h, v^a) \mapsto v^h. $$

<div class="olivine-admonish">

**Theorem.** Let $(R, R^+)$ be a complete Huber pair over $\mathbb{Z}_ p$. Then
there exists a canonical continuous bijection $\lvert \operatorname{Spd}(R, R^+)
\rvert \to \operatorname{Spo}(R, R^+)$. This map is a homeomorphism when either
(i) $R$ is a Tate ring, or (ii) $R = R^+$ is an adic ring.

</div>

Such Huber pairs $(R, R^+)$ for which this map is a homeomorphism is called an
*olivine Huber pair*.

## The reduction functor

<div class="olivine-admonish">

**Definition.** We say that a morphism $S \to T$ of (perfect) affine schemes is
a *v-cover* when for every valuation ring $V$ and a map $\operatorname{Spec} V
\to T$ there is an extension $V \subseteq W$ of valuation rings and a
commutative diagram
<script type="text/tikz">
\usepackage{amsmath} \usepackage{tikz-cd} \begin{document} \Large \begin{tikzcd}
\operatorname{Spec} W \arrow{r} \arrow{d} & S \arrow[two heads]{d} \\
\operatorname{Spec} V \arrow{r} & T.
\end{tikzcd} \end{document}
</script>
</div>


<div class="olivine-admonish">

**Fact.** A map $S \to T$ of perfect affine schemes is a v-cover if and only if
the induced map $S^\diamond \to T^\diamond$ is v-surjective. Here, we are using
the definition that $(\operatorname{Spec} A)^\diamond = \operatorname{Spd}(A,
A)$.
</div>

This allows us to define for each v-sheaf $\mathscr{F}$ (on perfectoid spaces)
its reduction
$$ \mathscr{F}^\mathrm{red}(A) = \Hom(\operatorname{Spd}(A, A), \mathscr{F}) $$
as a sheaf on perfect schemes with the v-topology.

