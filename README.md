# Bank-No-Break
Code source en langage VHDL et C du système de sécurité embarqué du projet Bank No Break

Nous sommes Bank no break, une start-up spécialisée dans les systèmes de sécurité embarqués pour les banques.

Description du projet :

Notre projet consiste à sécuriser l'accès aux coffres-forts via un clavier sur lequel l'utilisateur doit rentrer un code de vérification.
Ce système de sécurité est composé de  modules différents : un FPGA, un MCU, un clavier, un écran LCD.

Outils de développement : 

- Vivado (Langage VHDL) 
- MPLab (Langage C)

Outils de branchements : 

- carte NEXYS (FPGA)
- carte Microship (MCU) 
- écran LCD
- résistances de 220kOhm 
- jumpers
- afficheur 7 segments
- clavier numérique

Fonctionnement du prototype : 

On a branché le MCU à la carte FPGA par deux fils de connexion représentant l'UART (port RX et TX). 
La carte FPGA est reliée à l'afficheur 7 segments qui à pour but d'afficher des valeurs hexadécimales correspondant aux jours, 
aux mois ou l'année d'une date précise pour lequel l'utilisateur aura accédé à la machine.

Rôle des afficheurs 7 segments :

Pour le premier afficheur (à droite) : affiche la valeur saisie actuelle du clavier numérique.
Pour le deuxième afficheur (à gauche du premier) : affiche le nombre total de saisies sur le clavier avant de taper sur la touche #

les deux derniers : vont afficher de manière binaire

- 0F --> code incorrect 
- 1F --> code correct

le # est la touche de validation, et va afficher "F" sur le 
7 segments.

Les contributeurs du projet :

- Victor Goetschy
- Daniel Amado
- Calixte Angebaud
- Hugo Puszynski
- Arnaud Parmentier 
- Antony Vial

Licence :

Bank no Break, Copyright c, all rights reserved
