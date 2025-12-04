# 📦 AmmaExpress - Système de Livraison de Colis en Temps Réel

![Spring Boot](https://img.shields.io/badge/Spring_Boot-F2F4F9?style=for-the-badge&logo=spring-boot)
![Java](https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-005C84?style=for-the-badge&logo=mysql&logoColor=white)
![WebSockets](https://img.shields.io/badge/Real--Time-WebSockets-blue?style=for-the-badge)

> **Projet de Fin d'Année (PFA) 2024/2025**
> **École Marocaine des Sciences de l'Ingénieur (EMSI)**
> *Filière : Ingénierie Informatique et Réseaux*

---

## 📄 Description

**AmmaExpress** est une application web de gestion logistique conçue pour répondre aux défis de la livraison urbaine moderne. La plateforme permet la mise en relation directe entre les clients et les livreurs, avec une gestion complète du cycle de vie des colis.

L'objectif principal est de fournir une solution **simple, rapide et interactive** intégrant des fonctionnalités de **suivi en temps réel** via WebSockets, garantissant ainsi transparence et efficacité pour tous les acteurs (Clients, Livreurs, Administrateurs).

## 🚀 Fonctionnalités Clés

### 👤 Espace Client
* **Création de Colis :** Formulaire intuitif pour soumettre une demande de livraison.
* **Suivi en Temps Réel :** Visualisation de l'état du colis (En attente, En cours, Livré).
* **Historique :** Consultation de l'historique des envois passés.
* **Code de Suivi :** Recherche rapide de colis via un identifiant unique.

### 🚚 Espace Livreur
* **Gestion des Missions :** Visualisation des colis disponibles et en attente de prise en charge.
* **Mise à jour des Statuts :** Changement d'état des colis en temps réel (Prise en charge -> Livré).
* **Tableau de Bord :** Vue d'ensemble des livraisons effectuées et en cours.

### 🛡️ Espace Administrateur
* **Supervision Globale :** Dashboard statistique (Nombre de colis, utilisateurs actifs, livreurs).
* **Gestion des Utilisateurs :** Validation des comptes livreurs et gestion des clients.
* **Traçabilité :** Accès complet aux logs et à l'état du système.

---

## 🛠️ Architecture Technique

Le projet repose sur une architecture modulaire et robuste :



[Image of Spring Boot WebSocket architecture diagram]


| Composant | Technologie | Description |
| :--- | :--- | :--- |
| **Backend** | Java / Spring Boot | Logique métier, API REST et gestion de sécurité. |
| **Frontend** | HTML, CSS, JS | Interface utilisateur responsive (Bootstrap/Tailwind). |
| **Temps Réel** | WebSockets | Communication bidirectionnelle pour le suivi instantané. |
| **Base de Données** | MySQL | Persistance des données (Géré via phpMyAdmin). |
| **Serveur Local** | Laragon | Environnement de développement WAMP/LAMP. |

---

## 📸 Captures d'écran

### 1. Page d'Accueil & Services
Une interface accueillante présentant les services et le suivi rapide.
*(Insérer ici Figure 3.1 ou 3.3 du rapport)*
`![Page d'Accueil](screenshots/image_home.png)`

### 2. Dashboard Client & Suivi
L'espace personnel permettant de gérer les envois.
*(Insérer ici Figure 3.11 ou 3.14 du rapport)*
`![Dashboard Client](screenshots/dashboard_client.png)`

### 3. Interface Livreur
Gestion des colis en attente et prise en charge.
*(Insérer ici Figure 3.34 ou 3.35 du rapport)*
`![Interface Livreur](screenshots/interface_livreur.png)`

### 4. Dashboard Admin
Statistiques globales et gestion des utilisateurs.
*(Insérer ici Figure 3.27 du rapport)*
`![Dashboard Admin](screenshots/dashboard_admin.png)`

---

## 💻 Installation et Démarrage

Pour lancer le projet localement, suivez ces étapes :

### Prérequis
* Java JDK 17+
* Maven
* MySQL (via Laragon ou installé séparément)

### Étapes

1.  **Cloner le dépôt :**
    ```bash
    git clone [https://github.com/votre-username/AmmaExpress.git](https://github.com/votre-username/AmmaExpress.git)
    cd AmmaExpress
    ```

2.  **Configuration de la Base de Données :**
    * Créez une base de données nommée `ammaexpress_db` dans MySQL.
    * Mettez à jour le fichier `src/main/resources/application.properties` :
        ```properties
        spring.datasource.url=jdbc:mysql://localhost:3306/ammaexpress_db
        spring.datasource.username=root
        spring.datasource.password=votre_mot_de_passe
        ```

3.  **Lancer l'application :**
    ```bash
    mvn spring-boot:run
    ```

4.  **Accès :**
    * Ouvrez votre navigateur sur `http://localhost:8080`.

---

## 👥 Auteurs et Remerciements

**Réalisé par :**
* **Amyra Mouhib**
* **Manal Ejjebli**

**Encadré par :**
* **Dr. Samya Bouhaddour**

*Nous tenons à remercier l'EMSI et notre encadrante pour leur soutien tout au long de la réalisation de ce projet.*

---

## 📄 Licence
Ce projet a été réalisé dans un cadre académique.
