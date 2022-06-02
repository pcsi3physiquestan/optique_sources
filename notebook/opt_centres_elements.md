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

# Eléments principaux des systèmes centrés

## Eléments principaux: foyers

```{margin}
* La définition avec les rayons est utiles pour les graphiques
* La définition en terme de conjugaison est utile pour les mise en équation
```
````{important} __Foyers principaux objets et images__
* On définit le __foyer principal objet__ comme le point où tout rayon _incident_ passant par le foyer principal objet ressort du système optique (__rayon transmis__) en étant parallèle à l'axe optique.

__Le foyer principal objet est donc l'antécédent du point à l'infini sur l'axe optique.__

* On définit le foyer principal image comme le point tel que tout rayon __incident__ parallèle à l'axe optique ressort du système optique (__rayon transmis)__ en passant par le foyer principal image.

__Le foyer principal image est donc l'image du point à l'infini sur l'axe optique.__

```{figure} ./images/optique_foyer_quelconque.jpg
:name: foyer_principal_image_objet
:align: center
Foyer principal image (gauche) et objet (droite)
```

* Les plans focaux objet et image sont respectivement les plans frontaux contenant les foyers principaux objet ou image.
````

```{sidebar} Objet et image à l'infini
* Il est fondamental de savoir reconnaître et représenter un objet ou une image à l'infin : ils ne sont pas représentés par des points mais par des faisceaux parallèles dont _l'angle par rapport à l'axe optique défini la position de l'objet/image à l'infini. On parle __d'angle sous lequel et vu l'objet__.
```
````{important} __Foyers secondaires objets et images__
Les foyers _secondaires_ objet et image sont les points respectivement du plan focal objet ou image n'étant pas sur l'axe optique.

* Un foyer secondaire objet a pour image un point à l'infini __hors de l'axe optique__ (qu'on peut représenter par un faisceau sortant parallèle entre eux mais non parallèle à l'axe optique). _Une telle image est caractérisée par l'angle du faisceau ainsi formé_.

* Un foyer secondaire image a pour antécédent un point à l'infini __hors de l'axe optique__ (qu'on peut représenter par un faisceau entrant parallèle entre eux mais non parallèle à l'axe optique). _Un tel objet est caractérisé par l'angle du faisceau ainsi formé_.
````

## Eléments principaux: Centre optique et distance focale

```{margin} Remarque : Existence du centre optique
Pour un système optique quelconque, le centre optique n'existe pas forcément. Par exemple pour un système à plusieurs lentilles (lunette astronomique... ), il n'y a pas de centre optique du système complet.
```
````{important} __Centre optique__
Le __centre optique__ est le point de l'axe optique où tout rayon incident pointant vers ce point ressort sans être dévié.
````

```{margin}
Attention aux appelations et aux notations. Il arrive qu'on trouve la notation f pour la distance focale image.

De plus, on parle souvent - par abus de langage - de distance focale pour désigner implicitement la distance focale image.
```
````{important} __Distance focale objet et image__
* Lorsque le centre optique existe, on définit la distance focale objet f comme la distance __algébrique__ entre le centre optique O et le foyer principal objet F: $f = \overline{OF}$
* Lorsque le centre optique existe, on définit la distance focale image f' comme la distance __algébrique__ entre le centre optique O et le foyer principal image F': $f' = \overline{OF'}$
* On définit la vergence $V = 1 / f'$ avec $f'$ la distance focale image. Son unité est la __dioptrie__ notée $\delta$
````
