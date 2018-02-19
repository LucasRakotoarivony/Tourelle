# Cahier de suivi du projet de Lucas Rakotoarivony.

# Séance du 21 décembre 2017.

J'ai formé mon groupe composé de moi seul. J'ai décidé de créer une tourelle automatique qui détecte les objets en mouvements et leur tirent dessus à l'aide d'un Nerf.

Durant cette séance j'ai cherché le matériel nécessaire à ce projet. J'ai décidé d'utiliser une caméra Pixy, un moteur pas à pas et un Nerf. De plus pour utiliser la caméra Pixy j'utilise une carte Arduino Uno.


# Séance du 10 janvier 2018.

J'ai installé et commencé à utiliser PixyMon, l'application permettant de visualiser ce que voit la caméra Pixy.

J'ai aussi commencé à apprendre à utiliser le moteur pas à pas à l'aide de tuto et des exemples proposé par Arduino.

J'ai également démonté et utilisé le Nerf pour comprendre son fonctionnement et comment les élèves des années précédentes l'avaient utilisé.

De plus j'ai demandé à Monsieur Masson un servo-moteur afin de pouvoir déclencher le tir avec le Nerf.


# Séance du 19 janvier 2018.

J'ai démonté le Nerf afin d'accéder au mécanisme permettant de déclencher le tir. J'ai décidé d'y accrocher un embout de servomoteur pour pouvoir déclencher le tir sur commande de l'Arduino. Tout d'abord j'ai utilisé du scotch mais dès que je commencais à faire tourner le moteur, le scotch se détachait et l'embout également.
J'ai donc utilisé 2 serre cable et du fil de fer pour maintenir l'embout. Cette solution fonctionne pour maintenir l'embout cependant si je branche le servomoteur et que je le commande, c'est le moteur entier qui tourne et non l'embout. Je vais donc devoir fixer le moteur pour l'empêcher de tourner. 

# Séance du 24 janvier 2018.

J'ai passé une bonne partie de la séance a écouté les différents exposés de mes camarades.

Dans le temps restant de la séance j'ai réparé le chargeur du Nerf pour que à chaque tir la seconde cartouche se positionne correctement.

J'ai également cherché une solution pour fixer le servomoteur au Nerf de manière solide.
Et enfin j'ai cherché une solution pour déclencher un chronomètre si un objet était détecté par la caméra Pixy.

# Séance du 06 février 2018.

Durant les vacances de ski j'ai avancé mon programme et j'arrive désormais à calculer la trajectoire approximative d'un objet qui passe devant la caméra. (mon programme est disponible sur ce github).

Donc durant cette séance j'ai commencé par implémenter à ce code l'utilisation du servomoteur et j'ai testé mon programme en lançant un objet de couleur devant la caméra. J'ai ainsi remarqué plusieurs problèmes, le premier est que le programme fonctionne uniquement si l'objet va de la gauche vers la droite. De plus je n'ai toujours pas trouvé comment faire pour que le servomoteur s'oriente de manière précise en fonction de mes calculs.

A la fin de la séance j'ai fait des recherches pour savoir quel moteur serait le plus pratique pour faire pivoter ma tourelle, le moteur pas à pas ou le servomoteur. Pour l'instant j'utilise le servomoteur parce que je le maîtrise mieux.

# Séance du 19 février 2018

Tout d'abord j'ai modifié mon programme pour le réinitialiser si on passe un objet d'une certaine couleur devant la caméra, ou si aucun objet n'était détecté pendant environ 3 secondes.

Dans le rapport du 06 février je parle d'un problème lorsque l'objet va de la gauche vers la droite, durant cette séance je l'ai corrigé. Il fallait juste considérer deux cas, le premier si l'objet va de la droite vers la gauche et le second si l'objet va de la gauche vers la droite.

J'ai ajusté mon servomoteur pour qu'il montre où va atterir l'objet reperé par la caméra, pour l'instant le résultat est mitigé en effet le servomoteur pointe la bonne direction mais je ne pense pas qu'il soit très précis.
