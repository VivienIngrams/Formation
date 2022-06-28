# Formation

Lancer une commande dans le terminal
Le terminal
Le terminal (aussi appelé console) permet d’exécuter des logiciels en saississant leur nom. On appelle ça exécuter une commande.

Il en existe beaucoup, et chacune a son utilité. Bien heureusement, il n’est absolument pas nécessaire de toute les connaitre.

Cependant, certaines sont utilisées courament, il est donc intéressant de savoir qu’elles existent.

Pour exécuter une commande, on saisi le nom de la commande et on appuie sur la touche Entrée.

Une commande peut être composée de plusieurs éléments :

le nom de la commande
les arguments
Par exemple, dans la commande que nous allons voir juste après,  cd /home/student/Bureau, cd est nom de la commande, /home/student/Bureau est l’argument, une information que l’on transmet à la commande. Une commande peut avoir :

Aucun argument
Un argument
Plusieurs argumements, leur nombre est illimité.
cd
cd, pour Change Directory permet de positionner le terminal dans un dossier. En effet, à l’instar de l’explorateur de fichiers, le terminal est systématiquement positionné dans un dossier. Par défaut, quand on ouvre le terminal, il est positionné dans le dossier utilisateur (/home/student). Si l’on souhaite changer de dossier, il faut donc utiliser la commande cd.

Par exemple cd /home/student/Bureau pour se déplacer dans le dossier /home/student/Bureau.

On peut aussi, si l’on est déjà dans le dossier /home/student, simplement taper cd Bureau.

/home/student/Bureau est un chemin dit absolu. Il nous donne le chemin complet depuis la racine de l’ordinateur. Si on tape cd /home/student/Bureau, un chemin absolu,la commande sera valable peu importe où est positionné le terminal.

Bureau est un chemin relatif, cd Bureau n’est valable que si le terminal est positionné dans le dossier /home/student.

mkdir
Si l’on souhaite créer un nouveau dossier, nous pouvons utiliser la commande mkdir (pour MaKe DIRectory).

Par exemple, je suis dans le dossier /home/student/Bureau/html. Je souhaite créer un dossier S01, je vais utiliser la commande mkdir S01, qui va créer un dossier S01 à l’endroit ou est positionné le terminal. On aurait pu aussi écrire mkdir /home/student/Bureau/html/S01 (chemin absolu) du dossier à créer, le résultat aurait été exactement le même.

Si je souhaite créer plusieurs dossiers d’un seul coup : mkdir S01 S02 S03 S04 S01 S02 S03 S04.

ls
La commande ls, pour LiSt permet de lister les dossiers et fichiers du dossier dans lequel le terminal est positionné. Par défaut elle ne liste pas les fichiers et dossiers cachés (ceux dont le nom commence par .). Si l’on souhaite lister TOUS les fichiers et dossiers, il faut passer l’argument -a (a pour all) à la commande : ls -a.

touch
Si l’on souhaite créer un nouveau fichier vide, nous pouvons utiliser la commande touch.

Par exemple, je suis dans le dossier /home/student/Bureau/html. Je souhaite créer un fichier toto, je vais utiliser la commande touch toto, qui va créer un fichier toto à l’endroit ou est positionné le terminal. On aurait pu aussi écrire touch /home/student/Bureau/html/toto (chemin absolu) du dossier à créer, le résultat aurait été exactement le même.

pwd
Si je souhaite savoir où est positionné le terminal, je peux utiliser la commande pwd, pour Print Working Directory qui va afficher dans le terminal le chemin absolu du dossier dans lequel il est positionné.

 

Utiliser la syntaxe Markdown pour formater un texte
Qu’est ce que c’est ?
Markdown est un langage de mise en forme. C’est à dire que nous allons écrire du texte en rajoutant des indication pour qu’au rendu le texte obtienne cette mise en forme. La syntaxe Markdown est assez utilisée dès qu’il y a un besoin de mise en forme léger :

Slack
Discord
Le chat du cockpit
Github
…
Par exemple, si j’écris le texte suivant en markdown

 

Je suis *en italique* et je suis **en gras**

 

