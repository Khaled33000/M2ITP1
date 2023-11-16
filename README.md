# Installation automatisée de WordPress avec Terraform et Ansible sur Google Cloud
## Ce script permet d’installer automatiquement une stack WordPress avec une base de données MySQL sur des machines virtuelles GCP.
## Prérequis

- Un compte GCP avec des credentials configurées
- Terraform et Ansible installés localement

## Utilisation

- Pour utiliser le script: Clonez ce dépôt
Lancez le script install.sh: ./install.sh

## Le script va:

- Générer une paire de clés SSH
- Vérifier que Terraform est installé
- Initialiser le dossier Terraform et appliquer la configuration
- Récupérer les IP des machines WordPress et MySQL
- Vérifier qu'Ansible est installé
- Générer le fichier d'inventaire Ansible
- Appliquer les playbooks Ansible pour configurer WordPress et MySQL
- Vérifier que WordPress est accessible

## Architecture

Le script utilise:

- Terraform pour provisionner les machines GCE sur GCP
- Ansible pour installer et configurer WordPress et MySQL

La configuration Terraform se trouve dans terraform/.
Les playbooks Ansible utilisent des roles Ansible Galaxy.
2
