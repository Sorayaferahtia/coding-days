CSS Pill
================

Si vous n'êtes pas tout à fait à l'aise avec le langage HTML, nous vous conseillons d'aller sur cette page:
- [:pill: html](https://github.com/Coding-Days/coding-days/blob/master/assets/pills/html.md "html")

CSS Syntaxe
================

Tout d'abord, il y aura plusieurs mots de vocabulaire à intégrer pour que l'on parle tous la même langue :)

Une **règle** est consituée d'un sélecteur et d'un bloc avec une ou plusieurs déclarations

Un **sélecteur** vous permettra de cibler un élément en particulier

Une **déclaration** est une combinaison d'une propriété et d'une valeur (elle finit toujours par un ";")

La **propriété** définira le comportement à modifier du sélecteur de votre déclaration (background-color, width, etc)

La **valeur** définit le comportement de la propriété (background-color: blue;, width: 500px;, etc)


![css syntax image](https://raw.githubusercontent.com/makersacademy/taster2.0/master/assets/images/CSS%20Challenge/css_syntax.png)

L'inspecteur d'éléments
================

Je vous laisse découvrir cet outil magique et indispensable!

![inspect element](https://raw.githubusercontent.com/makersacademy/taster2.0/master/assets/images/CSS%20Challenge/inspect_element.png)

**Sur la gauche:**
Le site web en développement

**Sur la droite :**
La partie supérieure:
C'est votre DOM, référez-vous à cette [pill :pill:](https://la-cascade.io/quest-ce-que-le-dom/ "css selectors") Si vous ne savez plus exactement ce que c'est où si vous voulez plus de précision.                                                                                
Un usage très pratique de cet inspecteur sera le fait de pouvoir trouver le code correspondant à un élément très rapidement! Lorsque vous passer votre souris au-dessus (on hover) le DOM, vous verrez les éléments sur le site changer de couleur.

La partie inférieure:
C'est votre boite à outils CSS ! Vous pouvez modifier votre site (à gauche) en temps réel et voir si votre code fonctionne comme vous le souhaitez!

Vous avez énormément d'outils puissants et indispensables dans l'inspecteur d'élément, amusez-vous, posez-nous des questions, nous serons ravis de vous expliquer comment tout marche !

Introduction et principe d'héritage
================

CSS est l'acronyme de Cascading Style Sheets, feuilles de style en cascade.
L'appellation "cascade" est expliquée par le fait que:
1. Si une règle modifie un élément.
2. Si une deuxième règle modifie un deuxième élément en dessous la première.
3. Ce sera la deuxième règle qui fera effet.

Un petit exemple:

```css

h1 {
  color: blue;
}

h1 {
  color: red;
}

```

La couleur du h1 (titre important) sera donc... ROUGE!

Un autre exemple :

```css

div > h1 {
  color: blue;
}

h1 {
  color: red;
}

```

La couleur du h1 (titre important) sera donc... BLEU!

WTF?

Qu'est ce qu'il s'est passé !? Le sélecteur " > " permet de cibler l'élément descendant. On sélectionnera donc les titres en dessous d'une div.
Exemple:
```html
<div>
  <h1>Mon titre</h1>
</div>
```

La couleur du titre est bleue car la règle est plus précise!
Plus une règle est précise, plus elle aura de l'importance face aux autres.

>**Rappel :** Si vous souhaitez mettre des règles de priorités dans votre code, vous pouvez :                                                
1) Mettre un élément en dessous un autre                                                                                
2) Cibler plus précisément votre élément (bloc) avec un sélecteur, qui peut être une suite de balises, de class, d'ID, etc. Explorez tout ça dans l'inspecteur, vous apprendrez by doing :).


Nous avons donc introduit le principe d'héritage, nous allons désormais voir différents sélécteurs possibles.

CSS Selectors
================

