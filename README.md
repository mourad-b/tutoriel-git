# tutoriel-git

Quelques pistes en français pour démarrer avec **git** (outil en [ligne de commande](https://fr.wikipedia.org/wiki/Interface_en_ligne_de_commande)) et **GitHub** ([application web](https://fr.wikipedia.org/wiki/Application_web) pour partager du code).

* Syntaxe utilisée pour ce fichier README.md : [la syntaxe markdown](https://help.github.com/articles/markdown-basics/)
* C'est quoi Git et GitHub : [une vidéo en français (durée : 01:27:08)](https://www.youtube.com/watch?v=V6Zo68uQPqE) Merci aux auteurs!
* Un éditeur de fichiers textes : [Atom](https://atom.io/)
* Un exemple de fichier (en anglais): [README.md](https://gist.github.com/indexzero/1363524#file-readme-outline-md)
* License : [GPL v3 licence](http://dachary.org/loic/gpl-french.pdf)

## Résumé des commandes utilisées dans la vidéo

*Prérequis : il faut que le logiciel git soit installé*

### Installation

*Pour pouvoir travailler avec un outil de versionnement, il faut que cet outil soit installé sur votre ordinateur.*

* Sur GNU/Linux ou Solaris : [Installation depuis un terminal](http://git-scm.com/download/linux)
* Sur Mac OSX : [Téléchargement et installation](http://git-scm.com/download/mac)
* Sur Windows : [Téléchargement et installation](http://git-scm.com/download/win)

### Configuration

*Il y a certainement plein d'autres options de configuration, mais c'est pour commencer!*

* Vérifier que git est installé : `git --version`
* Définir votre nom : `git config --global "Votre Nom"` (Vous sur GitHub ou pas)
* Définir votre courriel : `git config --global "quelque.chose@domaine.extension"` (Celui utilisé sur GitHub ou pas)
* Afficher votre configuration actuelle : `git config -l`

### Créer un projet

*Ça revient simplement à créer un dossier sur votre ordinateur pour y mettre un unique fichier ou toute une arborescence de fichiers et dossiers.*

* Créer un dossier pour votre projet : `mkdir dossier` (Remplacez «dossier» par ce que vous voulez)
* Rentrer dans ce dossier : `cd dossier`
* Commencer à [gérer les versions](https://fr.wikipedia.org/wiki/Gestion_de_versions) du(des) fichier(s) du projet : `git init`
* S'informer sur l'état du projet : `git status` (peut être utilisé n'importe quand)

### Votre premier fichier

*Un simple fichier texte contenant vos idées, un poème, une liste de tâche ou un début de page html, ou pourquoi pas une image?*

* Créer un fichier : `touch index.html` (ou n'importe quel autre nom de fichier)
* Éditer ce fichier pour y écrire quelque chose : En utilisant un [éditeur de texte](https://fr.wikipedia.org/wiki/%C3%89diteur_de_texte).
* S'informer sur l'état du projet : `git status` (Git vous dira qu'il existe un fichier «index.html» non suivi)
* Demander à git de suivre les versions de ce fichier : `git add index.html` (ou le nom de votre fichier)
* S'informer sur l'état du projet : `git status` (Git vous dira qu'il y a un nouveau fichier)
* Dire à git de prendre en compte cette version du fichier avec un commentaire : `git commit --message "création du fichier"`
* S'informer sur l'état du projet : `git status` (Git vous affichera que la copie de travail est propre et qu'il n'y a rien à valider ou *à commiter*)

### Vos premières modifications

* Éditer votre fichier pour en modifier le contenu : En utilisant un [éditeur de texte](https://fr.wikipedia.org/wiki/%C3%89diteur_de_texte). (votre index.html ou autre fichiers)
* S'informer sur l'état du projet : `git status` (Git vous dira que le fichier «index.html» est modifié)
* Comparer le fichier avant et après ces modification pour voir les différences : `git diff` (les lignes qui commencent par un + sont les ajouts, celles par un - les suppressions)
* Demander à git de suivre les versions de ce fichier : `git add index.html` (ou le nom de votre fichier)
* Dire à git de prendre en compte cette version du fichier avec un commentaire : `git commit -m "modification du fichier"` (notez que --message "commentaire" peut-être raccourcis en -m "commentaire").
* Demander à git une listes des commits et leur commentaires : `git log` (Git vous affichera un ID, l'auteur, la date et le commentaire de chaque *commit*)

TODO : la suite :D

## Autres ressources

* [Autre tutoriel de base](http://christopheducamp.com/2013/12/15/github-pour-nuls-partie-1/)
* [Et sa suite](http://christopheducamp.com/2013/12/16/gitHub-pour-nuls-partie-2/)
* [Autre tutoriel et explications sur le fonctionnement de git](http://www.robusta.io/content/tutoriel/git/start-git.html)
* [Avec quelques info sur .gitignore](http://bloginfo.rakotonirina.net/git-commencer-a-utiliser-git/)
* [Page wikipedia](https://fr.wikipedia.org/wiki/Git)
* [La liste des commandes de git](http://git-scm.com/docs)
* [Visualiser des commit, branch, merge ...](http://www.wei-wang.com/ExplainGitWithD3/)
