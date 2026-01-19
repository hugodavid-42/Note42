*ps aux | grep fdisk* => Sert a reperer les processus | grep filtre la liste pour fdisk

Effacer un processus => 'sudo kill PID'

Paquet pour *pvcreate* => *sudo apt install lvm2*

**PATH**
Liste des dossiers ou linux va chercher les programmes quand tu tapes une commande.
Exmple fait pour ajouter *pvcreate* -> *export PATH=$PATH:/sbin:/usr/sbin*


**EXT4 c'est quoi**
systeme de fichiers moderne et standard de Linux, la maniere dont ils sont organise.
Fonctionnement:
- Journaling -> avant les modifs ext4 ecrit dans un journal ce qu'il va faire
- Extents -> au lieu de stocker en milliers de petit bloc, ext4 regroupe les donnees en groupe contigus.
- Allocation differee -> il attend d'avoir assez d'infos avant d'ecrire (optimisation)
- Verif rapide -> outils comme *fsck* pour reparer ext4


**HOST**
Nom de l'ordinateur

*hostnamectl status*
renommer -> *sudo hostnamectl set-hostname newname*
fichier source -> */etc/hosts*

Strong password policy > 12 characters (combinaison aA9!)

**Ajouter utilisateur**
ajout utilisateur -> *adduser name*
autoriser l'utilisation de sudo -> *sudo usermod -aG sudo name*
voir utilisateur connecte -> *who*
liste utilisateur -> *cut -d: -f1 /etc/passwd*
supprimmer user -> *userdel name*









