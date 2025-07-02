# Déploiement

## Vue d'ensemble

Cette page contient les procédures et bonnes pratiques pour le déploiement de nos applications.

## Hébergement

### OVH

#### Créer un sous-domaine

1. **Accéder à l'hébergement**
   - Aller dans **Hébergement**
   - Cliquer sur le domaine concerné

2. **Configuration du multisite**
   - Aller dans l'onglet **Multisite**
   - Dans le menu déroulant **Action** > Cliquer sur **Ajouter un domaine ou sous-domaine**

3. **Paramétrage du sous-domaine**
   - Choisir le domaine concerné
   - Renseigner le sous-domaine
   - **Dossier racine** : `www/xxx/public`
   - Valider

#### Régénération du certificat SSL

1. **Accès aux informations générales**
   - Aller dans l'onglet **Informations générales**
   - Localiser le bloc **Configuration**

2. **Régénération du certificat**
   - Cliquer sur **Certificat SSL...**
   - Sélectionner **Régénérer le certificat SSL**

> **Note** : La régénération du certificat SSL peut prendre quelques minutes à quelques heures pour être effective.

## Configuration GitHub

### Ajouter les secrets de déploiement

1. **Accéder aux paramètres du dépôt**
   - Aller sur le dépôt GitHub
   - Cliquer sur **Settings**

2. **Configuration des secrets**
   - Dans le menu de gauche, cliquer sur **Secrets and variables** > **Actions**
   - Cliquer sur **New repository secret**

3. **Ajouter les secrets FTP**
   Créer les 3 secrets suivants :
   - `OVH_FTP_HOST` : Adresse du serveur FTP
   - `OVH_FTP_USER` : Nom d'utilisateur FTP
   - `OVH_FTP_PASSWORD` : Mot de passe FTP

> **Important** : Ces secrets permettront au workflow GitHub Actions de se connecter au serveur OVH pour le déploiement automatique.