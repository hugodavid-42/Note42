Generateur mot de passe -> *sudo apt install pwgen*
*pwgen*
Pas de caractere speciaux et chiffre

Autre generateur -> apg (pas de chiffre)
openssl => *openssl rand -base64 16*


**Mot de passe**
configurer parametres d'expirations => *chage -M 30 user*
definir nombre de jour avant changement => *chage -m 2 user*
recap expiration => *chage -l user*

definir valeur par defaut pour new user => *nano /etc/login.defs*

hdavid42: 
