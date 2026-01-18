SSH = Secure Shell
- Se connecter a distance
- Executer des commandes a distances
- transferer des fichiers de manieres secur
- administrer un serveur sans ecran ni clavier
Donne un terminal a distance, mais chiffre et securise

SSh ecoute le port 22 par default
Modification possible dans */etc/ssh/sshd_config*
chnager le port permet d'eviter l'attaque de bot qui vise le port par defaut

trouver son ip debian -> *ip a*
10.0.2.15

installer SSH => *sudo apt install openssh-server*
 voir le statut de ssh => *sudo systemctl status ssh*

installer *ss* -> *sudo apt install iproute2*

*sudo ss -tlnp*


**Connecter a SSH**
username@ip
deconnecter -> exit ou logout ou ctrl +D

 **changer le port de ssh**
 *sudo nano /etc/ssh/sshd_config* et ssh_config
redemarrer ssh -> *sudo systemctl restart ssh*
verfie -> *sudo systemctl status ssh*

 