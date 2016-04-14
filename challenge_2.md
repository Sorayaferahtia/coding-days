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

> Pour les plus geek, ouvrez l'inspecteur d'élément, allez sur l'onglet réseau, recharger la page, et verifiez que le fichier style.css charge correctement.


### Section 2: Créer les blocs ! (1h30)

> Lorsque vous écrivez vos "class" et "Id", n'écrivez pas:
  .x or .y, etc
Préférez:
  .menu .menu__ul .menu__li

C'est pourquoi nous vous avons demander de coder votre structure HTML avant, afin de donner des nom coherent à vos differents blocs.

>Le ptit +: Commentez et Indentez votre code!

([Prenez cette pillule :pill:](https://github.com/makersacademy/taster2.0/blob/master/assets/pills/css.md "Taster v1") si vous avez des difficultés)

1. Commencer par le haut de votre site puis descendez progressivement
  - Réalisez dans un premier temps
    - Le header
    - Le menu
    - etc
2. Essayez de positionner vos éléments de façons intelligente.
  - Votre header peut être un bloc, relatif au body, avec une certaine hauteur.
  - Ceci vous aidera à placer de facon automatique les éléments en dessous les uns par rapport aux autres.

3. Toujours sur le header, vous pouvez opter pour plusieurs options
- Quelle est la difference entre ces deux exemples!?

**Sans container**
![header no container](https://raw.githubusercontent.com/Coding-Days/coding-days/master/assets/images/CSS%20Challenge/header__noContainer.png)
**Avec container**
![header container](https://raw.githubusercontent.com/Coding-Days/coding-days/master/assets/images/CSS%20Challenge/header__container.png)

Imaginez maintenant votre site sur plusieurs support...

Sur votre ordinateur portable 13 ou 15 pouces, pas vraiment de soucis à avoir un header qui prend toute la longueur..

Mais sur un 24, 27 pouces ou une télé?

  - Si vous n'avez pas de container votre header va prendre toute la longueur (du block), donc de votre page, concrètement, la longueur de l'écran sur lequel il est.

  - Si vous avez un container qui a soit une longueur en px, soit une longueur en %, voir autres. Vous allez pouvoir encapsuler votre contenu qui sera alors positionner relativement par rapport à celui-ci.
  En gros il va prendre sa taille quoi...
    - Mon container width: 80%;
      - Mon header en display: block;

    - Si vous vous demandez pourquoi est-ce qu'il est positioné à gauche et pas au milieu comme sur la photo, je suis sur que vous allez trouver comment le centrer!



[Challenge suivant, be Responsive!](https://github.com/makersacademy/taster2.0/blob/master/challenge_3.md "Challenge 3")
