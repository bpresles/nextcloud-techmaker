# Configuration

Définition des paramètres de base de données et du compte admin dans le répertoire `secrets` :

* nexcloud_admin_user => Nom d'utilisateur pour l'administrateur
* nexcloud_admin_password => Mode de passe pour l'administrateur
* postgres_db => Nom de la base de données
* postgres_user => Nom d'utilisateur pour la base de données
* postgres_pass => Mot de passe de l'utilisateur pour la base de données

## Modification de votre fichier hosts:

### Windows

1. Ouvrir Notepad en mode administrateur
2. Cliquer sur Fichier -> Ouvrir puis Naviguer dans C:\Windows\System32\drivers\etc et ouvrir le fichier hosts (penser à retirer le filtrage sur les fichiers .txt)

### Linux / macOS

1. Ouvrir en mode administrateur le fichier /etc/hosts avec votre éditeur préféré


### Modification

Ajouter la ligne suivante:

```
127.0.0.1 younup.mynextcloud.com
```

Puis enregistrer le fichier

# Démarrage du projet:

```bash
docker-compose up -d
```
