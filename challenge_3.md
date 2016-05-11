Challenge 3 - Make it pretty !
================

### Section 1: Faire le pont ! (15 min)

Comme nous l'avons vu pendant le cours, nous avons besoin de lier notre page HTML à notre page CSS.

1. Nous devons donc dire à notre page HTML où trouver la feuille de style CSS.

> Rappelez vous... Où est ce que l'on indique la localisation d'un ou plusieurs profils de métadonnées?

2. Maintenant, on va vérifier notre travail! Afin d'être sur que le lien ait été correctement établie, vous pouvez écrire une déclaration assez voyante comme celle-ci:

```css

body {
  background: lightblue;
}

```

> Pour les plus geek, ouvrez l'inspecteur d'élément, allez sur l'onglet réseau, recharger la page, et verifiez que le fichier style.css charge correctement.


### Section 2: Créer les blocs ! (1h30)

> Lorsque vous écrivez vos "class" et "Id", n'écrivez pas:
  .x or .y, etc
Préférez:
  .menu .menu__ul .menu__li

C'est pourquoi nous vous avons demander de dessiner, puis coder votre structure HTML avant, dans le but de donner des noms cohérents aux différents class et ID de vos blocs.

>Le ptit +: Commentez et Indentez votre code!

([Prenez cette pillule :pill:](https://github.com/makersacademy/taster2.0/blob/master/assets/pills/css.md "Taster v1") si vous avez des difficultés), gulp

1. Commencer par le haut de votre site puis descendez progressivement
  - Réalisez dans un premier temps
    - Le header
    - Le menu
    - etc
2. Essayez de positionner vos éléments de façons intelligente.
  - Votre header peut être un bloc, relatif au body, avec une certaine hauteur.
  - Ceci vous aidera à placer de facon automatique les éléments en dessous les uns par rapport aux autres.

3. Toujours sur le header, vous pouvez opter pour plusieurs options

Voici deux header lègerement diffèrents:

**Sans container**
![header no container](https://raw.githubusercontent.com/Coding-Days/coding-days/master/assets/images/CSS%20Challenge/header__noContainer.png)
**Avec container**
![header container](https://raw.githubusercontent.com/Coding-Days/coding-days/master/assets/images/CSS%20Challenge/header__container.png)

Imaginez votre site sur plusieurs support...

Sur votre ordinateur portable 13 ou 15 pouces, pas vraiment de soucis à avoir un header qui prend toute la longueur..

Mais sur un 24, 27 pouces ou une télé?

  - Si vous n'avez pas de container, votre header va prendre toute la longueur (du block), donc la longueur de l'écran sur lequel il est.

  - Si vous avez un container qui a:
    - Soit une longueur en px,
    - Soit une longueur en %,
    - Voir une autre unité (allez fouiner sur le web).

  Vous allez pouvoir encapsuler votre contenu qui sera alors positionner relativement par rapport à celui-ci.

  Concrètement, il va prendre sa taille quoi...
    - Mon container width: 80%;
      - Mon header en display: block;

    - Si vous vous demandez pourquoi est-ce qu'il est positioné à gauche et pas au milieu comme sur la photo, je suis certain que vous allez trouver comment le centrer!



[Challenge suivant, be Responsive!](https://github.com/makersacademy/taster2.0/blob/master/challenge_3.md "Challenge 3")
