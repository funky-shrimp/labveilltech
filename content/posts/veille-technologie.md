---
date: '2026-01-19T18:38:15+01:00'
draft: false
title: 'Veille Technologie'
---

## Ma philosophie technologique

J'ai une philosophie simple, d'une part parce que je suis étudiant et que je n'ai pas un Kopeck et d'une autre parce que j'aime les solutions techniques où je suis libre.

> If buying isn't owning, piracy isn't stealing

Pour ma veille technologique, j'ai choisis des solutions libres et pour lesquelles je ne suis pas dépendant des géants de la tech qui revendent nos données.

## Système d'écoute
Je voulais une solution qui me permettait de sauvegarder les articles qui m'intéressaient, y avoir accès sur mes appareils et garder privées mes données. Mon oeil portait déjà sur Obsidian.

Lors de mes recherches, [cet article](https://www.stephanmiller.com/sync-obsidian-vault-across-devices/) m'a permis de me diriger vers la solution que j'ai adopté.

Pour illustrer mes prochains propos, rien de mieux qu'un petit schéma de ma techstack.

![Illustration de la techstack de ma solution](/images/LabVeillTech-Veille_technologique.png)


### Obsidian et RSS Dashboard
Je me suis mis récemment à [Obsidian](https://obsidian.md/) pour m'essayer à la méthodologie "*second brain*" afin de m'y retrouver dans mes idées. Et j'ai pensé intéressant d'intégrer un flux RSS dans l'application.

En faisant mes recherches, j'ai découvert que l'on pouvait intégrer des plugins à Obsidian et je suis tombé sur [RSS Dashboard](https://github.com/amatya-aditya/obsidian-rss-dashboard) de Amatya Aditya et les fonctionnalités que le plugin propose réponde à plusieurs critères que j'avais au préalable pour un tel outil :
- Pouvoir enregistrer les articles
- Pouvoir les modifier et partager facilement
- Le tout dans un format simple et pérenne dans le temps

Parfait ! Ce format c'est le [Markdown](https://www.markdownguide.org/getting-started/)

Donc j'ai installé Obsidian sur mon PC et mon téléphone. Mais il fallait encore pouvoir consulter ce flux RSS sur mon téléphone. C'est là que [Syncthing](https://syncthing.net/) rentre en jeu.

### Syncthing
Syncthing me permet de synchroniser mon laptop avec mon smartphone sans être dépendant d'une solution d'un géant de la tech (One Drive, Google Drive...). Syncthing utilise le réseau local (Wifi) pour synchroniser les fichiers. Dans le cas où les appareils ne sont pas sur le même réseau, Syncthing utilise des serveurs relay maintenu par la communauté.
Mais ce choix de solution vient avec un coup : **La configuration**

En effet, j'ai dû un peu bidouillé pour lier mon *vault* Obsidian sur mon téléphone. J'ai dû installer un explorateur de fichier [Material Files](https://play.google.com/store/apps/details?id=me.zhanghai.android.files&hl=en_US) me permettant d'avoir un accès total aux dossiers de mon Google Pixel 7.

Concernant ce dernier, j'ai dû installer un [*fork* de Syncthing](https://github.com/researchxxl/syncthing-android) afin d'avoir cette application sous Android.

Finalement, la synchronisation fonctionne, mais je rencontre encore un petit soucis de synchronisation par rapport au plugin RSS Dashboard. Lorsque j'ajoute un flux RSS sur l'un de mes deux appareils, et que j'ouvre Obsidian sur l'autre, sa version du flux RSS (plus ancienne) écrase la nouvelle. Résultat, je n'arrive pas à avoir une parfait synchronisation. Je n'ai pas pris le temps de trouver une solution à ce problème, pour l'instant je dois ajouter le nouveau flux RSS depuis mon PC, lancer un scan avec Syncthing sur mon téléphone puis lancer Obsidian.

## Mon flux d'écoute

Mon flux d'écoute est le suivant :

- Smashing Magazine (JS, CSS)
- Webflow blog
- CSS Tricks
- Free Code Camp
- DEV Community
- MDN Blog

Cependant je dois encore trier et catégoriser les flux d'écoutes. Pour certains d'entre eux, je suis abonné au flux principal où tout type d'articles sont postés.

