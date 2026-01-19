---
date: '2026-01-19T23:26:50+01:00'
draft: false
title: 'CSS - Visualiser les transitions entre les pages'
---

## Visualiser les transitions
Jusqu'à maintenant, les transitions étaient réservées que pour les SPA *(Single Page Application)*.
Dorénavant, les MPA *(Multiple Page Application)* peuvent aussi en profiter.

![GIF de la transition](/images/LabVeillTech-view_transition.gif)

En d'autres termes : On peut avoir des transitions lors de la navigation entre les pages !!!

Pour cela rien de plus simple, une ligne de CSS suffit :

```css
@view-transition {
  navigation: auto;
}
```

Pour aller plus loin, [l'article](https://developer.mozilla.org/en-US/blog/view-transitions-beginner-guide/#going_beyond_the_default_transition) de Yash Raj Bharti nous montre comment avoir la même transition que sur le GIF ci-dessus.

## Sources
- [MDN - A beginner-friendly guide to view transitions in CSS](https://developer.mozilla.org/en-US/blog/view-transitions-beginner-guide/)
- [MDN - #view-transition](https://developer.mozilla.org/en-US/docs/Web/CSS/Reference/At-rules/@view-transition)