# Script d'installation ruTorrent / Nginx

![logo](https://raw.github.com/xavier84/RatXaBox/master/files/ratxabox.png)
**Auteur :** Ex_Rat
**Modifié par :** Xavier



## Installation:
Multilingue automatique
```
apt-get update && apt-get upgrade -y
apt-get install git-core -y

cd /tmp
git clone https://github.com/xavier84/RatXaBox ratxabox
cd ratxabox
chmod a+x bonobox.sh && ./bonobox.sh
```


**Vous pouvez aussi forcer la langue de votre choix:**
```
# Français
chmod a+x bonobox.sh && ./bonobox.sh --fr

# English
chmod a+x bonobox.sh && ./bonobox.sh --en

# Pусский  ( "д/H" или "y/n" )
chmod a+x bonobox.sh && ./bonobox.sh --ru

# German
chmod a+x bonobox.sh && ./bonobox.sh --de

# Español
chmod a+x bonobox.sh && ./bonobox.sh --es

# Português
chmod a+x bonobox.sh && ./bonobox.sh --pt

# Português do Brasil
chmod a+x bonobox.sh && ./bonobox.sh --ptbr
```
DROIT USER POUR LE REBOOT

nano /etc/sudoers Puis rajouter a la fin www-data ALL = NOPASSWD: ALL

LIEN SYMBOLIQUE POUR LE REPERTOIRE FILES MANAGER LS qui home dans /var/www/rutorrent/files-manager/files

ln -s home var/www/rutorrent/files-manager/files/home

DONNER LES DROIT A TOUS LE HOME POUR POUVOIR EFFACER LES FICHIER DANS LE MANAGER Puis chmord /www-Data tous le home et le reparer

chown -R www-data:www-data /home/

----------------------------------------------------------
Pour gérer vos utilisateurs ultérieurement, il vous suffit de relancer le script

![gestion](https://raw.github.com/xavier84/RatXaBox/master/files/gestion.png)

### Disclaimer
Ce script est proposé à des fins d'expérimentation uniquement, le téléchargement d’oeuvre copyrightées est illégal.

Merci de vous conformer à la législation en vigueur en fonction de vos pays respectifs en faisant vos tests sur des fichiers libres de droits.

### License
This work is licensed under a [Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License](http://creativecommons.org/licenses/by-nc-sa/4.0/)

