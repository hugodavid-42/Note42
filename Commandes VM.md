**Liste de commandes utile:**

- Paquet a ajouter pour un OS debian minimal pour pouvoir utiliser 'sudo apt update: 
	"/etc/apt/sources.list"
	*deb http://deb.debian.org/debian trixie main contrib non-free non-free-firmware (OBLIGATOIRE)
	deb http://deb.debian.org/debian trixie-updates main contrib non-free non-free-firmware
	deb http://security.debian.org/debian-security trixie-security main contrib non-free non-free-firmware
	
-   *sudo swapon --show* (voir les partions swap)
-  *sudo swapoff /dev/sda?* (enleve le swap) 

Afficher la table des partitions:
- *sudo fdisk -l*
- *lsblk*

sda => Disque dur principal
| - sda1 => Une partition primaire ( partition système )
| - sda2 => Partition étendue
| - sda5 => Partition logique
sr0 => Lecteur CD

Créer nouvelle partition:
- *sudo fdisk /dev/sda?* 

/dev/sda1  → primaire
/dev/sda2  → étendue
    ├── /dev/sda5  → logique
    ├── /dev/sda6  → logique
    └── /dev/sda7  → logique

Pour crypter installer cryptsetup:
- *sudo apt install cryptsetup*



