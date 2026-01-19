Generateur mot de passe -> *sudo apt install pwgen*
*pwgen*
Pas de caractere speciaux et chiffre

Autre generateur -> apg (pas de chiffre)
openssl => *openssl rand -base64 16*


**Mot de passe**

emplacement -> */etc/login.defs*
configurer parametres d'expirations => *chage -M 30 user*
definir nombre de jour avant changement => *chage -m 2 user*
recap expiration => *chage -l user*

definir valeur par defaut pour new user => *nano /etc/login.defs*

**Implementer regele de mdp**
emplacement -> */etc/pam.d/common-password*

hdavid42: Inception22@

**Groupe**

Emplacement => */etc/group*

creer un groupe -> *groupadd  group-name*
renommer groupe -> *groupmpd -n newname lastname*
Ajouter un membre -> *usermod -G groupa, groupb user-name*
afficher les membres d'un groupe -> *getent group group-name*

supprimer utilisateur d'un groupe -> *gpasswd -d nameuser namegroup*

