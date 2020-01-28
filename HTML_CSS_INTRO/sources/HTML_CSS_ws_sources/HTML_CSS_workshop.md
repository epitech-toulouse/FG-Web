---
module:			HUB
title:			Challenges CSS / HTML
subtitle:		Créez votre portfolio en HTML et CSS !

language:		HTML, CSS
repository: 	HTML_INTRO
binary:         index.html

author:			Tifaine Larroque
version:		2.0
---

Si vous lisez ceci c'est que vous venez de finir le tutoriel HTML ou que vous avez estimé déjà avoir les connaissances nécéssaires en HTML !
Dans ce workshop nous allons vous proposer plusieurs exercices en HTML et en CSS qui viseront à réaliser un portfolio.

#hint(Pas d'inquiétudes, la partie CSS sera un peu plus guidée que la partie HTML car si vous êtes la c'est que vous ne connaissez pas le CSS...)

#newpage

# Introduction

Le CSS est un langage permettant d'ajouter du style à du code HTML basique. Afin d'organiser les propriétés que l'on veut appliquer à différents éléments un fichier CSS est composé de classes. Celles-ci sont ensuite appliquées en ajoutant la propriété *class="nom_de_la_classe"* dans la balise visée.
Certaines classes comme *body* existent déjà et sont liées aux balises du même nom.

#hint(Vous trouverez dans les ressources du workshop un fichier CSS contenant quelques classes de base afin de vous aider à démarrer !)

# Exercice 0

Pour commencer, créez un fichier **index.html** qui vous servira de base et téléchargez le fichier **my_portfolio.css** qui contiendra le style de votre page.
Afin d'intégrer le CSS dans votre HTML il faudra importer le fichier **my_portfolio.css** dans **index.html**. Voici comment faire : #br

#imageCenterCorners(img1.png, 400px, 0)

#hint(La propriété *rel* permet de signaler que le fichier à importer sera une balise de style, la propriété *type* indique que cela sera du code CSS et la propriété *href* permet de renseigner le path du fichier à importer. **A vous de trouver où écrire cette ligne !**)

#newpage 

# Exercice 1

Maintenant que vos fichiers sont créés voici quelques éléments de base à ajouter à votre page :

* Un titre qui s'affichera dans l'onglet du navigateur.
* Un logo (de votre choix) qui sera affiché tout en haut de la page
* Un titre qui sera la titre principal de votre page, en dessous du logo. Par exemple **Portfolio de...**

#hint(Si vous ne savez pas comment réaliser ces tâches jetez un coup d'oeil au tuto HTML que vous avez fait précédement.)

# Exercice 2

Maintenant que vous avez un logo et un titre il faut avouer qu'avoir tout ça sur la gauche de votre page n'est pas très joli... Créez deux classes CSS :

* **center-text** qui permettra de centrer le texte sur la page.
* **center-img** qui permettra de centrer l'image sur la page.

Vous pourrez ensuite appliquer ces classes à leurs balises respectives.#br

**Bonus :** Il se peut que votre image soit trop grande et prenne une trop grande partie de votre page, à vous de créer une classe supplémentaire pour que sa taille soit correcte !

#hint(Si vous ne savez pas comment faire n'hésitez pas à vous inspirer des classes déjà présentes dans le fichier qui vous à été fourni.)

# Exercice 3

Pour le moment lorsque l'utilisateur arrive sur votre page il n'a qu'un titre et un logo. Il faudrait rajouter une description qui sera encadrée afin d'attirer son oeil dessus !
Votre classe devra faire 2 actions : 

* Encadrer votre texte.
* Centrer le cadre autour du texte afin qu'il ne prenne pas la totalité de l'écran.

#hint(Il existe plusieurs types d'encadrement, à vous de chercher et de décider ce que vous souhaitez mettre !)

# Exercice 4

Maintenant que votre page comporte un logo, un titre et une description il va falloir y ajouter un peu de contenu ! Un portfolio doit contenir les réalisations que vous souhaitez exposer. Vous allez donc ajouter un sous-titre **Mes projets** en gras et souligné.
En dessous vous rajouterez au moins 2 projets sous forme de liste qui devront avoir un titre de rang "inférieur" à **Mes projets**.
Dans chaque projet affichez :

