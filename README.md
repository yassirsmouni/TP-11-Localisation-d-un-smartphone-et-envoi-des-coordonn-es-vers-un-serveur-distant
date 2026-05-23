# 📍 TP 11 - Localisation et envoi vers serveur distant

## 📌 Description
Application Android connectée à un backend PHP/MySQL.  
Elle récupère la localisation GPS (latitude, longitude), la date et l’identifiant du téléphone, puis envoie ces données vers un serveur PHP via Volley.

---

## 🏗️ Architecture du projet

### 📱 Android
- Récupération GPS (latitude et longitude)
- Permissions localisation et Internet
- Envoi des données via Volley (HTTP POST)
- Affichage des informations (date et device ID)

---

### 🌐 Backend
- `database.sql` : création base et table
- `receive_position.php` : script de réception des données
- `config/` : connexion base de données
- `models/` : classe Position
- `dao/` : insertion en base

---

## 🗄️ Base de données
- Nom : `tp11_location`
- Table : `position`

### Champs :
- id
- latitude
- longitude
- date_envoi
- device_id

---

## ⚙️ Installation du backend

- Copier le dossier backend dans :
  `C:/xampp/htdocs/tp11_position`

- Importer `database.sql` dans MySQL via phpMyAdmin

- Configurer la connexion dans :
  `config/Database.php`

---

## 📱 Lancer l’application Android

- Ouvrir le projet dans Android Studio
- Lancer sur émulateur ou téléphone
- Ou via terminal :
---

## 🌐 URL du serveur

---

## 📡 Fonctionnement

- Récupération GPS
- Récupération date + device ID
- Envoi des données via Volley (POST)
- Réception côté PHP
- Insertion dans MySQL

---

## 📱 Sur téléphone réel

Remplacer :
par l’adresse IP du serveur local (ex: 192.168.x.x)

---

## 🚀 Conclusion

Ce projet permet de comprendre la communication entre Android et PHP/MySQL avec localisation GPS et envoi de données en temps réel.