Va donner comme résultat au rendu :

 

Je suis en italique et je suis en gras

 

Le texte markdown sera donc systématiquement lue par un logiciel pour être analysé et affiché avec la mise en forme souhaitée.

La syntaxe
Voici quelques éléments de la syntaxe Markdown

Titres
# Titre niveau 1
## Titre niveau 2
### Titre niveau 3

Mise en forme inline
*italique*
**gras**
~~Texte barré~~

Listes
1. Liste ordonnée
1. Les nombres ici ne comptent pas
1. La liste sera numérotée automatiquement

– Liste
– non ordonnée
– qui contient plein d’éléments

Maîtriser le terminal
Un grand merci à Guillaume L. pour cette prise de note ! 👌

Avant de commencer
Ouverture d’un terminal
Plusieurs options possibles :

En bas à gauche du menu Mint, cliquer sur l’icône du terminal
Depuis n’importe quel endroit, ctrl + alt + t ouvre un terminal (et plus généralement dans la plupart des distributions linux).
La casse
Le shell script (ou le langage que vous utilisez dans le terminal) est un langage qui est sensible à la casse. C’est à dire que les majuscules et les minuscules sont considérées comme des caractères différents.

Par exemple pwd est une commande, alors que PWD ou Pwd ou pWD... n’est pas une commande (n’existe pas).

La tilde ~
Dans le terminal, la tilde représente le répertoire HOME de l’utilisateur (vous). Ce répertoire est celui dans lequel vous trouvez (la plupart du temps) les dossiers suivants :

Bureau
Documents
Modèles
Public
Vidéos
Images
Musique
Téléchargements
L’autocompletion
Très utile. Les développeurs sont des flemmards, c’est pour ça qu’ils ont mis en place l’autocomplétion.
Le principe est d’appuyer sur la touche tabulation pendant la saisie, et l’ordinateur va compléter tout seul votre saisie si il peut.

C’est parti ! Les commandes basiques : naviguez dans vos fichiers à l’aide du terminal.
D’habitude, on utilise un explorateur de fichier, et on clique sur les dossiers pour les ouvrir (ou sur les fichiers). Saviez-vous qu’il était possible d’y naviguer à partir d’un terminal ? Le tout en utilisant seulement trois commandes : pwd, cd et ls.

pwd – Heu je suis où là ?
Première commande. Cette commande est extrêmement utile si vous êtes perdu, elle sert à afficher le dossier dans lequel vous vous trouvez actuellement.

Entrez pwd dans le terminal et appuyez sur entrée.

mint@mint ~ $ pwd
/home/mint
pwd veut dire print working directory et sert à afficher le répertoire courant.
Dans notre cas, le répertoire courant lors de l’ouverture du terminal est /home/mint.

ls – Un peu de lumière svp !
Cette commande sert à afficher la liste des fichier du répertoire courant.
Tapez ls dans le terminal et appuyez sur entrée.

mint@mint ~ $ ls
Bureau   Documents  Modèles  Public           Vidéos
Desktop  Images     Musique  Téléchargements
Par convention, les fichiers/dossiers qui commencent par un point  sont cachés, comme par exemple le fichier .gitignore.
Pour les voir, il faut utiliser la commande ls -a.

Il est possible d’ajouter une mise en liste avec l’option -l soit : ls -l.
Ou même de cumuler les options, mise en ligne et éléments cachés : ls -al.

cd – C’est naze ici, je me casse !
Cette commande sert à se déplacer parmi les fichiers. cd comme Change Directory.
En tapant ls, vous avez précédemment listé les fichiers de votre répertoire courant. Maintenant, essayez de rentrer dans le dossier Documents en tapant cd Documents/

