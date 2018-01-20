# coopalim-odoo

## Installation 

### mise en place de la machine virtuelle (depuis OVA)

 - Telecharger la machine virtuelle depuis le site bitnami
 - Installer le logiciel de virtualisation (j'ai réussi a lancer la machine avec VMWare Worstation Player 14)

### Installation des modules
 
 Par défaut, il n'est pas possible de rentrer des données. Il faut donc:
  - Installer le module de comptabilité du pays concerné (Français)
  - Cliquer sur Applications > puis installer les modules suivants:
    - Inventory management (Inventory, Logistics, Warehousing)
    - Sales Management (Quotation, Sales Orders, Invoicing)
    - Invoicing Management (Send invoice and track payments)
    - Purchase management (Purchase orders, receipts, vendor bills)?

### Changer la langue

La langue par défaut est l'anglais. Il est possible de passer en français:
 - Cliquer sur Configuration > Traductions > Load translation
   - Sélectionner la langue française
   
# Configuration des modules

Voir *odoo-xxxxxxx.md*, annexes puis configuration pour les paramètres spécifiques.
