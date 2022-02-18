# :computer: Installer un serveur FiveM sur un VPS Linux

# Mettre à jour sa machine

`apt update && apt full-upgrade -y`

# Créer le répertoire du serveur

`mkdir /home/fivemserver/ && cd /home/fivemserver/`

# Importer l'artifact du serveur

Site: https://runtime.fivem.net/artifacts/fivem/build_proot_linux/master/

`apt install curl wget screen nano tar && wget <lien de l'artifact>`

# Décompresser l'artifact

`tar xvf fx.tar.xz`

`rm fx.tar.xz`

# Installer les dépendences pour la base de données 

`apt install apache2 php libapache2-mod-php mariadb-server php-mysql php-curl php-gd php-intl php-json php-mbstring php-xml php-zip -y`

# Installer le panel web (Phpmyadmin)

`apt install phpmyadmin -y`

# Configurer MariaDB

`mysql`

`ALTER USER 'root'@'localhost' IDENTIFIED BY 'motdepasse';`

`exit`

# Editer le server.cfg

`nano server.cfg`
