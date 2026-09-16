---
layout: post
title: "Calabi–Yau Manifolds and Topological Strings"
date: 2026-09-17
---

String theory starts from a simple change of perspective: instead of taking point particles as the fundamental objects of the theory, one considers one-dimensional objects — strings. As a string propagates through spacetime, it sweeps out a two-dimensional surface, called its **worldsheet**.

Some of the most beautiful interactions between string theory and geometry arise when the space in which these strings propagate is a **Calabi–Yau manifold**. After a suitable modification of the underlying physical theory, known as a *topological twist*, one arrives at topological string theory and at two closely related theories: the **A-model** and the **B-model**.

What is particularly striking from a mathematical point of view is that these two theories isolate two different aspects of the geometry of a Calabi–Yau manifold. The A-model sees its symplectic geometry, while the B-model sees its complex geometry. The statement that these two apparently different theories can describe the same physics is one of the origins of **mirror symmetry**.

In this post I want to sketch this picture, starting from Calabi–Yau geometry and ending with the connection to symplectic topology.

## Calabi–Yau manifolds

There are several equivalent, or nearly equivalent depending on the hypotheses, ways of introducing Calabi–Yau manifolds. For our purposes, let \(X\) be a compact Kähler manifold of complex dimension \(n\) with trivial canonical bundle

\[
K_X = \Lambda^n T^{*1,0}X \cong \mathcal O_X.
\]

Equivalently, \(X\) admits a nowhere-vanishing holomorphic \(n\)-form

\[
\Omega \in H^0(X,K_X).
\]

In particular,

\[
c_1(X)=0.
\]

The Calabi conjecture, proved by Yau, then tells us that every Kähler class on \(X\) contains a unique Ricci-flat Kähler metric. Thus Calabi–Yau geometry naturally brings together complex, symplectic and Riemannian geometry.

The simplest compact example in complex dimension one is an elliptic curve. In complex dimension two, K3 surfaces provide a fundamental family of examples. In complex dimension three — the case that historically became especially important in string theory — perhaps the most famous example is the **quintic threefold**

\[
X=\{P(z_0,\ldots,z_4)=0\}\subset \mathbb{P}^4,
\]

where \(P\) is a homogeneous polynomial of degree \(5\) defining a smooth hypersurface.

Why is the quintic Calabi–Yau? The adjunction formula gives

\[
K_X
\cong
\left(K_{\mathbb P^4}\otimes\mathcal O_{\mathbb P^4}(5)\right)|_X.
\]

Since

\[
K_{\mathbb P^4}\cong\mathcal O_{\mathbb P^4}(-5),
\]

we obtain

\[
K_X\cong\mathcal O_X.
\]

So the degree \(5\) appearing in the definition of the quintic is not an accident: it precisely cancels the canonical bundle of \(\mathbb P^4\).

## Why do strings care about Calabi–Yau manifolds?

Suppose that the worldsheet of a string is a Riemann surface \(\Sigma\). A string propagating in a space \(X\) is described, at a very basic level, by a map

\[
\phi:\Sigma\longrightarrow X.
\]

One can construct a two-dimensional nonlinear sigma model whose fields include such maps. When the target \(X\) is Kähler, the sigma model can possess \(\mathcal N=(2,2)\) supersymmetry, which is the structure needed to perform the two topological twists leading to the A- and B-models.

The topological twist changes the interpretation of the theory in such a way that many of its observables cease to depend on the metric of the worldsheet. Instead, the resulting theory retains only certain geometric information about the target.

There are two possible twists:

\[
\text{A-model}
\qquad\text{and}\qquad
\text{B-model}.
\]

Their distinction is one of the key points of the story.

## The A-model

The A-model depends on the **symplectic geometry** of \(X\).

Let

\[
(X,\omega,J)
\]

be a Kähler manifold, with symplectic form \(\omega\) and compatible complex structure \(J\). After localization, the relevant maps in the A-model are \(J\)-holomorphic curves,

\[
\bar\partial_J\phi=0.
\]

Thus the path integral, which originally appears to involve an enormous space of maps \(\Sigma\to X\), localizes onto moduli spaces of pseudoholomorphic curves.

This is immediately familiar from symplectic geometry.

For closed strings, the worldsheet has no boundary. At genus zero the basic worldsheet is a sphere, so one encounters pseudoholomorphic maps

\[
u:S^2\longrightarrow X.
\]

Counting such curves, with appropriate marked points and constraints, leads to **Gromov–Witten invariants**.

At genus zero, these invariants deform the ordinary cup product on cohomology and give the quantum product

\[
*:QH^*(X)\otimes QH^*(X)\longrightarrow QH^*(X).
\]

Thus, in a rough but useful dictionary,

\[
\boxed{
\text{closed topological A-model}
\quad\longleftrightarrow\quad
\text{Gromov--Witten theory}.
}
\]

One important feature of the A-model is that it is insensitive to deformations of the complex structure. What matters instead is the symplectic, or more precisely complexified Kähler, data.

## The B-model

The B-model behaves very differently.

Rather than depending on the symplectic geometry of \(X\), it depends on its **complex structure**. Its observables are related to variations of complex structure, and the holomorphic volume form

