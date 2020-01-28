---
module:			HUB
title:			Tutoriel HTML
subtitle:		Les bases du HTML

language:		HTML
repository: 	HTML_INTRO
binary:         index.html

author:			Tifaine Larroque
version:		2.1
---

# Introduction 

Dans ce tutoriel nous allons vous apprendre pas à pas toutes les bases du HTML qui vous permettront par la suite de vous pencher sur d'autre langages ou frameworks plus poussés.#br

#hint(Aujourd'hui, le HTML est indispensable à la création du front-end d'un site web. Tout les langages et frameworks front-end nécéssitent l'utilisation du HTML. Donc si vous voulez faire du web, l'apprentissage du HTML est une étape indispensable !)

#newpage

# Pour commencer

Pour commencer créez un dossier nommé HTML_INTRO afin de rassembler tout les fichiers de votre site web. 
Ensuite, créez un fichier "index.html" qui contiendra tout le code de base de votre site.

# Les balises

Avant de commencer à coder il faut comprendre le principe de base du HTML : les balises. Celles-ci permettent de hiérarchiser et structurer le contenu de votre page web.#br
#imageCenterCorners(img1.png, 300px, 0)

* La balise *html* doit englober la totalité du code.
* La balise *head* permet de renseigner les informations de la page comme son titre ou les fichiers css à inclure cette partie est pour plus tard !
* La balise *body* rassemble tout le code qui composera la page web.#br

#hint(Chaque balise doit être refermée après avoir été ouverte !)

Afin d'avoir un premier aperçu de votre page web, ouvrez le fichier index.html dans votre naviguateur.

# Le titre de la page 

#hint(Le titre de la page est lisible dans l'onglet de celle-ci !)

Afin de définir le titre de la page il suffit d'utiliser une balise *title*. Dans les balises permettant d'afficher du texte celui-ci s'écrit directement entre la balise ouvrante et la balise fermante. A vous de trouver où placer cette balise !

# Organiser son code 

Un fichier HTML peut très vite devenir complexe et illisible lorsque beaucoup de balises s'embriquent les unes dans les autres. Il est donc très important de commenter son code, surtout en tant que débutant.
Un commentaire s'écrit de cette façon : 
#imageCenterCorners(img2.png, 300px, 0) 

# Ajouter un titre

En HTML il y a plusieurs types de titres. Ceux-cis sont définis par les balises *h1, h2, h3, h4*. Plus le chiffre de la balise est proche de 1 plus il sera "important" et donc dans une plus grosse police. Cela correspondrait par exemple à un titre, un sous-titre, un sous-sous-titre... #br
Vous pouvez donc ajouter un titre de votre choix à votre page web et essayer d'utiliser les balises *hX* comme bon vous semble ! Une fois de plus à vous de trouver où placer la balise!

# Ecrire du contenu

Maintenant que votre page à un titre (et peut-être un sous-titre !) il faut y ajouter un peu de contenu.
Il existe plusieurs balises pour écrire et mettre en forme du texte sur une page web.

* p qui permet d'écrire du texte simple.
* *b* qui permet d'écrire du texte en gras (*bold*).
* *i* qui permet d'écrire du texte en italique (*italic*).
* *br* qui permet d'afficher un saut de ligne. Cette balise est un peu particulière car elle n'a pas besoin d'être ouverte puis fermée. Cela s'appelle une balise "orpheline". Elle s'utilise comme ceci : *br/*.

#hint(Les balises *i* et *b* ont un comportement un peu différent de la balise *p*, à vous de faire quelques tests !)

#warn(Vous pourrez rencontrer ces balises sur des sites mais attention à bien différencier le fond comprenant le texte et l'agencement des balises HTML et la forme qui fait référence à la mise en page et le formatage du texte soit le CSS)

Vous pouvez donc rajouter un texte de votre choix sur votre page et tester l'utilisation des balises ! #br

Maintenant nous allons modifier la couleur du texte de la page. Nous allons cette fois-ci utiliser la balise *font*. Mais celle-ci doit être imbriquée dans une balise de texte basique afin de fonctionner. Voici un exemple : #br

#imageCenterCorners(img3.png, 400px, 0)

#hint(Dans la balise *font* la couleur peut être renseignée avec le code hexadécimal ou directement avec le nom de la couleur. Evidemment utiliser le code hexadécimal vous apportera plus de choix !)