Nous venons d'introduire le sélécteur " > ". Vous pourrez trouver une liste de 30 sélécteurs
[ici](http://code.tutsplus.com/tutorials/the-30-css-selectors-you-must-memorize--net-16048 "css selectors").

Nous couvrirons les plus utilisés:

####Le sélecteur étoile " * ":

Celui-ci ciblera tous les éléments du DOM.

```css

* {
  margin: 0;
}

```

Sauf si... une règle plus précise impacte un ou plusieurs éléments !

####Le sélecteur " balise ", ou " tag ":

Pour cibler une balise spécifique, vous pouvez mentionner cette ou ces balises comme suit:

```css

h1 {
  color: blue;
}

p {
  width: 700px;
}

```

Tous les titres seront bleus, et les paragraphes auront une longueur de 700px.

####Le sélecteur de class " . ":

Rappelez-vous, pendant le cours, nous avons vu ensemble comment faire le pont entre le HTML et le CSS.

Si vous avez ce code HTML:

```html

<p class="this_is_my_class_selector">
  Something
</p>
```

Vous pouvez désormais designer votre paragraphe (<p></p>) en ciblant sa classe comme suit:

```css

p.this_is_my_class_selector {
  width: 600px;
}

ou

.this_is_my_class_selector {
  width: 600px;
}

```

####Le sélecteur d'ID " # ":

Cela marche exactement comme le sélecteur de class:

```html

<p id="this_is_my_id_selector">
  Something
</p>
```

Vous pouvez désormais désigner votre paragraphe (<p></p>) en ciblant son ID comme suit:

```css

p#this_is_my_ID_selector {
  width: 600px;
}
```

or

```css
#his_is_my_ID_selector {
  width: 600px;
}

```
Mais alors, qu'elle est la différence entre une ID et une classe?

Une ID ne peut être utilisée qu'une seule fois.
Une classe peut être utilisée autant de fois que nécessaire!

Imaginez votre site,

Si vous souhaitez que tous vos titres soient en rouge et fassent 25px, vous pourrez utiliser une class que vous appliquerez à tous vos titres.

Seulement, pour une question de design, vous souhaitez qu'un titre soit différent, vous pourrez alors utiliser une ID.

####Le sélecteur chevron " > ":

Le chevron vous aidera à sélectionner l'élément descendant dans le DOM:

```css

div#container > ul {
  width: 600px;
}

```
Cette règle donnera une longueur de 600px à toutes les <ul></ul> (listes à puces) placées en dessous une div avec la class "container":


```html

<div id="container">
   <ul>
      <li> Item
        <ul> Second List
           <li> Item of the second list</li>
        </ul>
      </li>
      <li> Item </li>
      <li> Item </li>
      <li> Item </li>
   </ul>
</div>

```
La seconde liste à puces <ul></ul> ne sera donc pas affectée.

####Le sélecteur plus " + ":

Il ciblera seulement le premier élément après et pas à l'intérieur:

```css

div + p {
  width: 600px;
}

```
Seul le premier paragraphe après une div sera ciblé par cette règle.

####Le sélecteur virgule " , ":

Celui-ci vous aidera à définir les mêmes règles pour plusieurs éléments.

Par exemple si vous souhaitez que tous les input et les textarea de vos formulaires fassent la même taille, vous pouvez faire ceci:

```css

input, textarea {
  width: 600px;
}

```

####Combinez-les!

```css
div#form input.input, textarea, p > button {
  border: 6px solid red;
}
```
Cette règle va donner une bordure rouge de 6px à:

Les input, les textarea et les boutons à l’intérieur d'un paragraphe si tous ces sélecteurs sont à l'intérieur d'une div qui a une id "form".


Propriétés CSS
================

**background-color:** couleur de fond du block sélectionné;

```css
p.warning-notice {
  background-color: red;
}
```

**color:** couleur de la police d'écriture du block séléctionné;


```css
p {
  color: green;
}
```

**font:** Cette propriété possède plusieurs "sous" propriété;
On dit que c'est une super propriété.

```css
body {
  font-family: Arial, Helvetica, Sans-Serif; // in priority order
  font-size: 18px;
  font-style: italic;
  font-weight: bold;
}

ou

body {
  font: Arial, Helvetica, Sans-Serif, 18px, italic, bold;
}
```

**text-align:** Détermine comment un enfant est aligné horizontalement;
```css
#menu {
  text-align: right;
}
```


**border:** bordures du block ciblé;

```css
li.menu-item {
  border: 1px solid black;
}
```

**width and height:** dimension du block sélectionné;

```css
.photo {
  width: 200px;
  height: 100px;
}
```

Il existe bien plus de propriétés CSS![Vous pouvez les trouver ici](http://www.htmldog.com/reference/cssproperties/ "css proprieties"):

Le box model:
================

![css box model](https://raw.githubusercontent.com/makersacademy/taster2.0/master/assets/images/CSS%20Challenge/box_model.png)

Ceci va vous aider à placer vos éléments/block.

598x198 : C'est la longueur et largeur de votre élément (disons que c'est un paragraphe)
padding 16px: Votre paragraphe a 16px de padding tout autour de lui.
margin-top & margin-bottom 30px: Votre paragraphe aura 30px en haut et en bas de votre block.
margin-left & margin-right 40px: Votre paragraphe aura 40px à gauche et à droite de votre block.

![css box model](https://raw.githubusercontent.com/makersacademy/taster2.0/master/assets/images/CSS%20Challenge/boxmodelannot.png)

```css
div {
    width: 320px;
    padding: 10px;
    border: 5px solid gray;
    margin: 0;
}
```
Voici le calcul:
320px (width)
+ 20px (left + right padding)
+ 10px (left + right border)
+ 0px (left + right margin)
= 350px

Ou alors vous pouvez utiliser une simple déclaration:

```css
div {
    width: 350px;
    padding: 10px;
    border: 5px solid gray;
    margin: 0;
    -moz-box-sizing: border-box;
        box-sizing: border-box;
}
```
Voici le calcul:
350px (width)
+ 20px (left + right padding)
+ 10px (left + right border)
+ 0px (left + right margin)
= 350px

WTF?

La box-sizing: border-box; déclaration prend en compte les bordures, et le padding lorsque vous donner une valeur à la width.
Le block mesure désormais 350px. Lorsque vous développez un site en entier, comportant des milliers de lignes, ça sera beaucoup plus facile pour vous de manipuler ce type de block!

Le positionnement
================

Le positionnement est une des principales fonctions du CSS! Sans ça, notre page ne serait qu'une succession de block les uns après les autres.

>Un élément mis en display: block; prend par défaut la taille de la ligne en entier. Les autres éléments sont donc placés en dessous ou au-dessus de celui-ci.
Un élément placé en display:inline; laisse les autres éléments à gauche et/ou à droite de celui-ci.

Afin de positionner vos blocks vous pourrez donc attribuer plusieurs propriétés.

####Display

La différence entre **block** et **inline**:

Un ```<p>``` peut être un block, ils seront le plus souvent disposés les uns après les autres!

Un ```<a>``` va généralement être un élément inline à l'intérieur d'un autre block.

Vous avez aussi une propriété très utilisée, display: inline-block;

Ceci vous aidera à donner une width et height à votre élément.

display: none; est utiliseé pour cacher un élément (cette propriété est très utilisée en JavaScript).

####Position

position: relative; Cette propriété met le block en position relative. Elle aura pour but de placer l'élément en dessous le block relatif précédent.

position: absolute; Cette propriété fait flotter le block à l'intérieur du dernier block relatif parent.

position: fixed; Cette propriété fait flotter le block là où vous lui dites d'aller ! Si vous descendez sur la page, votre élément suivra !

[Vous pouvez essayer ce tutoriel rapide et très complet à ce sujet!](http://learnlayout.com/ "learn layout"):

Tips&Tricks:
================

####Commentaires

Un commentaire CSS peut être écrit de deux façons différentes:

Commentaire en ligne:

```css

.first_element + .second_element {
  font-size: 22px; //inline comment (maximum 1 line)
}

```
Commentaire en paragraphe:

```css
/*
I can write a comment in this line
this one as well
again ..
*/
.first_element + .second_element {
  font-size: 22px;
}

```

####Ne commencez jamais avec un chiffre:

```css

.1-first_element  {
  font-size: 22px;
}

```

Essayez autant que vous le voulez, ça ne marchera pas!

####Mais où je suis?

Si vous avez des problèmes à localiser et interpréter vos modifications, vous pouvez donner une bordure à votre block border: 1px solid;

C'est un peu meanless, mais ce tips vous sauvera énormément de temps au début!

####Un peu de logique?

```css

div.fluid_center  {
  width: 200px;
  margin-left: calc(50% - 100px);
}

```

Cette règle aura pour but de centrer l'élément .fluid_width au milieu de la page.
Le block sera à 50% du bord gauche, moins la moitié de sa taille, donc au milieu :).

####Le Cross-Browsing... On ne m'avait pas prévenu...

-webkit- pour Chrome                                                                                                    
-moz- pour Firefox                                                   
-o- pour Opera                                                   
-ms- pour IE                                                   

Par exemple, une transition sera écrite comme suit:

```css
.transition {
  -webkit-transition: all 1s ease;
     -moz-transition: all 1s ease;
      -ms-transition: all 1s ease;
       -o-transition: all 1s ease;
          transition: all 1s ease;
}
```
Cela permettra à tous les navigateurs de comprendre ce que l'on veut. En effet, tout ne tourne pas avec le même moteur et on leur propre façon d'interpréter vos demandes.
