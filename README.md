# Mettre à jour sa machine

apt update && apt full-upgrade -y

# Créer le répertoire du serveur

mkdir /home/fivemserver/ && cd /home/fivemserver/

# Importer l'artifact du serveur

Site: 

apt install curl wget screen tar && wget <lien de l'artifact>

# Décompresser l'artifact

tar xvf fx.tar.xz

rm fx.tar.xz

