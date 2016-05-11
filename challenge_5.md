Challenge 5 - Make it live!
================

###Section 1 -  Le framework ruby Sinatra! (30min)

Nous vous avons preparé le framework pour qu'il soit déjà fonctionnel!

Nous allons donc "Forker" le projet pour que vous puissiez le modifier à votre guise!

1. Aller sur la page
[GitHub project page](https://github.com/Coding-Days/sinatra-app "Sinatra app")

2. Cliquez sur "Fork"                                                 
![fork](https://raw.githubusercontent.com/makersacademy/taster2.0/master/assets/images/CSS%20Challenge/fork.png)

3. Attendez pendant le transfert                                                
![waiting process](https://raw.githubusercontent.com/makersacademy/taster2.0/master/assets/images/CSS%20Challenge/wait.png)

4. Vous pouvez maintenant le voir sur votre compte perso!                                                 
![forked repo](https://raw.githubusercontent.com/makersacademy/taster2.0/master/assets/images/CSS%20Challenge/forked.jpg)

Le projet est donc désormais sur votre compte Github, mais pas encore sur votre ordinateur! Il va falloir cloner le projet pour ça!

1.
```bash

git clone https://github.com/VOTRE-NOM/sinatra-app.git
cd sinatra-app
atom . #SUR MAC
XXXX . #SUR PC

```
Attention, lorsque vous cloner le projet, il va créer un repo avec son nom directement, donc mettez le aà la racine du dossier souhaité.

> cd signifie "change directory" c'est donc la commande pour vous balader sur votre ordinateur depuis votre terminal

>atom . dit à votre IDE (ici atom), d'ouvrir tous les fichiers enfants de là où vous êtes.

2. Nous nous interesserons seulement à deux fichiers:                                                 
  - Index.erb
  - Style.css

**Vous les trouverez dans: app > views > index.erb && public > css > style.css**

Baladez vous un peu dans le framework, explorez et posez-nous des questions si vous en avez!


3. Pour voir votre site à travers un serveur (comme le fera Heroku), vous devez lancer votre serveur local.

Toujours aà la racine de votre repo, lancer le serveur avec la commande suivante:

```bash
heroku local
```

Aller à l'adresse suivante dans votre navigateur: http://localhost:5000

Si ça marche aller à l'étape 4!

4. Copier le contenu des fichiers:
  - index.html dans index.erb du framework
  - style.css dans style.css du framework

Recharger la page http://localhost:5000 et assurez-vous que tout est pareil que ce matin.

Si vous êtes satisfait, next step!


>Rappellez vous, si vous êtes agile, vous mettez votre code en ligne **souvent** et **tôt**. Faite le donc apres chaque feature.

5. Vous avez donc votre site visible grace au serveur local d'Heroku, maintenant, mettons le en ligne pour de vrai!!

```bash
heroku create le-nom-de-votre-projet
git add .
git commit -m "adds my first feature"
git push origin master
git push heroku master
heroku open
```

Ça dit quoi? ;)

###Section 3 -  Créer une nouvelle page pour votre site !

1. Créez une seconde page dans le dossier /views et nommé le comme vous voulez (l'extension doit être en .erb).                                               
2. Ouvrez le fichier index.rb dans /controllers et faite une requête GET pour la nouvelle page que vous venez de créer.

```ruby
get '/my-second-page' do
  erb :my-second-page
end
```

3. Vous pouvez désormais developper dans  ma-seconde-page.erb et vous verrez les changements sur:                        
  - http://localhost:5000/ma-seconde-page.erb (pour voir les changement en local)
  - http://mon-application.herokuapp.com/ma-seconde-page.erb  (après avoir push to heroku)

4. Vous pouvez maintenant lier les deux pages dans votre menu :)                                                       

Si vous avez fini, amusez-vous à peaufiner votre appli, vous êtes arrivé à la fin :)

VOUS ALLEZ NOUS MANQUER !!!
