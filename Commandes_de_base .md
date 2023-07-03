# Commandes de base sous linux


## Sommaire
* manipulation des fichiers et des répertoires
* gestion des users et des droits
* gestion des logiciels
* commandes avancées
 
## Concepts généraux
Commande : logiciel lancé sans interface graphique
KISS : *Keep It Simple and Stupid*  - chaque commande ne fait qu'une seule chose, on enchaine les commandes pour faire des actions complexes
Les redirections : 
* \> : créé et écrit dans un fichier : sort /etc/passwd > /tmp/users_tries.txt
* \>\> : ajoute à la suite du fichier : date >> /tmp/date.txt
Aide sur une commande : man + la commande, exemple : man ls



## Manipulation des fichiers et des répertoires
* où suis-je ? pwd pour print working directory
* afficher le contenu d'un dossier ? ls pour l**i**s**t
* changer de répertoire courant ? cd + le répertoire (pour change directory), par  "cd /tmp
*  "cd" sans argument ramène dans le répertoire personnel
*  "cd -" revient au dossier précédent
*  Créer un fichier vide ? "touch"
*  Editer un fichier "nano"+le nom du fichier
*  compresser un dossier/fichier ? "tar" + nom de l'archive + nom du fichier/dossier à compresser
   * sans compression : tar cvf archive.tar /home/barth/projets
   * avec compression : tar czvf archive.tar.gz /home/barth/projets
* Extraire une archive tar ? "tar xzvf glpi.tar.gz
* Afficher le contenu d'un fichier ? "cat" + chemin vers le fichier
* Compter le nombre de lignes dans un fichier ? "wc -l" + chemin vers le fichier (pour "word count")
* Afficher la fin d'un fichier ? "tail" + le chemin vers le fichier (tail signifie queue)
   * afficher en temps réel la fin d'un fichier ? "tail -f" + chemin vers le fichier
* Afficher le début d'un fichier ? "head" + le nom du fichier
* Afficher les lignes du fichier / etc/passwd qui contiennent le mot "barth" ? grep barth /etc/passwd



MISE EN PRATIQUE 
Combien d'utilisateurs de mon système utilisent bash "grep bash /etc/passwd | wc - ls"




* 