\[
\Omega
\]

plays a central role.

For a Calabi–Yau threefold, one can study periods of the holomorphic three-form,

\[
\int_{\Gamma}\Omega,
\qquad
\Gamma\in H_3(X;\mathbb Z).
\]

As the complex structure varies, these periods vary as well and satisfy differential equations known as **Picard–Fuchs equations**.

The contrast with the A-model is therefore striking:

\[
\boxed{
\begin{array}{c|c}
\text{A-model} & \text{B-model}\\
\hline
\text{symplectic/Kähler geometry} & \text{complex geometry}\\
\text{holomorphic curve counts} & \text{periods and complex structures}\\
\text{Gromov--Witten invariants} & \text{variation of Hodge structure}
\end{array}
}
\]

At first sight these seem to be completely different theories.

Mirror symmetry says otherwise.

## Mirror symmetry

Very roughly, mirror symmetry predicts that Calabi–Yau manifolds come in pairs

\[
X \qquad\text{and}\qquad X^\vee
\]

such that the A-model on \(X\) is equivalent to the B-model on \(X^\vee\):

\[
A(X)\simeq B(X^\vee).
\]

Similarly,

\[
B(X)\simeq A(X^\vee).
\]

In particular, symplectic information about one Calabi–Yau manifold can be translated into complex-geometric information about its mirror.

This is already surprising at the level of deformation theory. Roughly speaking, Kähler deformations of \(X\) correspond to complex-structure deformations of \(X^\vee\), and vice versa.

But the correspondence becomes even more powerful when one tries to compute enumerative invariants.

A celebrated early example concerns rational curves on the quintic threefold. Directly computing the relevant curve counts on the A-model side is difficult. Mirror symmetry transforms the problem into a calculation involving periods on the mirror family, where the corresponding Picard–Fuchs equations can be studied explicitly.

This was one of the first dramatic indications that the physical idea of mirror symmetry contained genuinely new mathematical information.

## Opening the strings

So far we have only considered **closed strings**.

An open string has endpoints, and therefore its worldsheet has boundary. We must specify where this boundary is allowed to lie.

In the A-model, the relevant boundary conditions are given, in their simplest geometric form, by **Lagrangian submanifolds**

\[
L\subset X.
\]

Thus instead of closed holomorphic curves, we are led to maps

\[
u:(\Sigma,\partial\Sigma)
\longrightarrow
(X,L)
\]

satisfying

\[
\bar\partial_Ju=0.
\]

The simplest worldsheet is now a disc,

\[
u:(D^2,\partial D^2)\longrightarrow(X,L).
\]

The homotopy classes of such discs live in

\[
\pi_2(X,L),
\]

and their expected dimensions are governed by the Maslov index

\[
\mu:\pi_2(X,L)\longrightarrow\mathbb Z.
\]

We have therefore arrived naturally at one of the central objects of **Lagrangian Floer theory**: pseudoholomorphic discs with boundary on a Lagrangian.

This gives another part of the dictionary:

\[
\boxed{
\text{A-branes}
\quad\longleftrightarrow\quad
\text{Lagrangian geometry}.
}
\]

If we allow several Lagrangians \(L_0,L_1,\ldots\), then open strings can stretch between different branes. The states associated with strings stretching from \(L_0\) to \(L_1\) are reflected mathematically by the Floer complex

\[
CF^*(L_0,L_1).
\]

Holomorphic polygons with boundary on collections of Lagrangians then define higher operations

\[
\mu^k,
\]

which satisfy the \(A_\infty\)-relations.

Organizing all this information leads to the **Fukaya category**

\[
\mathcal F(X).
\]

So the categorical structure that appears in symplectic topology has a remarkably natural interpretation from the point of view of open strings: objects correspond to boundary conditions, morphisms correspond to open-string states, and the higher compositions encode their interactions.

## From mirror symmetry to homological mirror symmetry

The open-string picture suggests a much deeper version of mirror symmetry.

If A-branes are described by Lagrangian submanifolds and their Floer theory, what should the corresponding B-branes on the mirror be?

On the B-side, the relevant objects are closely related to coherent sheaves and complexes of coherent sheaves. This leads to Kontsevich's **homological mirror symmetry** conjecture, which predicts, in an appropriate setting, an equivalence

\[
D^\pi\mathcal F(X)
\simeq
D^b\operatorname{Coh}(X^\vee).
\]

The left-hand side belongs to symplectic topology. It is built from Lagrangian submanifolds and counts of pseudoholomorphic curves.

The right-hand side belongs to algebraic geometry. It is the derived category of coherent sheaves on the mirror.

What began as a duality between two physical theories therefore becomes a remarkable bridge between two apparently very different areas of mathematics.

## Where the strings went

There is something I find particularly appealing about this story.

If one first encounters Gromov–Witten invariants, Floer complexes or Fukaya categories purely from the mathematical side, the collection of objects involved can seem somewhat mysterious:

\[
J\text{-holomorphic spheres},\qquad
J\text{-holomorphic discs},\qquad
CF^*(L_0,L_1),\qquad
\mu^k,\qquad
\mathcal F(X).
\]
