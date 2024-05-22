# Introduction : mon intention
Ce projet me permet de créer une petite librairie CSS légère pour mes projets web. L'idée est d'avoir un fichier CSS prêt à l'emploi (style.css) situé à la racine de ce répertoire et ainsi avoir une mise en page agréable et UX/UI Friendly pour mes projets web.

Ce qu'on va retrouver dans ce répertoire simple niveau arborescence : 
* Le fichier index.html pour visualiser les composants stylisés
* Le fichier style.css qui contiendra le code CSS généré
* Le dossier src qui contient mon code SASS

# Comment installer ?
1. Télécharger le fichier style.css
2. Ajouter dans son HTML la ligne pour ajouter Font Awesome : 
```html
<link href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.2/css/fontawesome.min.css" rel="stylesheet" />
```

# Outils pour développer
* SASS : Pour faciliter la mise à jour et l'évolution du style CSS
* Font Awesome : Pour gagner du temps en utilisant des icônes préconçues

# Composants souhaités
* Un menu responsive
* Des jolis boutons (radio, toggle, checkbox, options)
* Un joli accordéon
* Des badges colorés
* Des formulaires contrôlés en HTML uniquement
* Des textes formatés (H1,...)
* Des animations de conteneurs simples (images ou section)

# Les conteneurs
Par défaut, le body fera toujours 100% en mobile, et 1000px lorsqu'il fera minimum 60em de largeur (grâce à la classe .main). 

## Des lignes et des colonnes
* Le <body> contient un conteneur (div.container) qui définit les lignes de la page
* Le conteneur div.container fait 100% de son parent, et peut contenir jusqu'à 4 colonnes (.col)
```html
<div class="container">
        <div class="col">
            <h2>Je suis la colonne 1/h2>
            <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Maiores ad quis debitis rerum officia
                accusantium
                quod optio earum, excepturi consequuntur? Amet cum sapiente id harum neque illo assumenda error
                voluptates!</p>
        </div>
        <div class="col">
            <h2>Je suis la colonne 2</h2>
            <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Maiores ad quis debitis rerum officia
                accusantium
                quod optio earum, excepturi consequuntur? Amet cum sapiente id harum neque illo assumenda error
                voluptates!
            </p>
        </div>
```
# Les images
La taille des images est par défaut définit à 100% en largeur et leur hauteur dépend de la taille de l'affichage. Les images peuvent avoir l'attribut cover avec la classe .img-cover ou contain avec la classe .img-contains. On peut également appliquer un effet de rondeur aux bords d'une image avec la classe .rounded

# Notes de réflexion/Suivi de développement
* 21/05/2024
  - Design des boutons : pour appliquer le style sur un bouton (ou en créer un sur une balise link), il faut utiliser la classe .btn. Si l'on souhaite un bouton rond, on ajoute la classe .btn-rounded. 
  - Couleur : comme avec la plupart des librairies CSS, on peut utiliser la classe btn-primary ou btn-secondary pour définir la couleur du bouton.
* 16/05/2024
  - Finalement, je reste sur l'idée de positionner les conteneurs comme si on était dans un tableau : il y a un conteneur principal pour toute la page (.main) qui reste à 100%. Il y a ensuite un conteneur pour mes éléments (.container) et des colonnes qui vont contenir les textes, images, etc (.col). C'est assez lisible, et largement inspiré des librairies CSS existantes.
  - J'essaie d'être le plus mobile-first possible.
* 15/05/2024 : 
  - Gestion du placement des conteneurs grâce aux Flexbox 
* 14/05/2024 - branche feature-containers : 
  - Responsive : Gestion du placement des conteneurs grâce aux Flexbox => en cours
  - UX/UI Friendly : Gestion des tailles et des espaces entre les différents éléments conteneurs => à faire 
* 14/05/2024 - branche feature-tiles : 
  - Je pars sur un nommage anglophone, pour être raccord avec ce qu'il se fait généralement. Branche feature-titles done pour le moment => Je la merge à la main sans trop de risque.
  - Création d'une classe 'tagline' pour les éventuelles phrases d'accroches.
  - Pas de marges intérieures/extérieures sur le style des titres et textes, on gère ça dans les conteneurs.
* 13/05/2024 : Première étape, bien structurer mon repo Git. Je pense créer une branche par composant. 

