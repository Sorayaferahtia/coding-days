Challenge 2 - Make it pretty !
================


### Section 1 : Faire le pont ! (20 min)

Comme nous l'avons vu pendant le cours, nous avons besoin de lier notre page HTML à notre page CSS.

1. Nous devons donc dire à notre page HTML où trouver la feuille de style CSS.

> Rappelez-vous... Où est-ce que l'on indique la localisation d'un ou plusieurs profils de métadonnées ?

2. Maintenant, on va vérifier notre travail! Afin d'être sûr que le lien ait été correctement établi, vous pouvez écrire une déclaration assez voyante comme celle-ci :

```css

body {
  background: lightblue;
}

```

> Pour les plus geek, ouvrez l'inspecteur d'élément, allez sur l'onglet réseau, recharger la page, et vérifiez que le fichier style.css charge correctement.

### Section 2 : Créer les blocs ! (1h30)

> Lorsque vous écrivez vos "class" et "Id", n'écrivez pas:
  .x or .y, etc
Préférez:
  .menu .menu__ul .menu__li

C'est pourquoi nous vous avons demander de dessiner, puis coder votre structure HTML avant, dans le but de donner des noms cohérents aux différents class et ID de vos blocs.

>Le ptit +: Commentez et indentez votre code correctement!

([Prenez cette pilule :pill:](https://github.com/Coding-Days/coding-days/blob/master/assets/pills/css.md "csspill") si vous avez des difficultés), gulp

1. Commencez par le haut de votre site puis descendez progressivement
  - Réalisez dans un premier temps
    - Le header
    - Le menu
    - etc
2. Essayez de positionner vos éléments de façons intelligentes.
  - Votre header peut être un bloc, relatif au body, avec une certaine hauteur.
  - Ceci vous aidera à placer de façon automatique les éléments en dessous les uns par rapport aux autres.

3. Toujours sur le header, vous pouvez choisir plusieurs options

Voici deux header légèrements différents:

**Sans container**
![header no container](https://raw.githubusercontent.com/Coding-Days/coding-days/master/assets/images/CSS%20Challenge/header__noContainer.png)
**Avec container**
![header container](https://raw.githubusercontent.com/Coding-Days/coding-days/master/assets/images/CSS%20Challenge/header__container.png)

Imaginez votre site sur plusieurs supports...

Sur votre ordinateur portable 13 ou 15 pouces, pas vraiment de soucis à avoir un header qui prend toute la longueur..

Mais sur un 24, 27 pouces ou une télé?

  - Si vous n'avez pas de container, votre header va prendre toute la longueur (du block), donc la longueur de l'écran sur lequel il est.

  - Si vous avez un container qui a :
    - Soit une longueur en px,
    - Soit une longueur en %,
    - Voir une autre unité (allez fouiner sur le web).

  Vous allez pouvoir encapsuler votre contenu qui sera alors positionné relativement par rapport à celui-ci.

  Concrètement, il va prendre sa taille quoi...
    - Mon container width: 80%;
      - Mon header en display: block;

    - Si vous vous demandez pourquoi est-t-il positionné à gauche et pas au milieu comme sur la photo, je suis certain que vous allez trouver comment le centrer!



[Next Challenge, be Responsive!](https://github.com/Coding-Days/coding-days/blob/master/challenge_3.md "Challenge 3")
