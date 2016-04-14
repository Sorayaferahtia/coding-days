Pre course
================

Avant d'écrire sa première ligne de code, il vous faudra installer pas mal de petits logiciel!

Petit apercu du menu, vous devrez installer:

- Git - Outil de collaboration et de versionning
- Github - Représentation visuelle de l'outil de git
- Ruby - Notre langage de predilection
- Heroku - L'entreprise qui hébergera votre application à la fin du Week End.
- Un éditeur de texte [Atom](https://atom.io/ "Atom.io") pour MAC et [NotePad ++](https://notepad-plus-plus.org/fr/ "NotePad ++") pour WINDOWS

Ceci est une liste non-exaustive de ce dont vous aurez besoin pour développer, mais cela suffit amplement pour le Week End Coding Days!

> Si vous cherchez votre teminal: Ouvrez la barre de recherche MAC Spotlight, et recherchez "Terminal.app".
Ou encore allez dans votre dossier /Applications puis /Utilitaires et choississez Terminal.app

![terminal image](http://apple.blogovlow.com/files/2012/02/Terminal.png)


####Sur MAC
1- Créer un compte sur [Github](https://github.com/join "Github")                                            
2- Créer un compte sur [Heroku](https://signup.heroku.com/ "Heroku")                                                   
3- Suivez les étapes d'installation sur: [Prepare to code](http://preparetocode.io "prepare to code")
  - Site que nous vous avons preparé avec &#9829;                                       
4- Une fois que tout est installé, redémarrez votre ordinateur                                                           
5- Ouvrez de nouveau votre terminal et tapez les commandes suivantes                                                                                                                                     
>Si vous cherchez votre teminal: Ouvrez la barre de recherche MAC Spotlight, et recherchez "Terminal.app".
Ou encore allez dans votre dossier /Applications puis /Utilitaires et choississez Terminal.app

>Le signe " $ " est une indication pour définir une ligne à taper. Vous ne devez donc pas le taper, c'est simplement une indication pour vous. Les autres lignes sont les réponses de votre terminal.

>Lorsque vous tapez votre mot de passe dans le Terminal rien ne se passe et c'est normal. tapez le quand meme et faites entré.

1. Lier votre compte Heroku "à votre ordinateur"
```bash
$ heroku login
Enter your Heroku credentials.
Email: me@example.com
Password:
```
Maintenant on verifie qu'on est bien connecté
```bash

$ cd && cat .netrc
machine api.heroku.com
  login me@example.com
  password c4cd94da15ea0544802c2cfd5ec4ead324327430
machine git.heroku.com
  login me@example.com
  password c4cd94da15ea0544802c2cfd5ec4ead324327430
```
2. Lier votre compte GitHUb "à votre ordinateur"
```bash
$ git config --global user.name "VOTRE USERNAME SUR GITHUB"

$ git config --global user.email "VOTRE ADRESSE MAIL DU COMPTE GITHUB"
$
```
Maintenant on verifie qu'on est bien connecté
```bash
```


[Suivez desormais ce lien pour parametrer Git:](https://help.github.com/articles/set-up-git/ "set up git")


**C'est bon! Vous êtes prêt pour le weekend!**
