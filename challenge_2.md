Challenge 2 - Make it pretty !
================

### Section 1: Faire le pont ! (15 min)

Comme nous l'avons vu pendant le cours, nous avons besoin de lier notre page HTML à notre page CSS.

1. Nous devons donc dire à notre page HTML où trouver la page CSS

Afin d'être sur que le lien ait été correctement établie , vous pouvez écrire une déclaration plutôt voyante comme celle-ci:

```css

body {
  background: lightblue;
}

```

> Pour les plus geek, ouvrez l'inspecteur d'élément, allez sur l'onglet réseau, recharger la page, et verifiez que le fichier style.css charge.


### Section 2: Créer les blocs ! (1h30)

> Lorsque vous écrivez vos "class" et "Id", n'écrivez pas:
  .x or .y, etc
Préférez:
  .menu .menu__ul .menu__li

1. Commencer par le haut de votre site puis descendez progressivement
  - Réalisez dans un premier temps
    - Le header
    - Le menu
    - etc

2. Essayez de positionner vos éléments de façons intelligente.
  - Votre header peut être un bloc, relatif au body, avec une certaine hauteur.
  - Ceci vous aidera à placer de facon automatique les éléments

>Ceci est un exemple, il existe un nombre quasi illimité de solution pour créer votre page. Vous pouvez essayer de le faire de cette façon car elle est assez classique.

([Prenez cette pillule :pill:](https://github.com/makersacademy/taster2.0/blob/master/assets/pills/css.md "Taster v1") si vous avez des difficultés)

Pour ne pas perdre la tête avec le CSS, vous devez faire attention de ne pas cibler directement les éléments par leur balise mais par une Classe (.x) ou une ID (#x).

C'est pourquoi nous vous avons demander de coder votre structure HTML avant, afin de donner des nom coherent à vos differents blocs.

>Le ptit +: Commentez votre code!

[Challenge suivant, be Responsive!](https://github.com/makersacademy/taster2.0/blob/master/challenge_3.md "Challenge 3")
