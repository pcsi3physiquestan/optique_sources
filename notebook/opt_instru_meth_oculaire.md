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

# Etude d'un oculaire

Un oculaire est dispositif permettant de donner d'un objet proche une image grossie. Dans son utilisation optimale pour un oeil emmétrope, cette image doit être à l'infini. La version la plus simple d'un oculaire est donc la loupe. Nous allons ici étudier un oculaire plus complexe composé de deux lentilles.

Utiliser deux lentilles permet en général de mieux traiter les aberrations et d'augmenter le champ de l'oculaire.

On considère donc un doublet de lentille \{$L_1,L_2$\} appelé doublet de Ramsden dont les distances focales images respectives sont $f_1 = f_2 = 3a$ et dont la distance entre les centre optiques respectifs $O_1$ et $O_2$ est $\overline{O_1 O_2} = a$.


````{admonition} Exercice 
:class: attention
1. Déterminer graphiquement puis par le calcul la position du foyer principal objet de l'ensemble des deux lentilles. Pourquoi est-ce important de savoir où il se trouve ? Commenter son caractère virtuel ou réel.
2. Déterminer le grossissement commercial de l'oculaire. Quelle focale faudrait-il à une loupe pour avoir le même grossissement commercial ?
````

````{important} 
:class: dropdown
__Bilan à retenir - Ce n'est PAS la correction.__  
On retiendra que:
* pour des systèmes devant grossir des objets à distance finies (oculaire, loupe, microscope... ), on va chercher -  dans le cas d'oeil emmétrope - à placer l'objet sur le foyer principal objet de l'ensemble.
* La mesure du grossissement (commercial) passe en général par l'utilisation de l'image intermédiaire.
````

````{topic} Modélisation simplifiée
Les oculaires sont rarement utilisées seules (sauf en joaillerie). En général, elle sont mise après une lentille d'objectif dans un appareil plus complexe comme une lunette ou un microscope.

Par la suite, on va étudier une lunette ou un microscope. En général, l'oculaire est composée de plusieurs lentilles mais on peut "faire comme si" elle se ramenait à une lentille (loupe) dont le grossissement est équivalent - on donne en général la focale correspondante. Celà simplifie l'étude sans changer les résultats. Il ne faut donc pas être étonné de voir des oculaires à une lentille par la suite.
````

