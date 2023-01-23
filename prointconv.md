# Fonctions continues par morceaux

## Définition, exemples 


```{admonition} Définition 4
Une application $f$ de $[a, b]$ and $\mathbb{R}$ est dit continue par morceaux s'il existe une subdivision $u=(x_i)_{i=0}^n$ de $[a, b]$ telle que pour chaque $i \in \{1,\ldots, n\}$ la restriction de $f$ à $]x_{i-1}, x_i[$ soit continue et admette des limites finies en $x_{i-1}$ et $x_{i}$.

La subdivision $u$ est dite adaptée à la fonction $f$.
```

**Illustration avec un exemple graphique**:

```{image} fig1.png
:alt: fishy
:class: bg-primary mb-1
:width: 500px
:align: center
```


```{admonition} Exemples
- Toute fonction en escalier est continue par morceaux. 
- Toute fonction continue est continue par morceaux.
- La fonction $f$ définie sur $[-1, 1]$ par : 

$$f(0)=0 \mbox{  et  } \forall x \in [-1, 1] \setminus \{0\}, f(x)=\dfrac{1}{x}
$$

n'est pas continue par morceaux, car elle n'a pas de limite finie à droite et à gauche de $0$.

```

```{admonition} Remarques

Comme pour les fonctions en escalier, on peut vérifier que :
- si $u$ est une subdivision adaptée à une fonction $f$ continue par marceaux,
alors toute subdivision plus fine que $u$ est adaptée à $f$,
- si $f$ et $g$ sont deux fonctions continues par morceaux sur $[a, b]$ , alors il existe
Une subdivision adaptée à $f$ et $g$.
```


```{admonition} Proposition 6
Une fonction continue par morceaux sur  $[a, b]$ est bornée sur $[a, b]$ .
```


```{admonition} Démonstration
:class: dropdown


Soit $f$ une fonction continue par morceaux sur  $[a, b]$. Soit $u=(x_i)_{i=0}^n$ une subdivision adaptée à $f$.

Pour chaque $i \in \{1, \ldots, n\}$ admet des limites finies en $x_{i-1}$ et $x_i$. Donc la restriction de $f$ sur $]x_{i-1}, x_i[$ admet un prolongement par continuité sur $[x_{i-1}, x_i]$ qui donc borne. Par suite, $f$ est bornée sur $]x_{i-1}, x_i[$.

Ceci dit, 

$$
\forall i \in \{1, \ldots, n\}, \exists M_i \geq 0, \forall x \in ]x_{i-1}, x_i[, |f(x)| \leq M_i
$$

En prenant $M = \max_{i \in \{1, \ldots, n\}} M_i$, nous aurons $\forall x \in ]a, b[, |f(x)| \leq M$.

Par suite, $f$ est bornée sur $]a, b[$.


```



```{admonition} Proposition 7
Soient $f$ et $g$ deux fonctions continues par morceaux sur $[a,b]$. Les assertions suivantes sont correctes :

- $ \forall \lambda, \mu \in \mathbb R, \lambda f + \mu g$ est continue par morceaux.
- $fg$ est continue par morceaux.
```


```{admonition} Démonstration
:class: dropdown

Soit $u=(x_i)_{i=0}^n$ une subdivision adaptée à $f$ et $g$.

Les restrictions des fonctions $f$ et $g$ à chacun des intervalles $ ]x_{i-1}, x_i[$ sont continues et admettent des limites finies en  $x_{i-1}$ et $x_i$, donc il en est de même pour $\lambda f + \mu g$ et $fg$. Les fonctions
$\lambda f + \mu g$ et $fg$ sont donc continues par morceaux sur $[a, b]$.

```
## Intégrale d'une fonction continue par morceaux 

```{admonition} Théorème (admis)


Soit $f$ une fonction continue par morceaux sur le segment $[a, b]$ . Pour tout
réel $\epsilon > O$:

- il existe une fonction en escalier $\theta$ telle que $|f - \theta| \leq \epsilon$
- il existe des fonctions en escalier $\varphi$ et $\psi$ telles que :  

$$
\varphi \leq f \leq \psi \mbox{   et  } \psi - \varphi \leq \epsilon
$$
```

**Notations**: Dans ce qui suit, pour une fonction continue par morceaux $f$ nous allons adopte les notations suivantes :

- $\mathcal{E}^+(f)$ l'ensemble des fonctions en escalier plus grandes que $f$.
- $\mathcal{E}^-(f)$ l'ensemble des fonctions en escalier plus petites que $f$.

```{admonition} Proposition 8


Soit $f$ une fonction continue par morceaux sur le segment $[a, b]$. Alors :

- $\left\{\int_{[a, b]} \varphi | \varphi \in \mathcal{E}^-(f)\right\}$ admet une borne supérieure,
- $\left\{\int_{[a, b]} \psi | \psi \in \mathcal{E}^+(f)\right\}$ admet une borne inferieure,

de plus,

$$
sup\left\{\int_{[a, b]} \varphi | \varphi \in \mathcal{E}^-(f)\right\}= inf\left\{\int_{[a, b]} \psi | \psi \in \mathcal{E}^+(f)\right\}
$$
```

```{admonition} Démonstration
:class: dropdown

Soit $f$ une fonction continue par morceaux sur $[a, b]$. Donc $\left\{f(x)|x\in [a, b]\right\}$ est une partie non vide de $\mathbb R$ bornee donc admet une borne supérieure et une borne inferieure. Soit $m=\inf_{[a, b]}$ et $M=\sup_{[a, b]}$.

- Les deux fonctions constantes $m$ et $M$ sur $[a, b]$ sont aussi continues par morceaux sur $[a, b]$. $\left\{\int_{[a, b]} \varphi | \varphi \in \mathcal{E}^-(f)\right\}$ est donc une partie de $\mathbb R$ non vide majorée (par $M(b-a)$). Alors, elle possède une borne supérieure ($\alpha$). De même, $\left\{\int_{[a, b]} \psi | \psi \in \mathcal{E}^+(f)\right\}$ une partie de $\mathbb R$ non vide minorée donc possède une borne inferieure ($\beta$). 



- Toute fonction $\varphi \in \mathcal{E}^-(f)$ est inferieure à toute fonction $\psi \in \mathcal{E}^+(f)$. Par suite:


$$
\int_{[a, b]} \varphi \leq \int_{[a, b]} \psi
$$

Fixons $\varphi \in \mathcal{E}^+(f)$. L'ensemble $\left\{\int_{[a, b]} \psi | \psi \in \mathcal{E}^-(f)\right\}$ est majoreé par $\int_{[a, b]} \varphi$. Alors nous avons forcement $\alpha \leq \int_{[a, b]} \varphi$ et ça pour tout $\varphi \in \mathcal{E}^+(f)$. Donc $\alpha$ est un minorant de $\left\{\int_{[a, b]} \varphi | \varphi \in \mathcal{E}^-(f)\right\}$. Par consequent, $\alpha \leq \beta$.
-------------
----------

Donc 

$$
\alpha \leq \beta
$$


D'autre part, d'après le théorème



 

```
