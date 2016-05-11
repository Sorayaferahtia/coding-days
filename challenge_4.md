Challenge 4 - Be responsive !
================

Ok, donc maintenant vous avez une page web, stylisé, il ne reste plus qu'à la rendre jolie sur tous les supports.

Pour ce faire, nous utiliserons la technique vue pendant le cours, les media queries!

### Section 1: Ma première media ! (15 min)

Ici on vous conseil d'essayer de faire des colones qui se ré-agenceront toutes seules au format mobile ou tablette.

1. Pour rappel, la media queries s'écrit dans la feuille de style CSS.
2. Repérer un comportement non souhaité lorsque vous redimensionnez votre fenêtre et décidez de ce que vous allez en faire.
3. Ouvrez l'inspecteur d'élément et repérez le breakpoint sur lequel il va falloir agir.
   Pour ce faire regarder les pixels comme sur la photo ci-dessous.
![Pixel inspector image](https://raw.githubusercontent.com/Coding-Days/coding-days/master/assets/images/Challenge%204/pixel-inspecteur.jpg)
4. Une fois votre breakpoint repéré, définissez votre media, elle peut avoir plusieurs forme:
    - @media screen and (max-width: 640px)
    - @media screen and (min-width: 200px) and (max-width: 640px)

>Si vous voulez une liste non exhaustive mais bien complète, c'est [ici](https://github.com/makersacademy/taster2.0/blob/master/challenge_4.md "Challenge 4") https://css-tricks.com/snippets/css/media-queries-for-standard-devices/

Pour rappel une media querie s'écrit comme suit:

```css

@media screen and (max-width: 640px) {
  .header {
    width: 600px;
  }
  /* Mes autres déclarations */
}

```
### Section 2: On check et double check ! (15 min)

On l'a déjà dit, mais l'inspecteur d'élément, c'est juste indispensable.. Il existe une fonction qui va vous permettre d'emuler le terminal sur lequel vous travaillez.
Regardez la photo ci-dessous et cliquez sur l'icone.

![Pixel inspector image](https://raw.githubusercontent.com/Coding-Days/coding-days/master/assets/images/Challenge%204/device-emulator.jpg)

Vous pouvez donc écrire et checker votre code en live afin d'aller à l'essentiel!

> N'oubliez pas la règle d'heritage, mettez vos media à la fin de votre code pour qu'elle s'execute après le code desktop.

**Lorsque vous arrivez là, que vous avez écrit quelques media dites le nous pour que l'on passe au cours sur les librairies et framework! :)**

### Section 3: Du responsive avec bootstrap avec jquery! (15 min)

Vous savez maintenant ce qu'est une librairie et un framework! Nous allons desormais utilisé les deux!

Pour ce faire:

1. Il faudra faire le lien avec les fichiers souhaitez. Il existe deux façons de faire:
  - Faire appel aux fichiers à partir d'un CDN (Content Delivery Network), ce qui veut dire que les fichiers sont sur un serveur distant (pas le votre), et que vous lui demander, à chaque chargement de page, de vous donner les infos.

>**Pros** Ca va plus vite, le chargement de ces fichiers n'est pas à la charge de votre serveur.
**Cons** Ça peut être risqué si le CDN est down (tombe), ce qui veut dire qu'il ne sera pas actif et ne pourra pas vous communiquer les fichiers.

  - Faire appel aux fichiers à partir de votre serveur. Vous stockerai donc les fichier dans votre site et ils seront donc toujours dispo.

> Si quelqu'un trouve la solution pour bénéficier du beurre, l’argent du beurre et du cul de la fermière, dites le nous! Il y en a une ;) !

2. Aujourd'hui, nous ferons appel au CDN, c'est la solution la plus simple pour être up and running rapidement.

3. Rappellez vous du cours d'hier sur le pont à faire entre vos fichiers HTML et CSS/JS
  - Où fait-on le pont?
  - Vers quelle source ou href la balise pointera?

> Voici deux liens vers les deux CDN dont nous auront besoin:

BootStrap: https://maxcdn.bootstrapcdn.com/bootstrap/3.3.6/css/bootstrap.min.css
jQuery: https://code.jquery.com/jquery-2.2.3.min.js

Faites ce qu'il faut faire avec ;)

### Section 4: BootStrap et son Grid magique! (15 min)

Maintenant que vous avez bien galéré avec vos colonnes au format tablette ou mobile on va voir comment bootstrap peut vous aider!

>Pour Rappel, Bootstrap vous propose des class (entre autre, mais nous n'utiliserons que ça ce week-end) qui changeront le comportement de vos blocks une fois mis en place.

Le grid bootstrap se présente comme suit:
![Grid bootstrap image](https://bootstrapbay.com/blog/wp-content/uploads/2014/09/bootstrap-grid-system.jpg)

Le colonnes sont donc très facilement maléable, et si vous souhaitez un comportement différent selon les terminaux, vous pouvez utiliser differentes colonnes:

![Pixel inspector image](https://raw.githubusercontent.com/Coding-Days/coding-days/master/assets/images/Challenge%204/colonnes-bootstrap.png)


Pour effectuer un grod bootstrap sur votre site il y a plusieurs conditions:
1. Créer un container:
```html
<article class="container">

</article>
```
2. Créer une row qui aura pour but de créer un groupe horizontal de colonnes.
```html
<article class="container">
  <section class="row">

  </section>
</article>
```
3. Créer desormais vos colonnes:
```html
<article class="container">
  <section class="row">
    <div class="col-md-6">
      Mon contenu à gauche
    </div>
    <div class="col-md-6">
      Mon contenu à droite
    </div>
  </section>.;
</article>
```

Les colonnes vont donc s'agencées toutes seules :).


>Plus de doc [ici](https://getbootstrap.com/css/#grid "bootstrap")

### Section 5: Un peu de jQuery maintenant! (15 min)

Afin que vous compreniez facilement comment le JS est utilisé, on utilisera la librairie jQuery qui vous permettra d'écrire du JS très simplement!

On ne va pas pousser trop loin mais essayer simplement de faire changer le comportement de la page du coté client.

Ce qu'on vous propose aujourd'hui c'est de changer les titres de couleur 10 secondes après que la page ait chargée!

On utilisera donc plusieurs fonctions:
- $( document ).ready(function() pour faire en sorte d'être sur que la page soit bien chargée avant d'executer notre code.
- setTimeout(function(){ votre code }, les milli secondes); Pour dire à la page d'attendre X secondes.
- $( "selecteur" ).css("declaration", "valeur"); Pour dire à un selecteur de changer son style.

> On vous propose de changer la couleur des titres apres 10 secondes, mais si vous avez des idées similaires, faites vous plaisir!

Quelques liens utiles:
- https://learn.jquery.com/using-jquery-core/document-ready/
- http://www.sitepoint.com/jquery-settimeout-function-examples/
- http://api.jquery.com/css/

La solution est là mais essayé de ne pas la regarder!

>!
  jQuery( document ).ready(function() {
    setTimeout(function(){
      jQuery("h1, h2, h3, h4, h5, h6").css("color", "red");
      alert("Yataaa!!");
    }, 10000);
  });






[Next challenge, Your fisrt project !](https://github.com/makersacademy/taster2.0/blob/master/challenge_4.md "Challenge 4")
