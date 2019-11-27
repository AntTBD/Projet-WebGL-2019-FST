# Projet WebGL 2019 FST
 
- declaration des variables
 
- init()
    |_ lancement de la création de tous les objets (scene/renderer/cam/controls/light/obj)
    
- loadModels
    |_ create LoaderManager/OBJLoader/MTLLoader
    |_ chaque mtl (textures) sont chargés puis affecté à l'obj correspondant
         ainsi de suite après chaque fin de chargement des obj
         affectation des objs avec textures dans des var globales
    |_ pour les rails : 
         - stockage des textures et geometry de chaque child dans des tableaux
         - recuperation de ces tex et geo pour recreer les rails au bon endroit grace aux boucles for qui init leur position et rotation
         - stockage de toutes les rails dans des tableaux
    |_ pour la locomotive :
         - ajout de phare qui s'allume lorque le soleil est en dessous du terrain
         - creation d'un tween pour le deplacement avec des courbe de bezier pour les virages
         
         
- animate()
     |_ deplacement de la loco entre chaque rail droit et calcul des courbes pour les virages