mint@mint ~ $ ls
Bureau   Documents  Modèles  Public           Vidéos
Desktop  Images     Musique  Téléchargements
`
mint@mint ~ $ cd Documents/`
``mint@mint ~/Documents $`
Pour entrez dans un dossier qui se nomme nouveauDossier, tapez `cd nouveauDossier/.`

Dans chaque dossier, le dossier courant est représenté par un ., le dossier courant est le répertoire dans lequel vous vous trouvez actuellement.

Le dossier parent est représenté par ... Donc pour revenir dans le dossier parent, tapez cd ../.

Créez, copiez, et déplacez des fichiers.
mkdir – Aller hop, un nouveau dossier !
Pour créer un dossier, utilisez la commande mkdir qui est l’abrégé de Make directory.
La commande suivante :

`mint@mint ~ $ mkdir nouveauDossier/`
Créera un dossier nouveauDossier dans le répertoire courant.

Autres exemples d’utilisation :

mint@mint ~ $ mkdir ../nouveauDossier/
mint@mint ~ $ mkdir dossierExistant/nouveauDossier/
Vous constatez que mkdir ne se limite pas au dossier actuel, vous pouvez aussi créer des dossiers via mkdir chemin/nouveauDossier

rmdir – Mais il est vide ce dossier ? Aller hop, poubelle !
Cette commande sert à supprimer une dossier vide.
Son fonctionnement est le même que mkdir :

mint@mint ~ $ rmdir dossierASupprimer/
mint@mint ~ $ rmdir ../dossierASupprimer/
mint@mint ~ $ rmdir dossierExistant/dossierASupprimer/
touch – Un nouveau fichier ?
Cette commande sert à créer un nouveau fichier.
Fonctionnement classique :

mint@mint ~ $ touch monfichier.extension
mint@mint ~ $ touch ../dossierExistant/monfichier.extension
mint@mint ~ $ touch dossierExistant/monfichier.extension
rm – Supprimez un fichier ou un dossier qui ne vous plait pas.
Cette commande sert à supprimer un fichier ou un dossier plein (contrairement à rmdir qui ne peut supprimer que des dossiers vide).

Supprime un fichier :

mint@mint ~ $ rm monfichier.extension
Fait une suppression récursive :

mint@mint ~ $ rm -r mondossier/
En gros retenez que c’est avec cette commande que vous pouvez supprimer un dossier contenant d’autres dossiers/fichiers.

Fait une suppression récursive et forcée :

mint@mint ~ $ rm -rf mondossier/
A utiliser avec précaution.

mv – Déplacer ou renommer ? Vous choisissez.
Cette commande permet de déplacer ou de renommer un fichier, en fonction de la façon dont vous l’utilisez.

Mettons que vous êtes dans le dossier courant ~. Dedans vous avez :

Documents
Images
Vidéos
test
Pour déplacer test dans Documents

mint@mint ~ $ mv test Documents
Pour renommer test en supertest

mint@mint ~ $ mv test supertest
cp – Copiez vos fichiers ou vos dossiers
Pour copier un fichier :

mint@mint ~ $ cp chemin/fichier.extension cheminDeDestination/
Pour copier un dossier, on ajoute le paramètre -R (copie récursive) :

mint@mint ~ $ cp -R chemin/monDossier/ cheminDeDestination/
Régler les droits sur un fichier/dossier
Permissions / Droits
Pour définir les droits, il faut déjà savoir les compter !

Type	Chiffre
Lecture	4
Ecriture	2
Exécution	1
Et ensuite on fait la somme des chiffres pour déterminer les droits que l’ont souhaite.

Exemples :

droits en lecture et écriture => 6
droits en lecture, écriture et exécution => 7
droits en lecture uniquement => 4
Utilisateurs
Ensuite, on peut déterminer les permissions pour 3 niveaux/types d’utilisateurs :

l’utilisateur propriétaire du fichier/dossier
le groupe d’utilisateurs lié au fichier/dossier
tous les autres
Ainsi, on peut dire que le propriétaire a tous les droits 7, le groupe lecture + exécution 5, aucun droit pour tous les autres 0 => 750

La commande
chmod 755 /var/www/html :

lecture+ecriture+execution pour le propriétaire du dossier /var/www/html
lecture+execution pour le groupe du dossier /var/www/html
lecture+execution pour tous les autres
chmod -Rf 755 /var/www/html :

applique la commande précédente pour le dossier /var/www/html mais aussi tous ses enfants