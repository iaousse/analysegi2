# Exercices

## Exercice 1

Soient $m, n \in \mathbb Z$, et $f$ une application telle que :

$$
\begin{array}{ccccc}
f & : & [m, n] & \to & \mathbb R \\
 & & x & \mapsto & \lfloor x \rfloor\\
\end{array}
$$

1. Vérifier que $f$ est une fonction en escalier et donner deux subdivisions adaptées à $f$.
2. Calculer 

$$
\int_{[m, n]} f
$$


## Exercice 2

Soit $f$ la fonction définie sur $[0, 4]$ par

$$
f(x) =
\begin{cases}
-1& \mbox{ si } x=0 \\ \\ 
1 & \mbox{ si } 0<x<1 \\
3 & \mbox{ si } x=1 \\
-2&  \mbox{ si } 1< x \leq 2 \\
4 & \mbox{ si } 2< x \leq 4
\end{cases}
$$

1. Vérifier que $f$ est une fonction en escalier.
2. Donner deux subdivisions adaptées à $f$ (notées $\sigma$ et $\sigma'$).
3.  Calculer $I(\sigma, f)$ et $I(\sigma', f)$.

## Exercice 3

Soit $f:[a,b]\to\mathbb{R}$ une fonction en escalier. On définit la fonction $h:[a,b]\to\mathbb{R}$ associée à $f$ par :

$$
h(x) = \begin{cases} f(x) & \text{si } x\in[a,c[\\ f(c) & \text{si } x\in[c,b] \end{cases}
$$

où $c\in[a,b]$ est une constante.

1. Montrez que $h$ est une fonction en escalier.
2. Proposer une subdivision adaptée à $h$.
3. Montrez que si $f$ est continue en $c$, alors $h$ est continue en $c$.


## Exercice 4
Soit $f$ une fonction en escalier sur $[a,b]$. Montrer que si $f$ est continue sur $[a, b]$ alors $f$ est constante sur $[a, b]$.

## Exercice 5
Soit $f$ une fonction en escalier sur $[a, b]$ et $\sigma_1$, $\sigma_2$ deux subdivisions adaptées à $f$. Montrer que $\sigma_1\cap \sigma_2$ est une subdivision adaptée à $f$.


## Exercice 6
Soit $f$ la fonction définie sur $[0, 2]$ par $f(x) = \cos(\frac{\pi}{2}[x^2]), \forall x \in [0, 2]$. Montrer que $f$ est une fonction en escalier sur $[0,2]$ et calculer son intégrale.
