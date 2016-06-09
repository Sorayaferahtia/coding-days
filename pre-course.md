Pre course
================

Pendant le weekend, vous allez travailler sur un projet personnel (votre portfolio par exemple), veillez donc à préparer en amont photos et wording.
Allez jeter un coup d'oeil sur [Unsplash](https://unsplash.com/ "Unsplash"), il y a de jolies photos.
Et sur [Lorem Ipsum](http://fr.lipsum.com/ "Lorem Ipsum"), si vous n'avez pas d'idée pour le wording, c'est un générateur de faux texte.

Essayer de dessiner votre "Mock up" sur papier, ça devrait ressembler à quelque choses comme ça (en plus simple):

![mockup image](https://raw.githubusercontent.com/makersacademy/taster2.0/master/assets/images/HTML%20Challenge/mockup%20example.gif)

Liste des logiciels que nous allons utiliser.

- Git - Outil de collaboration et de versionning
- Github - Représentation visuelle de l'outil de Git (Une interface moins brute)
- Ruby - Notre langage de programmation
- Heroku (toolbelt) - Application d'hébergement sur le Cloud, pour mettre en ligne, les fichiers que nous allons créer.
- Un éditeur de texte [Atom](https://atom.io/ "Atom.io") pour Mac et [NotePad ++](https://notepad-plus-plus.org/fr/ "NotePad ++") pour Windows

Ceci est une liste non-exaustive de ce dont vous aurez besoin pour développer, mais cela suffit amplement pour le Week End Coding-Days.

Quelques vidéos à regarder avant de continuer :
- [Learning GIT](https://www.youtube.com/watch?v=_Jmkvv_nKTE "Learning GIT")
- [What is the difference between Git and GitHub? ](https://www.youtube.com/watch?v=xKVlZ3wFVKA "What is the difference between Git and GitHub? ")
- [What Is Github ](https://www.youtube.com/watch?v=VUaBfYCmJls "What Is Github ")

- [http://stackoverflow.com/questions/11008787/what-exactly-is-heroku](http://stackoverflow.com/questions/11008787/what-exactly-is-heroku "http://stackoverflow.com/questions/11008787/what-exactly-is-heroku")

###Utilisateurs Mac & Windows
1- Créer un compte sur [Github](https://github.com/join "Github")                                            
2- Créer un compte sur [Heroku](https://signup.heroku.com/ "Heroku")



####Sur MAC                                                
1 - Suivez les étapes d'installation sur: [Prepare to code](http://www.preparetocode.io/mac/essential/ "prepare to code") (Un site preparé avec &#9829;)                                       
2 - Une fois que tout est installé, redémarrez votre ordinateur                                                           
3 - Ouvrez votre terminal et tapez les commandes suivantes           


>Si vous cherchez votre teminal: Ouvrez la barre de recherche MAC Spotlight, et recherchez "Terminal.app".
Ou encore allez dans votre dossier /Applications puis /Utilitaires et choississez Terminal.app
![terminal image](https://raw.githubusercontent.com/Coding-Days/coding-days/master/assets/images/Pre%20Course/Terminal.png)

>Le signe " $ " est une indication pour définir une ligne à taper. Vous ne devez donc pas l'écrire. Les autres lignes sont les réponses de votre invité de commande
>Notez que lorsque vous écrirez votre mot de passe, rien ne s'affichera, cela pour des raisons de sécurité (longueur du mot de passe cachée).

```
bash
$ heroku login
Enter your Heroku credentials.
Email: me@example.com
Password:

$ cd && cat .netrc
machine api.heroku.com
  login me@example.com
  password c4cd94da15ea0544802c2cfd5ec4ead324327430
machine git.heroku.com
  login me@example.com
  password c4cd94da15ea0544802c2cfd5ec4ead324327430
```

[Suivez désormais ce lien pour parametrer Git:](https://help.github.com/articles/set-up-git/ "Set up Git")

**C'est bon! Vous êtes prêt pour le weekend!**


###Utilisateurs Windows
1 - Téléchargez et installez Ruby [Ruby](http://rubyinstaller.org/downloads/ "Ruby")
![Étape 1 installation](https://raw.githubusercontent.com/Coding-Days/coding-days/master/assets/images/Pre%20Course/ruby//1.jpg)
![Étape 2 installation](https://raw.githubusercontent.com/Coding-Days/coding-days/master/assets/images/Pre%20Course/ruby//2.jpg)
![Étape 3 installation](https://raw.githubusercontent.com/Coding-Days/coding-days/master/assets/images/Pre%20Course/ruby//3.jpg)
![Étape 4 installation](https://raw.githubusercontent.com/Coding-Days/coding-days/master/assets/images/Pre%20Course/ruby//4.jpg)
![Étape 5 installation](https://raw.githubusercontent.com/Coding-Days/coding-days/master/assets/images/Pre%20Course/ruby//5.jpg)
![Étape 6 installation](https://raw.githubusercontent.com/Coding-Days/coding-days/master/assets/images/Pre%20Course/ruby//6.jpg)
![Étape 7 installation](https://raw.githubusercontent.com/Coding-Days/coding-days/master/assets/images/Pre%20Course/ruby//7.jpg)
![Étape 8 installation](https://raw.githubusercontent.com/Coding-Days/coding-days/master/assets/images/Pre%20Course/ruby//8.jpg)

2 - Téléchargez et installez Git [Git pour Windows](https://git-for-windows.github.io/ "Git pour Windows")
![Étape 1 installation](https://raw.githubusercontent.com/Coding-Days/coding-days/master/assets/images/Pre%20Course/git//1.jpg)
![Étape 2 installation](https://raw.githubusercontent.com/Coding-Days/coding-days/master/assets/images/Pre%20Course/git//2.jpg)
![Étape 3 installation](https://raw.githubusercontent.com/Coding-Days/coding-days/master/assets/images/Pre%20Course/git//3.jpg)
![Étape 4 installation](https://raw.githubusercontent.com/Coding-Days/coding-days/master/assets/images/Pre%20Course/git//4.jpg)
![Étape 5 installation](https://raw.githubusercontent.com/Coding-Days/coding-days/master/assets/images/Pre%20Course/git//5.jpg)
![Étape 6 installation](https://raw.githubusercontent.com/Coding-Days/coding-days/master/assets/images/Pre%20Course/git//6.jpg)
![Étape 7 installation](https://raw.githubusercontent.com/Coding-Days/coding-days/master/assets/images/Pre%20Course/git//7.jpg)
![Étape 8 installation](https://raw.githubusercontent.com/Coding-Days/coding-days/master/assets/images/Pre%20Course/git//8.jpg)
![Étape 9 installation](https://raw.githubusercontent.com/Coding-Days/coding-days/master/assets/images/Pre%20Course/git//9.jpg)
![Étape 10 installation](https://raw.githubusercontent.com/Coding-Days/coding-days/master/assets/images/Pre%20Course/git//10.jpg)

2 - Téléchargez et installez Heroku Toolbet [Heroku pour Windows](https://toolbelt.heroku.com/windows "Heroku pour Windows")
![Étape 1 installation](https://raw.githubusercontent.com/Coding-Days/coding-days/master/assets/images/Pre%20Course/heroku//1.jpg)
![Étape 2 installation](https://raw.githubusercontent.com/Coding-Days/coding-days/master/assets/images/Pre%20Course/heroku//2.jpg)
![Étape 3 installation](https://raw.githubusercontent.com/Coding-Days/coding-days/master/assets/images/Pre%20Course/heroku//3.jpg)
![Étape 4 installation](https://raw.githubusercontent.com/Coding-Days/coding-days/master/assets/images/Pre%20Course/heroku//4.jpg)
![Étape 5 installation](https://raw.githubusercontent.com/Coding-Days/coding-days/master/assets/images/Pre%20Course/heroku//5.jpg)
![Étape 6 installation](https://raw.githubusercontent.com/Coding-Days/coding-days/master/assets/images/Pre%20Course/heroku//6.jpg)
![Étape 7 installation](https://raw.githubusercontent.com/Coding-Days/coding-days/master/assets/images/Pre%20Course/heroku//7.jpg)
![Étape 8 installation](https://raw.githubusercontent.com/Coding-Days/coding-days/master/assets/images/Pre%20Course/heroku//8.jpg)

3 - Ouvrez maintenant l'invité de commande (c'est la console windows et tapez les commandes suivantes)
>Pour ouvrir l'invité de commande, ouvrez le menu démarrer, aller dans rechercher, et tapez cmd.exe.
>L'invité de commande devrait apparaître.


```bash
$ heroku login
Enter your Heroku credentials.
Email: me@example.com
Password:
```

>Le signe " $ " est une indication pour définir une ligne à taper. Vous ne devez donc pas l'écrire. Les autres lignes sont les réponses de votre invité de commande
>Notez que lorsque vous écrirez votre mot de passe, rien ne s'affichera, cela pour des raisons de sécurité (longueur du mot de passe cachée).
