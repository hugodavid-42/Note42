free -m | grep "^Mem:" | awk {print $3}

Commande *awk*:
pour prendre que les chiffre => '{gsub(/[ ^0-9]/,""); print}'