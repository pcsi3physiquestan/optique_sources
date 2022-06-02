---
jupytext:
  encoding: '# -*- coding: utf-8 -*-'
  formats: ipynb,md:myst
  split_at_heading: true
  text_representation:
    extension: .md
    format_name: myst
    format_version: 0.13
    jupytext_version: 1.10.3
kernelspec:
  display_name: Python 3
  language: python
  name: python3
---

# Méthodes

## Utilisation des lois de Snell-Descartes
_La correction est en ligne._

````{admonition} Exercice 
:class: attention
:class: attention

```{figure} ./images/exo_casserole.png
:name: casserole
:align: center
:width: 40%
```

On considère une pièce de monnaie de rayon $R_0$ dont on négligera l'épaisseur posée au fond d'une casserole de hauteur $H_0$ remplie à ras bord d'eau.

L'oeil d'un observateur se trouve à la verticale de centre de la pièce à une hauteur $H_1$.

1. On appelle O le centre de la pièce. Déterminer l'équation que vérifie l'ouverture angulaire $\theta_0$ du faisceau issu du point O et qui entre dans l’oeil en fonction du rayon de la pupille $R_1$.

2. **Faire l'application numérique pour $H_0 = H_1$ en choisissant  des valeurs numériques plausibles. On sera amener à simplifier l'équation précédente AVANT de la résoudre en justifiant les simplification réalisée par des ordres de grandeurs.
````

````{topic} Correction
>__Mise en équation__
>
>Notons le point I, le point d'incidence sur le dioptre air-eau pour le rayon extrême du faisceau issu de O et entrant dans la pupille. On note $i_1$ et $i_2$ les angles respectivement d'incidence et de réfraction. On a les relations :
>
>\begin{align*}
	n_{eau} \sin i_1 &= n_{air} \sin i_2\\
	\frac{IL}{\tan i_2} &= H_1\\
	IL + IJ &= R_1\\
	\tan i_1 &= \frac{IJ}{H_0}
\end{align*}
>
>On a 4 inconnues (IL, IJ, $i_1$ et $i_2$) et quatre inconnues, on peut donc résoudre le système.
>
>Il est important de voir que la résolution complète ne nous intéresse pas. On veut $i_1$ qui représente l'ouverture angulaire. On va donc chercher à __garder ____$i_1$____ et éliminer les autres inconnues.__
>
>Les grandeurs $H_0, H_1, R_1$ et les indices sont des grandeurs connues qu'on va garder.
>
>_Equation pour l'angle:_
>Les deux dernières équations permettent d'écrire: $IJ = H_0 \tan i_1$ et $ IL = R_1 - H_0 \tan i_1$ d'où le système:
>
>\begin{align*}
	n_{eau} \sin i_1 &= n_{air} \sin i_2\\
	\frac{R_1}{\tan i_2} - H_0 \frac{\tan i_1}{\tan i_2}&= H_1
\end{align*}
>soit en éliminant $i_2$ (_on a directement utilisant $n_{air} = 1$ -  on peut se le permettre car l'indice de réfraction est sans dimension: le changer par sa valeur numérique n'impacte pas l'analyse dimensionnelle_):
>
>\begin{equation}
\left ( R_1 - H_0 \tan i_1 \right )\sqrt{1 - n_{eau}^2 \sin^2 i_1} = H_1 n_{eau} \sin i_1
\end{equation}
>
>On rappelle que $\theta_0 = i_1$
>
>__Résolution aux petits angles__
>
>Nous allons faire une approximation pour résoudre cette équation (sans quoi la résolution devient TRÈS délicate). En effet, la taille de la pupille est de l'ordre du mm (on prendra $R_1 = 1\rm{mm}$) et la hauteur de la casserole est de l'ordre de la dizaine de cm. (on prendre $R_0 = 5\rm{cm}$). Il vient que les angles à la normale seront nécessairement petit.
>
>On peut avoir un ordre de grandeur en considérant que $\theta_0 \sim \arctan\frac{R_0}{2H_0} \sim 10^{-2} \rm{rad}$. En pratique, la propagation n'est pas rectiligne mais les angles $i_1$ et $i_2$ sont nécessairement du même ordre de grandeur que $\theta_0$.
>
>Or si $\theta_0 << 1$, on __peut faire les approximations dites des petits angles :__
>
>\begin{align*}
	\sin i &\approx i\\
	\tan i &\approx i\\
	\cos i &\approx 1\\
\end{align*}
>
>On ne conservera pas aussi les puissances au carré des petits angles (on parle d'approximation à l'ordre 1), des précisions seront données sur cette approximation dans des cours ultérieurs. On essaiera déjà d'appréhender la méthode d'utilisation de cette approximation.
>
>Ici l'équation devient :
>
>\begin{equation}
\left ( R_1 - H_0 i_1 \right ) = H_1 n_{eau} i_1 \Longrightarrow \theta_0 = i_1 \approx \frac{R_1}{H_0 + H_1} = 10^{-2}  \rm{rad}
\end{equation}
````
