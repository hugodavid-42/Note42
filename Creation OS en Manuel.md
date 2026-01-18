**Partion disk settings:**
- Use as => Choix du type d'utilisation :
	- Ext4 journaling file system -> /, /home. /boot
	- swap area -> pour la partition swap
	- physical volume for encryption -> sda5(LUKS)
	- physical volume for LVM -> LVM sans chiffrement

- Mount point => 

- Mount options => fonctions avancés pour monter la partition:
	- *defaults*
	- *noatime* -> optimise le ssd
	- *ro* -> lecture seule

- Label => Nom facultatif pour la partition:

- Reserved blocks => pourcentage déspace réservé a root, utile pour qu'un disque plein ne bloque pas le system:
	- Pour /boot et / laisse 5%
	- Pour /home mettre a 0 pour optimiser l'espace

- Typical usage => Optimisation du systeme de fichiers

- Bootable flag => indique si la partition ets amorcable

**Vue d'ensemble LVM**
- PV - Physical Volume => c'est la base ou LVM est stocke
- VG - Volume Group => Grand reservoir dans lequel on cree les volumes logiques
- LV - Logical Volume => Partitions virtuelles qu'on va utiliser co;;e si elles etaient normales.

[PV] = la partition chiffrée
   ↓
[VG] = un grand sac de stockage
   ↓
[LV root]  = / 
[LV home]  = /home
[LV swap]  = swap

