---
title: "Derived Functors and Derived Categories"
date: 2023-05-26 12:00:00 -800
categories: [Derived]
tags: [Derived Categories, Derived Functors]
math: true
---

I've always quite liked learned about derived functors, although I wasn't really grasping the motivation when initially learning some basic things about $\operatorname{Ext}^i (-,-) $ and $\operatorname{Tor}^i (-,-)$, which are *derived* from the left exact functor $\operatorname{Hom} (-,-)$ and $-\otimes -$, respectively. This verb *derived* actually comes from thinking about derived categories, but to get at this perspective, it takes a lot of effort! I'm writing this note, <a href="https://notsatos.github.io/files/derived_fntrs_cats copy.pdf">Derived Functors and Derived Categories</a>, which I hope to motivate the things I've spoken about above (as I learn them), hopefully in a rewarding way.  

The first time I came to learning about $\operatorname{Ext}^i _A (-, M)$, I didn't really understand what we really meant once we consider some $A$-module $N$ and take a projective resolution, trucate the resolution, take (co)homology, and yadda yadda yadda; we get $\operatorname{Ext}^i _A(N,M)$. To understand $\operatorname{Ext}^i _A(N, M)$, we should actually look at why we call it "Ext": this comes from looking at so-called  *extensions*. To keep this simple, we consider $\operatorname{Ext}^1 _A(N,M)$. 

By an *extension of $B$ by $A$* for some $R$-modules $A$ and $B$, we mean a short exact sequence:

$$ 0 \to A \to D \to B \to 0$$

So, for example, $0 \to \mathbb Z \to \mathbb Q \to \mathbb Q/\mathbb Z \to 0$ is an extension (with the obvious maps) of $\mathbb Q / \mathbb Z$ by $\mathbb Z$. Now, the "Ext" functor essentially measures how many inequivalent extensions there are (whereby we define equivalence by isomorphisms of short exact sequence that are the identity). (For the details of this equivalence, see the linked document above.) We define $\mathfrak{ext} (B,A)$ as the set of extensions of $B$ by $A$ up to the equivalence described. To keep this short, there is an isomorphism between $\mathfrak{ext} (B,A) \cong \operatorname{Ext}_R ^1(B,A) $ (considered as groups, where the binary operation of $\mathfrak{ext} (B,A)$ is something called *Baer multiplication*), where the $\operatorname{Ext}_R^1 (B,A)$ corresponds to the derived functor perspective, which preserves the trivial element. Although these derived functors are defined quite abstractly, they represent an answer to a quite simple question! For example, as $\mathfrak{ext} (B,A) \cong \operatorname{Ext} _R ^1(B,A)$, then we can consider $\mathfrak{ext} (\mathbb Q / \mathbb Z,\mathbb Z) \cong \operatorname{Ext} _{\mathbb{Z}}^1(\mathbb Q / \mathbb Z,\mathbb Z)$. Missing a lot on the details here, we can show that $\mathbb Q / \mathbb Z$ is a divisble abelian group and thereby an injective object in $\mathsf{Ab}$, so $\mathbb Q / \mathbb Z$ is acyclic, so  $\mathfrak{ext} (\mathbb Q / \mathbb Z,\mathbb Z) \cong \operatorname{Ext} _{\mathbb{Z}} ^1(\mathbb Q / \mathbb Z,\mathbb Z) = (0)$. As this isomorphism carries the trivial extension, then there essentially only one way to fill in the sequence:

$$ 0 \to \mathbb Z  \to \ast \to \mathbb Q / \mathbb Z \to 0$$ 

to get an exact sequence (up to equivalence described)!

