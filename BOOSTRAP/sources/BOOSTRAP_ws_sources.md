---
module:			HUB
title:			Tutoriel Bootstrap
subtitle:		Les bases de Bootsrap

language:		HTML / CSS
repository: 	BOOTSTRAP_WS
binary:         index.html

author:			Tifaine Larroque
version:		1.0
---

Dans le dernier workshop vous avez appris à utliser les bases du HTML et du CSS qui sont indispensables au développement web. Cependant comme vous avez pu  le remarquer, il est difficile d'avoir un rendu esthétique de façon simple et rapide.
C'est ici que Bootsrap entre en jeu ! C'est un framework proposant des composants simples à intégrer et à prendre en main ainsi qu'un système de grilles permettant de découper vos pages web en sections. Tout ses composants sont aussi adaptés à un design responsive ce qui, une fois de plus, peut vous faire gagner beaucoup de temps !

#newpage

# Introduction

Dans ce workshop nous allons créer de A à Z un site CV qui vous permettra de rassembler vos compétences et expériences professionnelles. Nous allons vous guider dans cette réalisation mais il faudra aussi lire de la documentation par vous même afin d'avoir tout les éléments nécéssaires !
Voici un lien vers la documentation de Bootstrap : #br
https://getbootstrap.com/docs/4.1/getting-started/introduction/ #br
Avant de commencer quoi que ce soit il faut comprendre le système de *grid* que Bootstrap met en place. Chaque section de votre site devra être entouré par une balise *div* ayant pour classe CSS *container-fluid*. Cette classe permet d'indiquer que la section doit prendre toute la longueur de la page. 
Ce découpage en *grid* va permettre d'associer des classes et styles différents à chaque sections de votre site et donc de ne plus tout avoir en un seul bloc.

#hint(Ce concept est très important, si durant le workshop cela ne vous semble pas clair n'hésitez pas à demander de l'aide !)

#warn(Si vous cherchez de la documentation par vous même, faites attention à bien lire la documentation de Bootstrap 4 et non 3 !)

# Pour commencer

Pour ce workshop nous vous avons fourni un fichier de base **index.html**, c'est dans celui-ci que se trouvera la majorité de votre code. Il contient déjà les meta nécéssaires et Bootstrap est déjà importé dans le fichier. Ouvrez ce fichier dans votre naviguateur.
Voici quelques tâches basiques afin de vous remémorer le workshop précédent :

