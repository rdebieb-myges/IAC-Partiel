# Je n'ai pas utiliser un cloud provider pour tester mon code en raison de l'expiration des crédits !
## Terraform (GCP)
Dans les fichiers se trouve:
  - Création d'un projet GCP
  - La création d'une instance GCP sous debian 12 avec une adresse IP publique dédié (affecté au projet GCP)
  - Le billing account

Un terraform plan était nécessaire afin de connaitre le provider utilisé.
Le terraform apply a permit de construire mes ressources.

## Ansible
### Création du répertoire ansible
Création du dossier playbook + de l'inventaire

### Playbook
Mettre à jour les repos pour avoir python en version 3.11

Cloner le repo où se trouve les requirements et l'application

Installer les requirements avec pip

Créer un utilisateur dédié pour l'API

Créer le service FastAPI grace à systemd

Relancer le démon systemd afin qu'il puisse prendre en compte le nouveau service + enable le service pour qu'il démarre au démarrage maintenant ainsi qu'au démarrage de la machine.
