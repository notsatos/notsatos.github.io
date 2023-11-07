---
title: "Galois Representations"
date: 2023-06-11 12:00:00 -800
categories: [p-adic Hodge Theory]
tags: [Galois Representations, p-adic Hodge Theory]
math: true
---
This is meant as a tiny note to recollect some ideas I've been reading about when it comes to Galois representations. That is, representations of the absolute Galois group $G_{\mathbf Q} = \text{Gal} (\overline{\mathbf Q} /\mathbf Q)$. 

Firstly, $G_{\mathbf Q}$ can be thought of as a limit. We can consider the system of finite Galois extensions $\text{Gal} (K/\mathbf Q)$ and then make this into a suitable system by declaring that $K \leq L$ if and only if $K$ is a subfield of $L$, where maps $\text{Gal} (K/\mathbf Q) \to \text{Gal} (L/\mathbf Q)$ are just given be restriction. Thus, 


$$ \varprojlim _K \text{Gal} (K/\mathbf Q) =   (\sigma_K) \in \prod_{K}  \text{Gal} (K/\mathbf Q) \colon \sigma_L|_K = \sigma _K \, \text{for all $K \subset L$} $$ 


Furthermore, we have $G_{\mathbf Q} \cong \varprojlim_{K} \text{Gal} (K/\mathbf Q)$ by the mapping $\theta \colon \sigma \mapsto \sigma | _K $. As we can equip each $\text{Gal}(K/\mathbf Q)$ is the discrete topology, then $G_{\mathbf Q}$ becomes a profinite group. From this general fact, we come to the conclusion that $G_{\mathbf Q}$ is compact and a totally disconnected topological group.

Recall that a topological group is a group $G$ which has multiplication and inversion, i.e. $m \colon (a,b) \mapsto a\cdot b$ and $i \colon a \mapsto a^{-1}$,  continuous maps with respsect to the endowed of $G$. Also note here that in topological groups being open subgroup implies being a closed subgroup but not the other way around necessarily. 

The profinite topology on $G_{\mathbf Q}$ amounts to declaring that the open subgroups of it are prcisely $\text{Gal} (\overline {\mathbf Q}/L)$ where $L $ is a finite extension of $\mathbf Q$. (Moreover, all the closed subgroups, which are not also open, are of the form $\text{Gal} (\overline{\mathbf Q}/K)$ for $K/\mathbf Q$ an infinite extension.)


This is a topological group because for the inversion map $i \colon G_{\mathbf Q} \to G_{\mathbf Q}$, given a open subset $U_L = \text{Gal}(\mathbf Q/L) \subset  G_{\mathbf Q}$, we have that $i^{-1} (U_L) = U_L$, and the multplicative map follows simiarly. The arguments don't really hinge on $G_{\mathbf Q}$, but instead just taking a Galois extension $L /K$ and defining the topology on $\text{Gal} (L/K)$ as we did for $G_{\mathbf Q}$.

We have the following analog of the fundamental theorem of Galois theory:



## Definition of (topological) Galois Representation 
For Galois representations, we want to consider only continuous maps $G_{\mathbf Q} \to \text{GL}_n (k)$ for $k$ a topological field, i.e. a field endowed with a topology which has addition, multiplication, and inversion as continuous map. The group $\text{GL}_n (k)$ will inherit the topology from being a subset of $k^{n^2}$. 

*Definition* A *Galois representation* of dimension $n$ over a (topological) field $k$ is a continuous group homomorphism 

$$\pi \colon G_{\mathbf Q} \to \text{GL}_n (k).$$

If $k$ is an extension of $\mathbf Q_\ell$, we call $\pi$ an *$\ell$-adic Galois representation*.

Some dub this the most important Galois representation, called the *$\ell$-adic cycltomic character*, which goes as follows. Let $\omega_n = \{{ \omega \in \overline{\mathbf Q}^\times \colon \omega^n = 1\}}$. We have an isomorphism of $\text{Gal} (\mathbf Q(\omega_n)/\mathbf Q) \cong (\mathbf Z/n \mathbf Z)^\times$ given by $\theta  \colon \sigma \mapsto a$ whereby $\sigma(\zeta) =\zeta^a$ for any $\zeta \in \omega_n$. Let $\ell$ be prime. We can write $\omega_{\ell^{\infty}} = \bigcup_{ n \geq 1} \omega_{\ell^n}$, and we have $ \text{Gal} (\mathbf Q(\omega_{\ell^\infty})/\mathbf Q) \cong \varprojlim_{n \geq 1} \text{Gal} (\mathbf Q(\omega_{\ell^n})/\mathbf Q)$. We we also have compatability so that $\text{Gal} (\mathbf Q(\omega_{\ell^n})/\mathbf Q) \cong \varprojlim_{n \geq 1} (\mathbf Z/\ell^n \mathbf Z)^\times \cong \mathbf Z_\ell^\times$. The composition $$\chi \colon \mathbf G_\mathbf \to \text{Gal} (\mathbf Q(\omega_{\ell^\infty})/\mathbf Q) \to \mathbf Z_\ell^\times \to \mathbf Q_\ell ^\times = \text{GL}_1(\mathbf Q_\ell)$$ is our $\ell$-adic character.