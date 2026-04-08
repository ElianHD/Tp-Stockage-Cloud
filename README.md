# ☁️ Tp-Stockage-Cloud

## 📌 Description

Ce projet permet de déployer un serveur de stockage cloud personnel avec **ownCloud** via Docker et Docker Compose.

Il permet de :

* Stocker et partager des fichiers
* Accéder à ses données depuis un navigateur
* Créer un cloud personnel sur un réseau local

---

## 🛠️ Prérequis

Avant de commencer, il faut installer :

### 🔹 Git

```bash
sudo apt update
sudo apt install git -y
```

### 🔹 Cloner le projet

```bash
git clone https://github.com/ton-utilisateur/Tp-Stockage-Cloud.git
cd Tp-Stockage-Cloud
```

---

## 🛠️ Technologies utilisées

* Docker
* Docker Compose
* ownCloud
* MariaDB

---

## 📂 Structure du projet

```
.
├── docker-compose.yml   # Configuration des conteneurs
├── install_docker.sh    # Script d'installation de Docker
└── README.md            # Documentation du projet
```

---

## ⚙️ Installation

### 1️⃣ Installer Docker

```bash
chmod +x install_docker.sh
./install_docker.sh
```

---

### 2️⃣ Lancer le projet

```bash
docker-compose up -d
```

---

## 🌐 Accès à l'application

Une fois lancé, accède à ownCloud via :

👉 http:/localhost:8080

---

## 🔐 Identifiants par défaut

* **Utilisateur** : admin
* **Mot de passe** : adminpass

⚠️ Pense à les modifier après la première connexion !

---

## 📦 Fonctionnement

* Le service **ownCloud** gère l’interface web et les fichiers
* Le service **MariaDB** gère la base de données
* Les données sont persistées grâce aux volumes Docker

---

## 🔧 Commandes utiles

### Arrêter les conteneurs

```bash
docker-compose down
```

### Supprimer complètement (⚠️ supprime les données)

```bash
docker-compose down -v
```

### Voir les logs

```bash
docker-compose logs -f
```

---

## 🚀 Améliorations possibles

* 🔒 Ajouter HTTPS (certificat SSL)
* 🌍 Accès depuis Internet
* 📱 Synchronisation avec mobile
* 🔁 Sauvegardes automatiques

---

## 👤 Auteur

Projet réalisé par **ElianHD**

---

## 📜 Licence

Projet à but éducatif (TP BTS SIO)
