---
title: "The  p-Adic Local Langlands Correspondence for GL_2 (Q_p)"
date: 2023-04-22 12:00:00 -800
categories: [Langlands]
tags: [Galois representations, Langlands, Translation]
math: true
---

As a short preface, this is an attempted translation of the paper written by Laurent Berger for the Bourbaki Seminar, N. 1017, which lays out, quite clearly, the $p$-adic local Langlands correspondence for $\operatorname{GL}_2 (\mathbf Q_p)$. The original version is in French and is posted here: <a href="https://arxiv.org/abs/1002.4111">arXiv:1002.4111 </a>


____

# The p-Adic Local Langlands Correspondence for $\operatorname{GL}_2 (\mathbf Q_p)$

Abstract. The $p$-adic local Langlands correspondence for $\operatorname{GL}_2 (\mathbf Q_p)$ is a bijection between some $2$-dimensional representations of $\operatorname{Gal}(\overline{ \mathbf Q_p}, \mathbf Q_p)$ and some representations of $\operatorname{GL}_2 (\mathbf Q_p)$. This bijection can in fact be constructed using the theory of $(\varphi, \Gamma)$-modules and some results of $p$-adic analysis. One then deduces from the properties of this construction some interesting arithmetical applications.


## Introduction. 

The $p$-adic local Langlands correspondence for $\operatorname{GL}_2 (\mathbf Q_p)$ is a bijection between some $2$-dimensional representations of $\operatorname{Gal}(\overline{ \mathbf Q_p}, \mathbf Q_p)$ and some representations of $\operatorname{GL}_2 (\mathbf Q_p)$. These representations are with coefficients either in a finite extension of $\mathbf F_p$ (correspondence in characteristic $p$), or in a finite extension of $\mathbf Q_p$(correspondence $p$-adic).

In the case of the correspondence in characteristic $p$, we can make a list of objects on the side of $\operatorname{Gal}(\overline{ \mathbf Q_p}, \mathbf Q_p)$ as well as on the side of $\operatorname{GL}_2 (\mathbf Q_p)$ and this makes it possible to define a numerical bijection whose construction is given in $\S 1$. In the case of the $p$-adic correspondence, we start by explaining how to sort through the representations of $\operatorname{Gal}(\overline{ \mathbf Q_p}, \mathbf Q_p)$ (Fontaine's theory) and in those of $\operatorname{GL}_2 (\mathbf Q_p)$ (representations "admissibles" in the sense of Schneider and Teitelbaum). In following, we give the first examples of the correspondence constructed by Breuil, which is the objective of $\S 2$. It's by studying these examples that Colmez understood how to construct this correspondence in a functorial way, thanks to the theory of $(\varphi, \Gamma)$-modules. This construction is given in $\S3$ for the "triangular" representations. Section $\S 4$ contains the general construction, as well as some properties of the correspondence.

1. the compatibility with the reduction modulo $p$,

2. link with the correspondence of the "classical" local Langlands.

In section $\S5$, we give some applications of the correspondence, including

1. the calculation of the reduction modulo $p$ of the crystalline representations,

2. the proof of (numerous cases of) the conjecture of Fontaine-Mazur.

This text does not say much about the motivation of these constructions. Apart from the compatibility with the classical local Langlands correspondence, a very important property of the p-adic correspondence is its realization in the complete cohomology of the towers of modular curves (work in progress). Finally, the extension of these constructions to groups other than $\operatorname{GL}_2(\mathbf Q_p)$ is particularly delicate and is the subject of numerous works in progress, of which it would be premature to speak of (see [Bre10]).

### **Notations** 
Throughout this text, $E$ designates a finite extension of $\mathbf Q_p$ for which we write $\mathcal O_E$ for its ring of integers, $\mathfrak m_E$ the maximal ideal of $\mathcal O_E$ and $k_E$ its residue field. The fields $E$ and $k_E$ are the fields of coefficients of representations that we consider.  

Class field theory provides an application $\mathbf Q_p^\times \to \operatorname{Gal}(\overline{\mathbf Q_p}, \mathbf Q_p)^{\operatorname{ab}}$ whose image is dense and that we normalize by deciding that the image of $p$ is the geometric frobenius. This application premits us to consider the characters of $\mathbf Q_p^\times$ with values in $E^\times$ or $k_E^\times$ as characters of $\operatorname{Gal}(\overline{\mathbf Q_p}, \mathbf Q_p)^{\operatorname{ab}}$. We denote $\mu_\lambda$ the character of $\mathbf Q_p^\times$ which is unramified (that is trivial on $\mathbf Z_p^\times$) and which sebd $p$ to $\lambda$ and we note $|\cdot |$ the character $x \mapsto x^{-\operatorname{val}_p(x)}$ where $\operatorname{val}_p(p)=1$.

## 1. Representations in characteristic $p$