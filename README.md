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

# Notes de réflexion/Suivi de développement
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

