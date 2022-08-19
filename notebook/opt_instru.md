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
# Instruments d'optique

````{admonition} Compétences
* Modéliser à l'aide de plusieurs lentilles un dispositif optique d'utilisation courante.
* Connaître les positions relatives des éléments d'un système afocal à deux lentilles.
* Savoir calculer des éléments caractéristiques (grossissement, grossissement commercial, profondeur de champ) pour un instrument d'optique donné (leur définition étant donnée).
````

_Ce chapitre étant un chapitre d'application, la mise en contexte ci-dessous est relativement courte. On y trouvera princpalement des exercices._

````{topic} Intérêt d'un instrument d'optique
Un instrument d'optique peut avoir plusieurs buts suivant les raisons de son utilisation. On distingue les instruments d'optique devant être utilisés par l'oeil (loupe, lunette... ) et les instruments d'optique servant à projeter l'image (en vue d'un enregistrement: l'appareil photographique).

Nous allons surtout développer l'étude des premiers (un devoir libre traite de l'appareil photographique). Ces instruments ont en général pour but de permettre l'observation d'objets dans les meilleures conditions c'est-à-dire:

* l'image (finale) donnée par l'instrument sera placée au Punctum Remotum de l'oeil de l'utilisateur. Cette image sert d'objet pour l'oeil.
* l'image (finale) est en générale "grossie", c'est-à-dire que __l'angle sous laquelle on la voit avec l'instrument sera plus grand que l'angle sous lequel on la voyait à l'oeil nu.__
````

````{sidebar} Cas de l'utilisation par un oeil myope
En général, les instruments sont analysés par le constructeur dans le cadre canonique précédent (on parle de caractéristiques "commerciales"). Mais une bonne partie des instruments proposent un réglage (l'oculaire - cf. suite) permettant d'adapter l'appareil à un utilisateur myope.
````
````{topic} Cas d'étude canonique
L'étude canonique consiste à analyser les caractéristiques d'un instrument dans le cadre d'une utilisation par un __oeil emmétrope.__

__Conséquence:__ On cherchera à placer l'image finale __à l'infini.__. On étudiera très souvent les caractéristiques de l'instrument dans ce cadre.
````

## Types de systèmes

```{important} 
__Système afocal__

Un système __afocal__ est un système donnant d'un objet à l'infini une image finale à l'infini.
```
````{sidebar} Autres systèmes
Il existe d'autres systèmes visant des objets à distance finie: loupe, microscope, viseurs... Dans le cadre d'utilisation canonique, ces instruments renvoient néanmoins l'image finale à l'infini.
````

## Caractéristiques générales: Champ, résolution et profondeur de champ (en ligne)

````{topic} Caractéristiques générales
* Champ angulaire : écart angulaire maximal pouvant être vue par l'instrument d'optique.
* Pouvoir de résolution : angle minimal nécessaire pour pouvoir distinguer (résoudre) deux objets visés.
* Profondeur de champ : intervalle de position permettant d'être vue nette à travers l'instrument pour un réglage donné.
* Latitude de mise au point : gamme de réglage (et position) possible de l'instrument d'optique permettant à l'oeil de l'observateur d'observer l'objet net (l'image finale vue donnée par l'instrument - donc l'objet vu par l'oeil - doit être entre le Punctum Proximum et le Punctum Remotum). La latitude de mise au point dépendant de l'oeil de l'observateur, on déterminer implicitement la latitude de mise au point du système {instrument + oeil}
    * _En pratique, ces grandeurs dépendent du système d'observation derrière l'instrument (en pratique l'oeil de l'observateur). C'est pourquoi on parle en général du champ angulaire/résolution... du système {instrument + oeil}._
````

## Le grossissement

````{topic} Problème du grandissement
Le grandissement ne donne pas forcément d'information utile pour un objet/image vu par l'oeil car la taille apparente dépend de la distance à l'objet (un objet à l'infini a une taille... infinie).

On utilise plutôt _l'angle sous lequel est vu un objet_ et la tendance à _grossir_ est associée au __grossissement__ : un rapport _d'angle_ sous lequel est vu l'objet avec l'appareil et à l'oeil nu.
````
````{important} __Grossissement__

On définit le __grossissement__ d'un instrument d'optique comme le rapport (en valeur absolue) de l'angle sous lequel on voit l'objet à travers l'instrument d'optique sur l'angle sous lequel on voit l'objet à l'oeil nu.
````

````{topic} Cadre d'utilisation du grossissement
Le grossissement dans le cas général dépend de la position de l'objet visé (si l'image n'est pas renvoyé à l'infini) et de la position de l'oeil (si l'objet n'est pas à l'infini).

C'est pourquoi, on utilisera le grossissement principalement __pour les instruments d'optique afocaux.__

Comme nous allons le voir, pour les instruments visant un objets à distance finie, les constructeurs donnent une donnée commercial dans une utilisation canonique: on calcule ou mesure le grossissement dans des conditions optimales: l'image finale sera à l'infini et l'angle à l'oeil nu est le plus grand possible, d'où la définition:
````

````{important} __Grossissement commercial__

On définit le __grossissement commercial__ d'un instrument d'optique comme le rapport (en valeur absolue) de l'angle sous lequel on voit l'objet à travers l'instrument d'optique __lorsque l'image finale est à l'infini__ sur l'angle sous lequel on voit l'objet à l'oeil nu __lorsque l'objet est placé au Punctum Proximum de l'oeil soit à $d=25\rm{cm}$__ (soit l'angle maximal sous lequel on peut voir l'objet à l’oeil nu).
````