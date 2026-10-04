---
title: Lampe à poser - inspiration Design Studio 407
description: Recréer la lampe à panneaux ouvrants de Design Studio 407, motorisée et habillée de laiton/bronze et de noyer.
image: /esquisses/images/lampe-a-poser-studio-407/croquis.jpg
tags:
  - luminaire
  - impression 3D
  - électronique
  - finitions
---

Une lampe à poser inspirée de Design Studio 407 : panneaux ouvrants motorisés, réglés par un potentiomètre, et finitions laiton/bronze et noyer.

<!--more-->

## L'inspiration

La lampe « 겹 (Gyeop) : 빛을 여닫는 겹의 조명 » (environ : *Couches : la lampe dont les couches ouvrent et ferment la lumière*) de [Design Studio 407](https://www.instagram.com/design_studio_407/). Ses panneaux empilés se règlent pour choisir la direction et l'intensité de la lumière.

- [Page du produit](https://407.co.kr/product/%EA%B2%B9-%EB%B9%9B%EC%9D%84-%EC%97%AC%EB%8B%AB%EB%8A%94-%EA%B2%B9%EC%9D%98-%EC%A1%B0%EB%AA%85/293/category/24/display/1/) (130 000 KRW)
- [Publication Instagram](https://www.instagram.com/p/DLyiisAzg3Q/)

## Ce que j'aime

- Le côté industriel
- La lumière douce et réglable
- Les finitions propres
- Les matériaux « nobles »

## L'idée

<div class="box doc-meta bloc-image" markdown="1">
<div class="bloc-image-texte" markdown="1">

- La lampe n'est pas livrée en dehors de la Corée : la refaire moi-même.
- Ajouter une motorisation commandée par un potentiomètre, qui sert de variateur : il fait bouger les panneaux ouvrants et varier la lumière.
- L'adapter à ma décoration actuelle avec des touches de laiton/bronze et/ou de noyer.

</div>
<figure class="bloc-image-media" markdown="0">
<img src="{{ '/esquisses/images/lampe-a-poser-studio-407/croquis.jpg' | relative_url }}" alt="Croquis de la lampe : extérieur effet bois, visserie laiton, dessous des panneaux mobiles en laiton, base pour cacher la carte et le servomoteur, variateur à potentiomètre">
</figure>
</div>

## À tester

Matériel à disposition : une imprimante 3D. Comment obtenir les effets métal et bois ?

### Effet bois

- [ ] Imprimer avec un filament effet bois
- [ ] Si impression 3D : comment ajouter une texture pour le veinage, et du multicouleur pour les nœuds ?
- [ ] Coller un placage de noyer, type bande de chant, sur une plaque imprimée
- [ ] Possible de faire une plaque avec l'extérieur en bois et la tranche en métal ?

### Effet métal (laiton/bronze)

- [ ] Galvanoplastie, ou électrodéposition ([vidéo de référence](https://www.youtube.com/watch?v=zzQSOLA8qzs))
- [ ] Feuille de placage métallique
- [ ] Adhésif vinyle métallisé
- [ ] Filament effet métal
- [ ] Visserie effet laiton ?

### Motorisation

- [ ] Micro servomoteur type SG90 : probablement suffisant pour bouger les panneaux, à vérifier
- [ ] Trouver un système pour bouger tous les panneaux en même temps. Pistes :
  - une tringle commune reliée à chaque panneau par une petite biellette, comme sur des persiennes ;
  - un engrenage ou une crémaillère qui fait tourner tous les axes ensemble.

## À prévoir

### Matériaux

- La lampe chauffe : choisir un plastique résistant à la chaleur, au moins pour les pièces proches de la source de lumière.
- La visserie en laiton est en général peu solide : se renseigner plus en détail, ou trouver une alternative et la remplacer, même si elle colle moins à l'esthétique recherchée.

### Électronique

- Alimentation de l'ampoule
- Carte électronique pour piloter le servomoteur et le variateur ?
- Une base en bois pour cacher la carte et le servomoteur ?
- Avec un microcontrôleur, prévoir éventuellement une communication Bluetooth/Wi-Fi pour en faire une lampe connectée : allumage et ouverture automatiques selon l'heure, par exemple. Un ESP32 ? (il intègre Wi-Fi et Bluetooth)
