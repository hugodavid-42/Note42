MAC = MAndatory access control
securite qui controle l'acces et privilege
- quels fichiers un programme peut lire ou ecrire
- quels repertoire il peut acceder
- quels ports reseau il peut utiliser
- quelles actions systemes il peut effectuer

emplacement -> /etc/appamror.d

Le noyau linux interroge AppArmor a chaque appel systeme

verifier etat general -> *sudo aa-status

installer les outils -> *sudo apt install apparmor-utils*


Mode enforce(programme confine toute action non autorise est bloque) => *sudo aa-enforce /etc/apparmor.d/usr.sbin.sshd*

Mode complain(pas bloque mais enregistre les violations) => *sudo aa-complain /etc/apparmor.d/usr.sbin.sshd*

verifier lancement au demarrage -> *systemctl is-enabled apparmor*
