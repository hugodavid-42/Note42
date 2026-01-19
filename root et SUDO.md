aller en root -> su -

modif sur la commande sudo -> *visudo*
- Defaults passwd_tries=3
- Defaults badpass_message=*msg*
recuperer les logs => *Defaults log_input,log_output*

Indique ou stocker les logs => *Defaults iolog_dir="/var/log/sudo"*

ecrit un resume de l'action dans ce fichier => *Defaults logfile="/var/log/sudo/sudo.log"*

Forcer les commandes depuis un termina reel => *Defaults requiretty*

Ou trouver les logs => *Defaults secure_path="/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/snap/bin"*


**Archiver action sudo**
emplacement -> /var/log/sudo
sudo mkdir -p /var/log/sudo
sudo chmod 700 /var/log/sudo


SUDO => Substitude User DO
execute commande sous autre utilisateur => *sudo -u user*

autoriser l'utilisation de sudo -> *sudo usermod -aG sudo name*
lister permissions -> *sudo -l*  ou *id user* 

emplacement => */etc/sudoers*


changer permission en tant que root => visudo
	%SUDO    ALL=(ALL:ALL)ALL
	usergroup  hote=(user:groupes)commandes

Exemple:
user ALL=(ALL) /usr/bin/nano /etc/hosts



