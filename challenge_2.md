Challenge 2 - Make it pretty !
================

### Section 1: Faire le pont ! (15 min)

Comme nous l'avons vu pendant le cours, nous avons besoin de lier notre page HTML à notre page CSS.

1. Nous devons donc dire à notre page HTML où trouver la page CSS

Afin d'être sur que le lien ait été correctement établie , vous pouvez écrire une declaration plutôt voyante comme celle-ci:

```css

body {
  background: lightblue;
}

```

> Pour les plus geek, ouvrez l'inspecteur d'élément, allex sur l'onglet réseau, recharger la page, et verifiez que le fichier style.css charge.


### Section 2: Create the blocks ! (1h30)

> Lorsque vous écrivez vos "class" et "Id", n'écrivez pas:
  .x or .y, etc
Préférez:
  .menu .menu__ul .menu__li

1. Commencer par le haut de votre site et descendez progressivement
  - Réalisez dans un premier temps le header
  - Needs to be a block that push other elements underneath
  - It has the "monospace" font
  - The link (make it open in a new tab with an attribute)

2. Go on with the article:
  - Is relatively positioned after the menu
  - The width is about 80vw (learn about vw and vh units)
  - In order to put the picture on the right and the text on the left, you can float: left; the text.

3. The footer
  - Can be in position: fixed;
  - the text is centered by default

>This is exhaustive, you can do whatever you want, but try to think in this way.

([take this pill :pill:](https://github.com/makersacademy/taster2.0/blob/master/assets/pills/css.md "Taster v1") if you have some trouble)

To not loose your mind with CSS, you need to be careful and not write on top on the other rules.
That's why, we recommend you to code the structure of your page first and after to make it pretty.

[Next challenge, be Agile!](https://github.com/makersacademy/taster2.0/blob/master/challenge_3.md "Challenge 3")
