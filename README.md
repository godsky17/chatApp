# Application de Messagerie Instantanée

## 📋 Description du Projet

Ce projet consiste à développer une **application de messagerie instantanée** moderne, simple et performante. Il a été réalisé dans le cadre du cours de **Développement Web et Mobile** par notre équipe. L'objectif est de permettre à des utilisateurs de s'inscrire, de se connecter, et d'échanger des messages en temps réel via une interface intuitive.

---

## ✨ Fonctionnalités Clés

- Inscription et authentification sécurisée des utilisateurs.
- Envoi et réception de messages instantanés en temps réel.
- Statut en ligne/hors ligne des utilisateurs.
- Historique des discussions.
- Responsive design pour une expérience utilisateur fluide sur mobile et desktop.

---

## 📁 Structure du Projet



---

## 🛠️ Technologies Utilisées

- **Backend** : [Node.js](https://nodejs.org/), [Express](https://expressjs.com/), [Socket.IO](https://socket.io/).
- **Frontend** : [React.js](https://reactjs.org/) (ou Vue.js/Angular selon votre choix).
- **Base de Données** : [MongoDB](https://www.mongodb.com/) pour la gestion des utilisateurs et des messages.
- **Authentification** : [JWT](https://jwt.io/) (JSON Web Token) pour sécuriser les accès.
- **Temps Réel** : Socket.IO pour la communication en temps réel entre utilisateurs.

---

## 🚀 Guide de Déploiement

### Pré-requis

Avant de commencer, assurez-vous d'avoir les éléments suivants installés sur votre machine :

- **postgresql** (local) base de donnee. Pour l'instalation de postgresql je vous conseil de vous referez a la documentation ou a la video suivante : https://youtu.be/c_VFpEec5C4?si=aHN6BAY1AYL_DeZg
- **pgAdmin**
- **Git** pour cloner le projet
- **php 8** la version 8 de php au minimum

### Étapes d'Installation

1. **Cloner le dépôt :**
   ```bash
   git clone https://github.com/nom-utilisateur/nom-projet.git
   cd nom-projet
2. **Configuration de la base de donnee**
    Rendez-vous dans le fichier .env de votre projet laravel et configurer la connexion a la base de donnee de la maniere suivante :
    ```bash
    DB_CONNECTION=pgsql
    DB_HOST=127.0.0.1
    DB_PORT=5432
    DB_DATABASE=chatapp_db
    DB_USERNAME=postgres
    DB_PASSWORD=postgres
    

    Ensuite allez dans le fichier config/database.php et modifier la ligne concernant la connexion par defaut a la base de donnee :
    ```bash
    'default' => env('DB_CONNECTION', 'pgsql'),
   
3. **Migration de la base de donne**
   ```bash
   php artisan migrate

4. **Lancement du projet**
   ```bash
   php artisan serve

   Ensuite ouvrer votre navigateur et lancer  le projet en suivant l\'addresse du projet.
   http://localhost:8000

5. **Se rendre sur sa branche de travaille**
```bash
git branch
git switch nom_de_la_branche

