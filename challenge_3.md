Challenge 4 - Be responsive !
================

Ok, donc maintenant vous avez une page web, stylisé, il ne reste plus qu'à la rendre jolie sur tous les supports.

Pour ce faire, nous utiliserons la technique vue pendant le cours, les media queries!

### Section 1 : Ma première media ! (20 min)

Ici on vous conseille d'essayer de faire des colonnes qui se réagenceront toutes seules au format mobile ou tablette.

1. Pour rappel, la media queries s'écrit dans la feuille de style CSS.
2. Repérer un comportement non souhaité lorsque vous redimensionnez votre fenêtre et décidez de ce que vous allez en faire.
3. Ouvrez l'inspecteur d'élément et repérez le breakpoint sur lequel il va falloir agir.
   Pour ce faire regarder les pixels comme sur la photo ci-dessous.
![Pixel inspector image](https://raw.githubusercontent.com/Coding-Days/coding-days/master/assets/images/Challenge%204/pixel-inspecteur.jpg)
4. Une fois votre breakpoint repéré, définissez votre media, elle peut avoir plusieurs formes:
    - @media screen and (max-width: 640px)
    - @media screen and (min-width: 200px) and (max-width: 640px)

>Si vous voulez une liste non exhaustive mais bien complète, c'est [ici](https://github.com/makersacademy/taster2.0/blob/master/challenge_4.md "Challenge 4") https://css-tricks.com/snippets/css/media-queries-for-standard-devices/

Pour rappel, une media querie s'écrit comme suit :

```css

@media screen and (max-width: 640px) {
  .header {
    width: 600px;
  }
  /* Mes autres déclarations */
}

```
### Section 2 : On check et double check ! (15 min)

On l'a déjà dit, mais l'inspecteur d'élément, c'est juste indispensable.. Il existe une fonction qui va vous permettre d'émuler le terminal sur lequel vous travaillez.
Regardez la photo ci-dessous et cliquez sur l'icône.

![Pixel inspector image](https://raw.githubusercontent.com/Coding-Days/coding-days/master/assets/images/Challenge%204/device-emulator.jpg)

Vous pouvez donc écrire et checker votre code en live afin d'aller à l'essentiel !

> N'oubliez pas la règle d'héritage, mettez vos media à la fin de votre code pour qu'elle s'exécute après le code desktop.

**Lorsque vous arrivez là, que vous avez écrit quelques media dites-le-nous pour que l'on passe au cours sur les librairies et framework! :)**

[Prêt pour la mise en ligne ?  !](https://github.com/Coding-Days/coding-days/blob/master/challenge_4.md "Challenge 4")
