# Somme de Riemann


```{admonition} Définition 
Soient $u=(x_i)_{i=0}^n$ une subdivision de $[a, b]$ et $v=(y_i)_{i=1}^n$ une famille de points de $[a, b]$ telle que :

$$
\forall i \in \{1, \ldots, n\}, y_i \in [x_{i-1}, x_i]
$$

Si $f$ est une fonction continue par morceaux sur $[a, b]$, on appelle **somme de Riemann** de $f$ associée a la subdivision $u$ et a la suite $v$, la quantité:

$$
\sigma(f, u, v)= \sum_{i=1}^n(x_i-x_{i-1})f(y_i)
$$

```
Pour le cas d'une fonction en escalier (qui est une fonction continue par morceaux), la somme de Riemann $\sigma(f, u, v)$ est égale a son intégrales.



Les cas les plus utilises sont ceux ou la subdivision $u=(x_i)_{i=0}^n$ est pas constant, c'est-à-dire lorsque $x_i = a+i\dfrac{b-a}{n}$



- Considérons une subdivision régulière $u=(x_i)_{i=0}^n$  $v=(y_i)_{i=1}^n$ une famille de points de $[a, b]$ telle que :

$$
\begin{cases}
x_i = a + i\dfrac{b-a}{n},  ~~ 0\leq i \leq n \\
y_i = x_{i-1} , ~~ 1\leq i \leq n \\
\end{cases}
$$

La somme de Riemann correspondante s’écrit :

$$
\sigma(f, u, v) = \dfrac{b-a}{n}\sum_{i=0}^{n-1} f(a+i\dfrac{b-a}{n})
$$


```{image} sumreimaninf.PNG
:alt: fishy
:class: bg-primary mb-1
:width: 400px
:align: center
```

- Considérons une subdivision régulière $u=(x_i)_{i=0}^n$  $v=(y_i)_{i=1}^n$ une famille de points de $[a, b]$ telle que :

$$
\begin{cases}
x_i = a + i\dfrac{b-a}{n},  ~~ 0\leq i \leq n \\
y_i = x_{i} , ~~ 1\leq i \leq n \\
\end{cases}
$$

La somme de Riemann correspondante s’écrit :

$$
\sigma(f, u, v) = \dfrac{b-a}{n}\sum_{i=1}^n f(a+i\dfrac{b-a}{n})
$$


```{image} sumreimansup.PNG
:alt: fishyy
:class: bg-primary mb-1
:width: 400px
:align: center
```



```{admonition} Proposition (résultat admis)

Soit $f$ une application continue sur $[a, b]$,

Pour tout $\epsilon > 0$, il existe $\eta > 0$ tel que pour toute subdivision $u=(x_i)_{i=0}^n$ et pour toute famille $v=(y_i)_{i=1}^n$ qvec $y_i \in [x_{i-1}, x_i]$ pour tout $i \in \{1,\ldots,n\}$ on a:

$$
\delta(u)\leq \eta \Rightarrow \left|\int_{[a, b]} f - \sigma(f, u, v)\right| \leq \epsilon
$$

```


```{admonition} Proposition

Soit $f$ une application continue sur $[a, b]$,

Pour tout $\epsilon>0$, il existe $\eta>0$ tel que pour toute subdivision $u=(x_i)_{i=0}^n$ et pour toute famille $v=(y_i)_{i=1}^n$ avec $y_i \in [x_{i-1}, x_i]$ pour tout $i \in \{1,\ldots,n\}$ on a:

$$
\delta(u)\leq \eta \Rightarrow \left|\int_{[a, b]} f - \sigma(f, u, v)\right| \leq \epsilon
$$

```
Les sommes de Riemann sont aussi proches que l'on veut de son intégrale quand le module de la subdivision tend vers 0.
