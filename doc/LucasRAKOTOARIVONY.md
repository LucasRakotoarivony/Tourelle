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

# Séance du 12 mars 2018

Pour commencer j'ai écrit la partie du code servant à controler le servomoteur permettant de déclencher le tir. Ce code consiste juste à modifier le servowrite du servomoteur.

Ensuite j'ai relié le servomoteur au Nerf et j'ai commencé les essais. J'ai rencontré deux problèmes, le premier est que le matériel que j'ai utilisé pour fixer l'embout du servomoteur et la gachette n'était pas assez solide donc j'ai du prendre des matériaux plus solides, le second problème est que si le servomoteur est laissé sans contrainte c'est toute la partie supérieure du servomoteur qui va tourner et non la gachette.

Je n'ai pas encore résolu le dernier problème est actuellement je fais mes essais en bloquant le servomoteur avec mes mains. Cependant en utilisant cette solution j'arrive à tirer avec mon Nerf.

# Séance du 26 mars 2018

Durant cette séance j'ai perfectionné le système de tir, j'arrive maintenant à tirer avec mon Nerf en continu. Il ne me reste plus qu'a bloquer le servomoteur pour l'empêcher de tourner. Je ferai cela à la séance prochaine.

Ensuite j'ai commencé à travailler sur la structure de la tourelle, je pense installer le Nerf sur une plateforme en carton et mettre cette plateforme sur un servomoteur ou un moteur pas à pas. J'ai également fais des recherches pour trouver un moteur assez puissant pour faire tourner la plateforme rapidement.

De plus j'ai également écouté les différents exposés de mes camarades.

# Séance du 05 avril 2018

Pour commencer j'ai fait la présentation de mon projet et j'ai écouté celles de mes camarades.

Ensuite j'ai finalisé le tir de mon Nerf. J'ai percé deux trous dans la structure du Nerf pour pouvoir fixer le Nerf. Le Nerf tire donc sur commande.

J'ai ensuite chercher un servomoteur qui me servira à faire pivoter ma tourelle, j'ai cherché un servomoteur assez puissant pour faire tourner ma structure aisément. Pour l'instant je vais essayer le servomoteur mg996r mais je changerai sûrement si il n'est pas assez puissant.

# Séance du 09 avril 2018

J'ai décidé d'utiliser un servomoteur HS-311 pour faire pivoter ma tourelle. J'ai donc vissé l'embout et je l'ai attaché à mon Nerf.

Ensuite j'ai effectué des tests pour savoir quelle position du moteur permet de orienter le Nerf selon la direction indiqué par la caméra.

Et enfin j'ai cherché comment bloquer le servomoteur pour que ce ne soit pas lui qui tourne.

# Séance du 02 mai 2018

Durant cette séance j'ai cherché comment bloquer mon Nerf et j'ai cherché un support pour placer ma tourelle en équilibre. J'ai donc utilisé une planche comme support. J'ai ensuite cherché des vis pour bloquer le moteur.

Finalement cette solution est compliqué à mettre en place car la planche est trop volumineuse et lourde, j'ai donc décidé de créer le support moi-même en utilisant Autodesk, et ensuite aller l'imprimer ce support au Fablab.
