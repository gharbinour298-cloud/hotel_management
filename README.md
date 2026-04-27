#  Hotel Management Web Application (PHP MVC)

## Description du projet

Cette application est un projet de gestion d’hôtel développé en **PHP**, utilisant l’architecture **MVC (Model-View-Controller)**, **MySQL**, **PDO**, et la gestion des sessions.

Le système permet la gestion complète d’un hôtel avec deux espaces distincts :
- **Espace Administrateur**
- **Espace Client**

---

## Objectifs 

- Créer une application web dynamique avec PHP & MySQL
- Appliquer le pattern MVC
- Utiliser la Programmation Orientée Objet (POO)
- Gérer l’authentification sécurisée avec sessions
- Manipuler une base de données avec PDO
- Gérer l’upload de fichiers (images des chambres)
- Utiliser l’IA de manière critique dans le développement

---

##  Technologies utilisées

- PHP 8+
- MySQL 
- PDO 
- HTML5 / CSS3
- JavaScript 
- XAMPP (Apache local server)

---

##  Architecture du projet

Le projet suit une architecture MVC :


app/
├── controllers/ → Logique métier
├── models/ → Accès base de données + entités
├── views/ → Interface utilisateur
config/ → Configuration DB
public/ → Point d’entrée (index.php)
uploads/ → Images des chambres
database/ → Scripts SQL


---

## Fonctionnalités

### Authentification
- Connexion administrateur
- Connexion client
- Inscription client
- Sessions sécurisées

---

###  Admin
- Gestion des clients (CRUD)
- Gestion des chambres (CRUD + upload image)
- Gestion des réservations
- Recherche et filtrage des réservations

---

### Client
- Inscription / Connexion
- Consultation des chambres disponibles
- Réservation de chambre
- Consultation de ses réservations

---

## Base de données

Tables principales :
- `users` (administrateurs)
- `clients`
- `rooms`
- `reservations`

Relations :
- Un client peut avoir plusieurs réservations
- Une chambre peut être réservée plusieurs fois (avec contrôle de dates)

---

## Sécurité

- PDO avec requêtes préparées
- Hashage des mots de passe (`password_hash`)
- Vérification avec `password_verify`
- Protection CSRF (formulaires critiques)
- Séparation des sessions admin/client
- Validation des données serveur

---

## Installation

### 
1. Cloner le projet
```bash
git clone https://github.com/gharbinour298-cloud/hotel_management/tree/main
2. Placer dans XAMPP
htdocs/Hotel-managment-php
3. Démarrer Apache & MySQL
4. Importer la base de données

Importer :
database/hotel_management.sql
database/seed.sql
5. Configurer la base de données

Modifier :
config/config.php
 Accès au projet
Application locale :
http://localhost/Hotel-managment-php/public/index.php
 Comptes de test
Admin :
Email: admin@example.com
Password: admin123
Client :

Créer un compte via inscription

 Fonctionnalités avancées
Gestion des statuts de chambres (available / booked)
Upload sécurisé des images
Séparation stricte admin / client
Architecture MVC propre et modulaire
 Utilisation de l’IA

L’intelligence artificielle a été utilisée pour :

Comprendre certaines structures MVC
Corriger des erreurs logiques
Optimiser la gestion des réservations
Améliorer la sécurité (sessions, CSRF, validation)

Toutes les suggestions ont été analysées et adaptées manuellement au projet

 Améliorations futures
Ajout de pagination
Système de notifications email
Dashboard statistique
API REST
Amélioration UI/UX
Système de rôles avancés

 Auteur 
Projet réalisé par Eya Medhioub et Nour Gharbi dans un cadre académique 
 
