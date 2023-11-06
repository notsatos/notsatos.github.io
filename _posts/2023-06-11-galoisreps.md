---
title: "Galois Representations"
date: 2023-06-11 12:00:00 -800
categories: [p-adic Hodge Theory]
tags: [Galois Representations, p-adic Hodge Theory]
math: true
---
This is meant as a tiny note to recollect some ideas I've been reading about when it comes to Galois representations. That is, representations of the absolute Galois group $G_{\mathbf Q} = \text{Gal} (\overline{\mathbf Q} /\mathbf Q)$. 

Firstly, $G_{\mathbf Q}$ can be thought of as a limit. We can consider the system of finite Galois extensions $\text{Gal} (K/\mathbf Q)$ and then make this into a suitable system by declaring that $K \leq L$ if and only if $K$ is a subfield of $L$, where maps $\text{Gal} (K/\mathbf Q) \to \text{Gal} (L/\mathbf Q)$ is just given be restriction. Thus, 


$$ \varprojlim _K \text{Gal} (K/\mathbf Q) = \{{  (\sigma_K) \in \prod_{K}  \text{Gal} (K/\mathbf Q) \colon \sigma_L|_K = \sigma _K \, \text{for all $K \subset L$} \}}$$ 

