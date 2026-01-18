
sda                                                    TYPE=disk      
|
| -> sda1                                                 TYPE = part   MOUNTPOINT = /boot
| -> sda2                                                  TYPE = part        MOUNTPOINT =
| -> sda5                                                  TYPE = part         MOUNTPOINT =
	|→   sda5_crypt                               TYPE = crypt
	        |-> name--vg-root           TYPE =lvm   MOUNTPOINT = /
	        |-> name--vg-swap_1      TYPE=lvm MOUNTPOINT=[SWAP]
	        |-> name--vg-home        TYPE=lvm   MOUNTPOINT=/home
