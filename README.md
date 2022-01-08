# Projet WebGL 2019 FST
 
<ul>
    <li>declaration des variables</li>
    <li>init()
        <ul>
            <li>lancement de la création de tous les objets (scene/renderer/cam/controls/light/obj)</li>
        </ul>
    </li>
    <li>loadModels()
        <ul>
            <li>create LoaderManager/OBJLoader/MTLLoader</li>
            <li>
                chaque mtl (textures) sont chargés puis affecté à l'obj correspondant<br>
                ainsi de suite après chaque fin de chargement des obj<br>
                affectation des objs avec textures dans des var globales
            </li>
            <li>
                pour les rails : <br>
                - stockage des textures et geometry de chaque child dans des tableaux<br>
                - recuperation de ces tex et geo pour recreer les rails au bon endroit grace aux boucles for qui init leur position et rotation<br>
                - stockage de toutes les rails dans des tableaux
            </li>
            <li>
                pour la locomotive : <br>
                - ajout de phare qui s'allume lorque le soleil est en dessous du terrain<br>
                - creation d'un tween pour le deplacement avec des courbe de bezier pour les virages
            </li>
        </ul>
    </li>
    <li>animate()
        <ul>
            <li>deplacement de la loco entre chaque rail droit et calcul des courbes pour les virages</li>
        </ul>
    </li>
</ul>
   
         
<p>Animation:</p>

![Animation](rapport/screens/animation.gif)

<img src="rapport/screens/all%20textures.PNG" height=500>
