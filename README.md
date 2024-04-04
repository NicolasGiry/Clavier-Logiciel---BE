# Clavier-Logiciel - BE

Ce projet est un bureau d'études réalisé avec l'aide de M. Raynal, chercheur à l'IRIT sur le domaine de l'amélioration des systèmes de saisie de texte. 
Le but est de réaliser un clavier logiciel à destination de personnes en situation de handicap moteur, utilisant un pointeur à la place d'un clavier physique.
L'utilisation d'un système de prédiction linguistique sera utilisée pour simplifier la saisie. De plus, il est important de réduire au maximum la distance parcourue
par le pointeur, pour éviter à l'utilisateur de s'épuiser.

Le projet a un but expérimental, me permettant de développer et d'imaginer un nouveau clavier qui répondra au mieux aux critères cités plus haut.
J'ai réalisé un état de l'art des claviers logiciels existants, pour mieux appréhender l'élaboration de ma solution.
Le clavier que je propose sera structuré selon 3 cercles concentriques. Rangeant les lettres les plus probables dans le cercle le plus au centre et les moins probables sur le cercle extérieur. 
À chaque touche pressée, on calculera la lettre la plus probable d’être sélectionnée à la suite. Si celle-ci ne se trouve pas dans le cercle le plus au centre alors on va l’introduire à l’intérieur, 
en échangeant sa place avec la lettre la moins probable de ce cercle. Pour indiquer ce changement, la lettre ajoutée émettra un léger flash lumineux, cela attirera le regard de l’utilisateur,
l’aidant à sélectionner la lettre la plus probable. L’objectif est que la prochaine lettre choisie soit toujours le plus au centre pour que l’utilisateur bouge le moins possible son pointeur. 

premier prototype :

![Screenshot 2024-03-25 231542](https://github.com/NicolasGiry/Clavier-Logiciel---BE/assets/114723956/7b18e8bb-c1fd-43a5-8e9a-ead504b7ffa0)

Démonstration clavier statique : 

https://github.com/NicolasGiry/Clavier-Logiciel---BE/assets/114723956/6204d85f-f796-42b6-852b-31ae712c1a00
