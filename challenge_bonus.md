Challenge Bonus - Bootstrap & jQuery !
================

### Section 1 : Du responsive avec bootstrap ! (20 min)

Vous savez maintenant ce qu'est une librairie et un framework! Nous allons désormais utiliser les deux !

Pour ce faire:

1. Il faudra faire le lien avec les fichiers souhaitez. Il existe deux façons de faire:
  - Faire appel aux fichiers à partir d'un CDN (Content Delivery Network), ce qui veut dire que les fichiers sont sur un serveur distant (pas le vôtre), et que vous lui demandez, à chaque chargement de page, de vous donner les infos.

>
- **Pros** Ca va plus vite, le chargement de ces fichiers n'est pas à la charge de votre serveur.
- **Cons** Ça peut être risqué si le CDN est down (tombe), ce qui veut dire qu'il ne sera pas actif et ne pourra pas vous communiquer les fichiers.

  - Faire appel aux fichiers à partir de votre serveur. Vous stockerez donc les fichiers dans votre site et ils seront donc toujours dispo.

> Si quelqu'un trouve la solution pour bénéficier du beurre, l’argent du beurre et du cul de la fermière, dites-le-nous! Il y en a une ;) !

2. Aujourd'hui, nous ferons appel au CDN, c'est la solution la plus simple pour être up and running rapidement.

3. Rappelez-vous du cours d'hier sur le pont à faire entre vos fichiers HTML et CSS/JS
  - Où fait-on le pont?
  - Vers quelle source ou href la balise pointera?

> Voici deux liens vers les deux CDN dont nous aurons besoin:

Bootstrap: https://maxcdn.bootstrapcdn.com/bootstrap/3.3.6/css/bootstrap.min.css
jQuery: https://code.jquery.com/jquery-2.2.3.min.js

Faites ce qu'il faut faire avec ;)

### Section 2 : BootStrap et son Grid magique! (25 min)

Maintenant que vous avez bien galéré avec vos colonnes au format tablette ou mobile on va voir comment bootstrap peut vous aider!

>Pour Rappel, Bootstrap vous propose des class (entre autres, mais nous n'utiliserons que ça ce week-end) qui changeront le comportement de vos blocks une fois mis en place.

Le grid bootstrap se présente comme suit:
![Grid bootstrap image](https://bootstrapbay.com/blog/wp-content/uploads/2014/09/bootstrap-grid-system.jpg)

Le colonnes sont donc très facilement malléables, et si vous souhaitez un comportement différent selon les terminaux, vous pouvez utiliser différentes colonnes:

![Pixel inspector image](https://raw.githubusercontent.com/Coding-Days/coding-days/master/assets/images/Challenge%204/colonnes-bootstrap.png)


Pour effectuer un grid bootstrap sur votre site, il y aura plusieurs conditions :
1. Créer un container :
```html
<section class="container">

</section>
```
2. Créer une row qui aura pour but de créer un groupe horizontal de colonnes et mettre des margin des deux côtés.
```html
<section class="container">
  <div class="row">

  </div>
</section>
```
3. Créer desormais vos colonnes:
```html
<section class="container">
  <div class="row">
    <article class="col-md-8">
      Mon contenu à gauche
    </article>
    <aside class="col-md-4">
      Mon contenu à droite
    </aside>
  </div>.;
</section>
```

Les colonnes vont donc s'agencer toutes seules :).

>Plus de doc [ici](https://getbootstrap.com/css/#grid "bootstrap")

### Section 3 : Un peu de jQuery maintenant! (25 min)

Afin que vous compreniez facilement comment le JS est utilisé, on utilisera la librairie jQuery qui vous permettra d'écrire du JS très simplement!

On ne va pas pousser trop loin mais essayer simplement de faire changer le comportement de la page du côté client.

Ce qu'on vous propose aujourd'hui c'est de changer les titres de couleur 10 secondes après que la page ait chargée!

On utilisera donc plusieurs fonctions :
- $( document ).ready(function() pour faire en sorte d'être sur que la page soit bien chargée avant d'exécuter notre code.
- setTimeout(function(){ votre code }, les milli secondes); Pour dire à la page d'attendre X secondes.
- $( "sélecteur(s)" ).css("declaration", "valeur"); Pour dire à un sélecteur de changer son style.

> On vous propose de changer la couleur des titres après 10 secondes, mais si vous avez des idées similaires, faites-vous plaisir !

Quelques liens utiles :
- https://learn.jquery.com/using-jquery-core/document-ready/
- http://www.sitepoint.com/jquery-settimeout-function-examples/
- http://api.jquery.com/css/

<details>
  <summary>La solution est là mais essayez de ne pas la regarder!</summary>
  <details>
    <summary>Je suis un tricheur et je l'assume... </summary>

```js
       jQuery( document ).ready(function() {
         setTimeout(function(){
           jQuery("h1, h2, h3, h4, h5, h6").css("color", "red");
           alert("Yataaa!!!");
           console.log("Yataaa!!!");
         }, 10000);
       });
```


  </details>
</details>
