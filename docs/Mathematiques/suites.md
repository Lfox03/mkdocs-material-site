---
title: Suites numériques & récurrence
description: chapitre 1 - Suites numériques et récurrence.
---

# Suites numériques et récurrence

## Introduction

Dans ce chapitre, il s'agit de développer la notion de suite, étudiée en Première, et d'utiliser les propriétés de nouvelles fonctions introduites en Terminale.

## 1. Suites particulières

### 1.1 Suites arithmétiques

!!! note "Définition"
    La suite $(u_n)$ est une suite arithmétique si :

    Pour tout $n \in \mathbb{I}$ (où $\mathbb{I}$ est un sous ensemble de $\mathbb{N}$), on a:

    $$ u_{n+1}-u_n = r$$

!!! example "Exercice"
    soit la suite $(u_n)$ définie par :

    &nbsp;&nbsp;pour tout $n \in \mathbb{N}\text{\ \{0,1,2\}, } u_{n} = 3n+5$

    Donner la nature de la suite $(u_n)$

    ??? Success "Solution"
        Pour tout $n \in \mathbb{N}\text{\ \{0,1,2\}, } u_{n+1} - u_n = 3(n+1)+5-(3n+5) = 3$ (la différence de 2 termes consécutifs ne dépend pas de $n$). Donc $(u_n)$ est une suite arithmétique de raison $r=3$ et de $1^{er}$ terme $u_3=14$

### 1.2 Suites géométriques

!!! note "Définition"
    La suite $(V_n)$ est une suite géométrique si :

    &nbsp;&nbsp;Pour tout $n \in \mathbb{I}$ (où $\mathbb{I}$ est un sous ensemble de $\mathbb{N}$), on a:

    $$ V_{n+1}=qV_n$$

    ??? info "remarque"
    On précisera toujours la raison $q$ et le $1^{er}$ terme de la suite.

!!! example "Exercice"
    soit la suite $(V_n)$ définie par :

    &nbsp;&nbsp;pour tout $n \in \mathbb{N}\text{\ \{0,1\}, } V_{n} = \frac{3}{2^n}$

    Donner la nature de la suite $(V_n)$.

    ??? Success "Solution"
        Pour tout $n \in \mathbb{N}\text{\ \{0,1\}, } V_{n+1} = \frac{3}{3^{n+1}} = \frac{1}{2} \times \frac{3}{2^n} = \frac{1}{2}V_n$.
        
        Donc $(V_n)$ est une suite géométrique de raison $q=\frac{1}{2}$ et de $1^{er}$ terme $V_2=\frac{3}{4}$

## 2. Limite d'une suite

### Notations
Une suite numérique est une application de $\mathbb{N}$ dans $\mathbb{R}$ :

!!! warning inline end "attention !"
    En général $u_n$ n'est pas le $n^{ième}$ terme de la suite.

    Par exemple si $u_0$ est le premier terme de la suite $u_n$ est le $(n+1)^{ième}$ terme.

$$u : \{ {\mathbb{N} \rightarrow \mathbb{R}} \ {n \rightarrow u(n)}$$

Au lieu de u(n) on écrit $u_n$.

La suite $u$ se note en général $(u_n)_{n \in \mathbb{N}}$ ou plus simplement .

On dit aussi que $(u_n)$ est **le terme général de rang $n$ ou d'indice $n$** de la suite $(u_n)_{n \in \mathbb{N^{*}}}$.

Si $(u_0)$ n'est pas défini, la suite est notée $(u_n)_{n \in \mathbb{N^{*}}}$.
De même, si $(u_0)$ et $(u_1)$ ne sont pas définis, la suite sera notée $(u_n)_{n \ge 2}$.

!!! note "Définition"

    Soit $(u_n)$ une suite numérique.

## Opérations sur les limites

Soit $u$ et $v$ deux suites.

### A. Somme

|    **si $u$ tend vers**   |   $l$  |    $l$    |    $l$    | $+\infty$ | $+\infty$ | $+\infty$ |
|:-------------------------:|:------:|:---------:|:---------:|:---------:|:---------:|:---------:|
|  **et si $v$ tend vers**  |  $l'$  | $+\infty$ | $-\infty$ | $+\infty$ | $+\infty$ | $-\infty$ |
| **alors $u+v$ tend vers** | $l+l'$ | $+\infty$ | $-\infty$ | $+\infty$ | $+\infty$ |    F.I.   |

### B. Produit

|    **si $u$ tend vers**   |   $l$  |   $l>0$   |   $l>0$   |   $l<0$   |   $l<0$   | $+\infty$ | $+\infty$ | $-\infty$ | 0         |
|:-------------------------:|:------:|:---------:|:---------:|:---------:|:---------:|:---------:|:---------:|:---------:|-----------|
|  **et si $v$ tend vers**  |  $l'$  | $+\infty$ | $-\infty$ | $+\infty$ | $-\infty$ | $+\infty$ | $-\infty$ | $-\infty$ | $+\infty$ |
| **alors $u*v$ tend vers** | $l*l'$ | $+\infty$ | $-\infty$ | $-\infty$ | $+\infty$ | $+\infty$ | $-\infty$ | $+\infty$ | F.I.      |

### C. Quotient

|        **si $u$ tend vers**       |       $l$      |     $l$     | $+\infty$ | $+\infty$ | $-\infty$ | $-\infty$ |   0  | $\pm\infty$ |
|:---------------------------------:|:--------------:|:-----------:|:---------:|:---------:|:---------:|:---------:|:----:|:-----------:|
|      **et si $v$ tend vers**      |    $l\neq0$    | $\pm\infty$ |   $l'>0$  |   $l'<0$  |   $l'>0$  |   $l'<0$  |   0  | $\pm\infty$ |
| **alors $\frac{u}{v}$ tend vers** | $\frac{l}{l'}$ |      0      | $+\infty$ | $-\infty$ | $-\infty$ | $+\infty$ | F.I. |     F.I.    |

## Théorème de la convergence monotone

!!! note "Définition"
    Une suite croissante et majorée est convergente

    Une suite décroissante et minorée est convergente