#newpage

# Inserer des images

Afin d'insérer des images sur votre page il faut utiliser *img*, qui est une balise orpheline comme *br*.
Comme pour la balise *font* il faut rajouter des propriétés dans la balise pour afficher l'image que vous souhaitez.

* *src* qui devra contenir le path du fichier que vous souhaitez afficher.
* *alt*, un texte qui sera affiché si suite à un soucis l'image ne peut pas s'afficher.
* *title* qui sera affiché lorsque l'utilisateur passera sa souris sur l'image.
* *height* et *width* qui permettrons de définir la taille de l'image.

Voici un exemple : 

#imageCenterCorners(img4.png, 500px, 0)

#hint(Seule la propriété src est obligatoire afin d'afficher une image, les autres sont optionnelles.)

#hint(Spécifier la width et la height en px peut déformer l'image, pour garder la forme de base de l'image ces propriétés peuvent aussi être spécifiées en %.)

# Les liens 

Une page web n'est pas très utile si elle n'a aucun lien avec d'autres pages ! Que cela soit vers une autre page de votre site ou vers un site externe les liens sont très utiles. Il y a besoin de 2 éléments pour ajouter un lien :

* Une balise *a* qui permet d'insérer un lien et dans laquelle nous allons écrire le texte lié au lien.
* Une propriété *href* qui permet de spécifier vers où le lien doit rediriger l'utilisateur.

#hint(Ce n'est pas obligé de mettre du texte dans la balise *a*, cela peut par exemple être un image !)

# Les listes

Les listes sont un élément très utile et très simples à intégrer. Elles nécessitent 2 balises différentes qui vont venir s'imbriquer :

* *ul* (unordered list) qui déclare qu'une liste doit être affichée.
* *ol* (ordered list) est une liste numérotée.
* *li* qui définit chaque élément de la liste.

Voici un exemple: #br

#imageCenterCorners(img5.png, 400px, 0)

# Les tableaux

En HTML les tableaux ne sont pas très esthétiques mais à l'aide d'un peu de CSS ils sont bien plus lisibles ! Pour le moment nous allons juste voir comment construire le squelette du tableau à l'aide du HTML. Les tableaux peuvent paraître complexe car ils nécéssitent 4 balises différentes :
* *table* qui déclare qu'un tableau doit être affiché.
* *tr* qui permet de déclarer une ligne du tableau. 
* *th* qui met en evidence le titre de la ligne.
* *td* qui affiche un par un les éléments de la ligne correspondante. La propriété *rowspan* permet de fusionner la case actuelle avec la case de la ligne d'en dessous.#br

Voici un exemple : #br

#imageCenterCorners(img6.png, 300px, 0)

#hint(Les tableaux offrent pleins de possiblités, vous pouvez tester d'autres combinaisons si vous le souhaitez !)

# Les inputs

La balise input permet de récupérer des données de la part de l'utilisateur. Cela peut-être à peu près n'importe quoi ! Pour le moment cela ne vous est pas forcément utile car il n'y à rien pour récupérer les données rentrées par l'utilisateur. Cela sera surtout utile lorsque nous ferons un workshop sur le PHP ou NodeJS ! Les types les plus répandus sont :

* *Checkbox*
* *Date*
* *Text* qui peut aussi être utilisé avec une propriété *placeholder* qui affiche du texte même quand l'utlisateur n'a rien tapé.
* *Number*
* *File*
* *Color*

Voici un exemple : #br

#imageCenterCorners(img7.png, 300px, 0)

#hint(La balise input est très polyvalente, à vous de tester plusieurs types possibles !)

# Les boutons

Comme la balise *input*, la balise *button* à plusieurs types possibles. 

* Le type *button* qui est le plus basique.
* Le type *submit* qui permet d'envoyer les données d'un formulaire que l'utilisateur aura rempli. (Nous verrons les formulaires plus en détails dans de prochains workshops.)

#hint(Un bouton peut réaliser toutes les actions que vous voudrez grâce à la propriété *onclick* . Pour le moment cela ne vous sera pas utile mais ça le sera dans de futurs workshops !)

# La suite...

Maintenant que vous connaissez toutes les bases du HTML vous pouvez passer aux challenges HTML / CSS que nous avons préparé pour vous. Bonne chance !
