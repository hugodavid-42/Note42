aller en root -> su -

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



