---
title: Research
date: 2025-08-10
draft: false
---

Here's a list of things I've written for an academic audience.
Papers are listed chronologically, oldest to newest.

> "If you find any paper below hard to read, write to me [1], as that means the paper is poorly written, not that the result is hard."
-- Boris Bukh


***

[MPW+24] -- Cole Mathis, Devansh Patel, Westley Weimer, Stephanie Forrest,
**Self-organization in computation and chemistry: Return to AlChemy**,
2024,
[*Chaos* 34 *(9)*](https://pubs.aip.org/aip/cha/article-abstract/34/9/093142/3314760/Self-organization-in-computation-and-chemistry),
[pdf](https://arxiv.org/pdf/2408.12137),
[doi](https://doi.org/10.1063/5.0207358)

**TLDR**: Generate a giant set of expressions in the [lambda
calculus](https://en.wikipedia.org/wiki/Lambda_calculus) (a simple functional
programming language). Take two out. Compose and reduce (evaluate) them. Return
the composed expression and one parent back into the set. Repeat a bazillion
times. Do you observe anything interesting? Are there theoretical implications
for certain types of chemistries?

***

[Vim25] -- Devansh Vimal,
**Planarity of Mycielski-like graph expansions**,
2025,
*arXiv preprint*,
[pdf](https://arxiv.org/abs/2505.09534)

**TLDR (non-math):** OK, this one is really cool.
[Charlieplexing](https://en.wikipedia.org/wiki/Charlieplexing) is a neat little
method of reading inputs from a lot of switches using relatively few
microcontroller pins. Charlieplexed circuits can be transformed into 'power
saving' circuits by adding a few interrupt lines. The transformation of an
ordinary charlieplex circuit to the power-saving circuit might make the
power-saving circuit unroutable on a single-sided PCB (i.e. non-planar). Here,
I characterize all charlieplex circuits for which the power-saving circuits are
planar. Turns out that this is the set of all
[bipartite](https://en.wikipedia.org/wiki/Bipartite_graph)
[cactus](https://en.m.wikipedia.org/wiki/Cactus_graph) graphs.

I discovered this result after trying much too hard to save $1 off of a
PCB order by making my PCB single-sided. The PCB was for
[heartstopper](https://github.com/agentelement/heartstopper), a tiny mechanical
keyboard.

**TLDR (math):** Let G be a graph, and let S(G) be a transformation of this
graph such that for each vertex v of G, there is a vertex v' connected to v and
all neighbors of v. Then S(G) is planar if and only if G is a bipartite cactus.

The transformation S(G) is similar to Mycielski's operation. Structural
graph theory problems like this do not often have a clean characterization, so
this is a cute result.

***

[VMW+25] -- Devansh Vimal, Cole Mathis, Westley Weimer, Stephanie Forrest,
**Prebiotic Functional Programming: Endogenous Selection in an Artifical Chemistry**,
2025,
*[ALIFE](https://2025.alife.org) (to appear)*
[pdf](https://arxiv.org/abs/2509.03534)
[git](https://github.com/agentelement/functional-supercollider)

**TLDR**: A pseudo-follow-up to [MPW+24]. In [MPW+24], the lambda calculus
expressions act sort of like organisms, and composition sort of acts like a
crossover operator. Hey, that's all you need for evolution! Now let's play god:
can we add special organisms (carefully constructed combinators) into the
system such that we force the evolution of desirable lambda calculus
expressions?

(You can, but good results take up a lot of reductions.
Luckily, we wrote a very parallel lambda calculus reduction machine in rust.)

***

[VPS+25] -- Devansh Vimal, Garrett Parzych, Olivia M. Smith, Devendra Parkar and Sean Bergen, Joshua J. Daymude, Cole Mathis,
**Open, Reproducible Calculation of Assembly Indices**,
2025,
*arXiv preprint*,
[pdf](https://arxiv.org/abs/2507.08852),
[git](https://github.com/DaymudeLab/assembly-theory)

**TLDR**: There's a graph-theoretic measure of molecular complexity called the
assembly index of a molecule. It's controversial among people doing space
chemistry stuff. Worse still, it's #P-complete. Let's try to compute it really
fast anyway. And we'll make it open-source, because proprietary software = bad.

***
[1] in this case, "me" = me, not Boris
