sda                                                   TYPE=disk
├── sda1                                         TYPE=part     MOUNTPOINT=/boot
├── sda2                                         TYPE=part     (partition étendue)
│    └── sda5                                   TYPE=part
│         └── sda5_crypt                    TYPE=crypt
│              ├── name--vg-root         TYPE=lvm   MOUNTPOINT=/
│              ├── name--vg-swap_1    TYPE=lvm   MOUNTPOINT=[SWAP]
│              └── name--vg-home      TYPE=lvm   MOUNTPOINT=/home



sda1 => partition non chiffé pour boot
sda2 => partition étendu
sda5 => partition logique
sda5_crypt => conteneur LUKS
name--vg- => volumes logiques LVM


**SWAP**
Evite les crashs quand la RAM est sature



