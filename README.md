# coopalim-odoo

## Installation 

### mise en place de la machine virtuelle (depuis OVA)

 - Telecharger la machine virtuelle depuis le site bitnami
 - Installer le logiciel de virtualisation (j'ai réussi a lancer la machine avec VMWare Worstation Player 14)

### Activer SSH

sudo rm -f /etc/ssh/sshd_not_to_be_run
sudo systemctl enable ssh
sudo systemctl start ssh

### Retrouver le mot de passe par défaut

For security reasons the master password is randomly generated during the installation of the application. To find the master password, edit the /opt/bitnami/apps/odoo/conf/odoo-server.conf configuration file and search for the line below, which contains the password:

  admin_passwd = PASSWORD

### Changer la langue

La langue par défaut est l'anglais. Il est possible de passer en français:
 - Cliquer sur Settings > Translations > Load translation
   - Sélectionner la langue "French / français"
 - Cliquer sur administrator > Language > French
 - L'interface devrait passer en français
 
### Installation des modules
 
 Par défaut, il n'est pas possible de rentrer des données. Il faut donc:
  - Installer le module de comptabilité du pays concerné (Français)
  - Cliquer sur Applications > puis installer les modules suivants:
    - Gestion de l'inventaire : Inventaire, Logistique, Gestion de stock
    - Gestion des ventes : Devis, commandes, facturation
    - Gestion de la facturation : Envoyer les factures et suivre les paiements
    - Gestion des achats : Bons de commande, Reçus, Factures des Fournisseurs

### Installation de la localisation comptable

 - Configuration > Facturation > Localisation Comptable > Installer plus de localisations comptables
 - Sélectionner l'extension "Comptabilité - France"
   
## Configuration des modules

Voir *odoo-xxxxxxx.md*, annexes puis configuration pour les paramètres spécifiques.
