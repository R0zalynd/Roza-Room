---
title: Un seul anneau, avec queue d'aronde intégrée
description: Passage à un anneau unique avec la queue d'aronde intégrée, et nouvelles mesures du cache-pot par périmètres.
project: accroche-plante
image: /projects/accroche-plante/conception/anneau-queue-d-aronde-cao.png
tags:
  - mécanique
  - impression 3D
---

Passage à un seul anneau, qui intègre directement la queue d'aronde : plus de pièce d'interface, et de nouvelles mesures du cache-pot pour le dimensionner.

<!--more-->

## Evolutions du design

- **Un seul anneau au lieu de deux :**
  - par choix de design ;
  - parce qu'avec deux anneaux, sans un modèle parfait du pot, ils n'auraient jamais été parfaitement ajustés en même temps;
- **Queue d'aronde (dovetail) intégrée à l'anneau**, ce qui supprime la pièce d'interface qui servait de glissière. Ça règle le problème de solidité de l'insert et le manque de visserie relevés lors de l'[impression des premières pièces]({{ '/journal/2026/09/30/impression-premieres-pieces/' | relative_url }}).
- **Réduction de l'accroche sur l'escalier :**  Avec un seul anneau, la pièce n'a pas besoin d'être aussi grande. Sachant que j'ai 5 pots à accrocher au total, réduire la taille des pièces n'est pas une mauvaise option.

## Mesures pour le nouvel anneau

<div class="box doc-meta bloc-image" markdown="1">
<div class="bloc-image-texte" markdown="1">

Mesure de deux périmètres, $$P_1$$ et $$P_2$$, à 25 mm d'écart en hauteur, à l'aide d'une bande de scotch.

Le rayon se déduit du périmètre d'un cercle :

$$P = 2\pi \times r \iff r = \frac{P}{2\pi}$$

D'où, avec $$P_1 = 42{,}3\ \text{cm} = 423\ \text{mm}$$ et $$P_2 = 410\ \text{mm}$$ :

$$r_1 = \frac{P_1}{2\pi} = \frac{423}{2\pi} \approx 67\ \text{mm}$$

$$r_2 = \frac{P_2}{2\pi} = \frac{410}{2\pi} \approx 65\ \text{mm}$$

Le rayon diminue donc d'environ 2 mm sur 25 mm de hauteur, soit une paroi inclinée de :

$$\alpha = \arctan\left(\frac{r_1 - r_2}{25}\right) \approx 4{,}7^\circ$$

Mes mesures ne sont pas forcément ultra précises, je rajouterais un peu de jeux sur la CAO.

</div>
<figure class="bloc-image-media" markdown="0">
<img src="{{ '/projects/accroche-plante/mesures/perimetres-scotch.jpg' | relative_url }}" alt="Cache-pot entouré d'une bande de scotch de 25 mm de haut, avec repères, pour mesurer les deux périmètres">
</figure>
</div>

## Ajustement du modèle CAO

Je profite de ce projet pour tester des fonctionnalités d'Onshape : pour modifier mon fichier j'ai créée une branche "anneau unique" pour garder en mémoire la première version si jamais je souhaite revenir en arrière par la suite.

Pour la création des différentes pièces, je prends le temps de tester des fonctions plutôt que d'aller au plus efficace. Par exemple, j'expérimente un peu avec des opérations booléennes, des configurations, du lissage ou du surfacique (non concluant dans ce cas précis). Pour l'instant, mon assemblage est strictement fixe donc tout est dans un seul part-studio. Il faudra que je teste plus en détails l'assembly-studio sur un autre projet, ou en reprenant les parts de celui-ci même si les degrés de liberté ne sont pas très intéressants. 

### Anneau de support avec queue d'aronde

En passant à un seul anneau j'ai peur que ce ne soit plus très solide, donc j'ajoute un peu d'épaisseur et de hauteur par rapport à la version précédente. En ajoutant la queue d'aronde directement à l'anneau je supprime le besoin d'une pièce d'interface. 

<div class="images-cote" markdown="0">
<img src="{{ '/projects/accroche-plante/conception/anneau-queue-d-aronde-cao.png' | relative_url }}" alt="Nouvel anneau unique avec sa queue d'aronde, fixé sur l'escalier (CAO)">
<img src="{{ '/projects/accroche-plante/conception/anneau-queue-d-aronde-detail.png' | relative_url }}" alt="Anneau seul autour du cache-pot, avec la queue d'aronde intégrée (CAO)">
</div>

### Pièces d'accroche sur l'escalier

- **Pièces plus petites**, en cohérence avec le passage à un seul anneau.
- **Un peu de jeu ajouté sur les faces en contact avec la rambarde :** selon le barreau testé, l'ajustement était parfois trop juste, car les barreaux ne sont pas uniformes (couches de peinture, etc.).

<div class="images-cote" markdown="0">
<img src="{{ '/projects/accroche-plante/conception/accroche-escalier-reduite-cao.png' | relative_url }}" alt="Pièce d'accroche réduite autour du barreau, avec l'anneau en transparence (CAO)">
<img src="{{ '/projects/accroche-plante/conception/accroche-escalier-ensemble-cao.png' | relative_url }}" alt="Ensemble monté sur l'escalier : accroche réduite, anneau, cache-pot avec plaque de drainage et tube d'évacuation (CAO)">
</div>

## Prochaines étapes

- [ ] Imprimer un set complet pour tout tester, monter le prototype et le laisser une semaine pour vérifier qu'il supporte bien la charge
- [ ] Imprimer l'anneau avec des paramètres « strength » (solidité)