* Un petit paragraphe de description du projet. 
* Une image correspondant à votre projet. (Que vous remettrez à la bonne taille si necessaire)

#newpage

# Exercice 5

Maintenant qu'il y a un peu de contenu dans votre page, vous avez peut-être remarqué que la police n'est pas très jolie.

* Trouvez une police qui vous plait sur *Google Fonts* et importez la dans votre fichier HTML.
* Faites en sorte que la police s'applique à toiut le corps de votre page grâce à une classe CSS.

#hint(Pour que la police s'applique à toute votre page regardez bien les classes qui sont déjà dans le fichier qui vous est fourni !)

# Exercice 6

Pour le moment vous affichez quelques informations sur vos projets mais pour un recruteur ce n'est pas très interessant. Il va falloir donner la possiblité à l'utilisateur d'avoir accès aux sources ou au rendu final de votre projet !
Vous allez donc ajouter 2 moyens de faire ceci :

* D'abord en cliquant sur l'image. Ajoutez donc un message indiquant à l'utilisateur qu'en cliquant sur votre image il aura accès à votre projet. Puis faites en sorte que le click sur l'image renvoie l'utilisateur sur votre projet.
* Ensuite en ajoutant un lien **Github du projet** ou **Nom du site web** en dessous de l'image. Vous ajouterez une classe CSS qui change la couleur du lien et qui enlève le soulignement.

#hint(Pour le moment si vous cliquez sur l'un de vos liens cela quittera votre page actuelle. Il existe un propriété CSS qui permet d'ouvrir un lien dans un nouvel onglet.)

# Exercice 7

Maintenant que votre page commence à prendre forme il serait mieux de modifier la taille des titres afin de les mettre plus ou moins en avant.
Modifiez la taille de la police de h1, h2 et h3 selon ce que vous souhaitez mettre plus ou moins en avant sur votre page !

#hint(Si vous ne savez pas comment faire basez vous sur ce qui est sur le fichier fourni !)

#hint(En plus de la taille de chaque balise vous pouvez aussi changer les couleurs !)

# Exercice 8

Votre page commence à ressembler à quelque chose mais il manque un élément important ! Il faut renseigner vos compétences ainsi que votre niveau dans chacune d'entre elles.
Premièrement créez un sous-titre **Mes compétences** que vous espacerez un petit peu du contenu qui est au dessus (une propriété CSS permet de faire ça !).
Ensuite votre tableau devra contenir :

* Une entête **Compétence** et une entête **Niveau**. La police devra être plus grande que la police du reste du tableau.
* Les compétences de votre choix ainsi que votre niveau dans celle-ci.
* Des bordures qui encadreront tout le tableau mais ne prendront pas toute la longeur de la page.

Voici un exemple de tableau sur lequel vous pouvez vous baser : #br

#imageCenterCorners(img2.png, 450px, 0)

# Exercice 9 

Pour finir nous allons séparer votre site en sections afin de changer le background de celui-ci.
Une nouvelle balise entre en jeu ici : *div*. Cette balise sert à englober plusieurs balises afin de construire des sections et diviser la page en plusieurs parties. Une classe appliquée à une div sera appliquée à toutes ses balises enfant.
Vous allez donc séparer votre site en 3 parties :

* Un header qui contiendra le logo et le titre de votre page (eventuellement la description, c'est à vous de choisir).
* Le corps du site, que vous pourrez séparer en sous parties selon les sections.
* Le footer du site, que vous allez créer en écrivant quelques informations sur vous ou même en donnant des liens vers vos réseaux sociaux.

#hint(A vous de gérer les couleurs et tailles de chaque élément, bonne chance !)

# Pour aller plus loin

Si vous avez déjà fini le workshop et qu'il reste du temp n'hésitez pas à nous poser des questions ou à nous demander d'autres challenges à réaliser sur ce petit projet !

#hint(Le rendu que vous avez eu aujourd'hui n'était peut-être pas très esthétique mais lors d'un prochain Workshop nous vous montrerons comment faire des sites plus beaux !)