* Donnez un titre à votre page (qui doit être affiché dans l'onglet du navigateur).
* Changez la police de votre page web.
* Ajoutez un logo de votre choix dans l'onglet du naviguateur qui contient déjà votre titre.

#hint(L'icone située dans l'onglet du naviguateur s'appelle un *favicon* à vous de trouver comment l'intégrer.)

# La navbar de votre page web

Une navbar est un élément situé en haut de votre page et qui permettra à l'utilisateur de naviguer sur votre site. Ici cela permettra de naviguer uniquement entre les sections d'une même page.
Pour commencer créez votre navbar, elle devra avoir plusieurs attributs : 

* Un thème sombre ou clair, à vous de choisir.
* Votre logo tout à gauche de la navbar.
* Une liste des sections qui seront présents sur votre site : *Qui suis-je ?*, *Compétences*, *Experiences professionnelles*, *Contact*.
* Elle devra rester collée en haut de la page même lorsque l'utilisateur scrollera vers le bas.

#hint(Veillez à garder votre code le plus simple possible, Bootstrap propose souvent plusieurs syntaxes qui amènent au même résultat. Trouvez celle qui rendra votre code le plus lisible !)

# La creation des sections

Comme nous en avons parlé plus haut, Bootstrap permet de facilement diviser votre page web en plusieurs sections. Celles-ci devront avoir quelques propriétés de base :

* Laisser une marge de chaque côté de la page. (Afin que votre contenu ne soit pas collés au bord de l'écran)
* Un grand titre centré au milieu de la page (*Qui suis-je ?*, *s*, *Experiences professionnelles*).
* Une séparation avec la section suivante.

La section *Contact* sera un peu différente des autres, cela doit être un *footer* et non une section classique. Il vous faut donc utiliser une balise *footer* et non *div*. Il devra avoir le même thème que la navbar et être collé au bas de votre page web.

#hint(Si vous n'arrivez pas à fixer votre footer en bas de la page ne vous inquiétez pas, vous pourrez régler ça une fois que vos sections seront complètes.)

# La section *Qui suis-je ?*

Maintenant que vous avez le squelette de votre site il faut créer du contenu ! Votre section devra être divisé en deux colonnes : l'une contenant une photo de vous et une autre une courte description qui permettra de vous présenter. C'est donc ici qu'intervient le système de *grid*. Pour vous aider à vous lancer voici un morceau de code duquel vous pourrez commencer : #br

#imageCenterCorners(img1.png, 300px, 0)

La div ayant pour classe *row* indique que ce qui suivra sera un enchainement de colonnes à afficher dans la page. Les div suivantes détérmineront le nombre de colonnes que vous voulez. Afin de déterminer la largeur de chaque colonne il y a la classe *col-x*. La largeur de la page étant divisée en 12, si la classe est *col-6* cela signifie que la colonne prendra la moitié de la largeur de la page.

# La section *Competences*

Dans cette section vous allez présenter vos compétences. Ici, pas besoin de grilles car nous allons présenter vos compétences sous forme de tableau ! Voici les critères du tableau que vous allez créer : 

* Il doit contenir deux colonnes : *Compétence*, *Niveau* et *Réalisations*.
* Au moins trois lignes contenant vos compétences ainsi que le niveau que vous avez dans celles-ci. Pour la colonne *Réalisations* écrivez une description rapide de vos experiences dans cette compétences.
* Le tableau doit avoir une colonne sur deux d'une couleur différente (petit indice : *striped*).
* Le tableau doit être centré sur la page.

#hint(Si vous avez d'autres idées de colonnes pour votre tableau n'hésitez pas à les rajouter !)

# La section *Experiences professionnelles*

Dans cette section vous allez lister les expériences professionnelles que vous avez eu. C'est donc le retour du système de grilles, mais aussi l'introduction d'un nouvel élément. Pour commencer créez le nombre de colonnes que vous voulez qui prendront le tiers de la page chacune.
Ensuite nous allons ajouter des *cartes*. Voici les critères de celles-ci :

* Une image *header* qui contiendra le logo de l'entreprise, si vous n'avez pas d'image n'en mettez pas.
* Un titre qui décrira en quelques mots votre expérience.
* Un corps qui décrira plus en détails votre expérience.

#hint(Si vous avez peu d'experiences n'hésitez pas à en inventer pour le workshop. Si vous en mettez plus de 3 alors que celles-ci sont censées prendre un tiers de la largeur de la page, ne vous inquiétez pas Bootstrap mettra tout en place correctement !)

# La section *Contact*

Cette section sera plutôt simple car elle ne doit pas contenir trop d'informations. C'est pour cela que nous allons principalement utiliser des icônes ! Pour cela allez sur le site de **Font Awesome**, c'est une banque d'icônes gratuits et simples à intégrer dans du code HTML. Voici les critères de ce footer :

* Il doit être divisé en 3 colonnes.
* La première colonne doit contenir les logos des réseaux sociaux que vous souhaitez partager avec l'utilisateur (Linkedin, Twitter, Facebook...) ainsi qu'un lien lié à chaque icône redirigeant vers le réseau social en question.
* La 2ème colonne doit contenir un icône email ainsi que votre adresse email.
* La 3ème colonne doit contenir un icône téléphone ainsi que votre numéro de téléphone.

# La navbar... partie 2

Comme vous avez dû le remarquer, pour le moment votre navbar ne sert pas à grand chose à part énoncer les sections qui seront présentes sur votre site. Il faut maintenant lier chaque élément de votre navbar à la section correspondante. Pour ce faire il y aura deux étapes :

* Attribuer une propriété id à chaque section.
* Attribuer un *href=#X* à chaque éléments de la navbar.

Une fois que vous aurez fait ceci, un clic sur la navbar devrait rediriger la page sur la section séléctionnée !

# Bonus

Pour le moment vous avez vu certains composants basiques de Bootstrap ! S'il vous reste encore un peu de temps pour ce workshop voici quelques bonus que vous pouvez réaliser :

* Rajouter un bouton *Me contacter* à la suite de votre description personnelle qui redirigera sur votre footer.
* Indiquer sur quelle section est actuellement l'utlisateur dans la navbar (scrollspy).
* Un carousel qui pourrait servir à présenter certaines de vos réalisations de façon plus visuelle.

#hint(N'hésitez pas à rajouter vos propres bonus et à nous demander de l'aide si vous ne savez pas comment faire quelque chose qui vous interesse !)

