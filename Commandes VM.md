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
- cfdisk /dev/sdb?

/dev/sda1  → primaire
/dev/sda2  → étendue
    ├── /dev/sda5  → logique
    ├── /dev/sda6  → logique
    └── /dev/sda7  → logique

Pour crypter installer cryptsetup:
- *sudo apt install cryptsetup*

luksFormat => Linux Unified Key Setup

Donner droit root => *sudo -i*

Mettre un mdp a la partition crypte:
- cryptsetup --verify-passphrase luksFormat /dev/sdb?
Ouvrir:
- cryptsetup luksOpen /dev/sdb?


