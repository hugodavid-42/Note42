**Liste de commandes utile:**

- Paquet a ajouter pour un OS debian minimal pour pouvoir utiliser 'sudo apt update: 
	"/etc/apt/sources.list"
	*deb http://deb.debian.org/debian trixie main contrib non-free non-free-firmware (OBLIGATOIRE)
	deb http://deb.debian.org/debian trixie-updates main contrib non-free non-free-firmware
	deb http://security.debian.org/debian-security trixie-security main contrib non-free non-free-firmware
	
-   *sudo swapon --show* (voir les partions swap)
-  *sudo swapoff /dev/sd?* (enleve le swap) 

Afficher la table des partitions:
- *sudo fdisk -l*
- *lsblk*

Créer 