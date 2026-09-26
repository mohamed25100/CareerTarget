# 🎯 CareerTarget

> Application web full-stack permettant de centraliser et suivre les métiers, formations, entreprises et opportunités professionnelles ciblées.

**CareerTarget** est un projet personnel développé dans le but de faciliter la recherche d'emploi, d'alternance, de stage et de formations.

L'application permet de centraliser les informations importantes concernant les **métiers ciblés**, les **formations**, les **entreprises** et les **candidatures**, tout en offrant une interface permettant de suivre l'avancement des démarches.

---

## 📸 Aperçu

> Les captures d'écran seront ajoutées après le développement de l'interface.

### Dashboard

![Dashboard](docs/screenshots/dashboard.png)

### Métiers

![Métiers](docs/screenshots/metiers.png)

### Formations

![Formations](docs/screenshots/formations.png)

### Entreprises

![Entreprises](docs/screenshots/entreprises.png)

### Candidatures

![Candidatures](docs/screenshots/candidatures.png)

---

# 🚀 Fonctionnalités

## 👨‍💻 Gestion des métiers

L'application permet de gérer les métiers ciblés.

Fonctionnalités :

* Ajouter un métier
* Modifier un métier
* Supprimer un métier
* Consulter les détails d'un métier
* Rechercher un métier
* Filtrer par domaine
* Associer des technologies à un métier
* Ajouter une description
* Ajouter un niveau d'expérience
* Ajouter un type de contrat recherché

Exemples :

* Développeur Java
* Développeur Full Stack
* Développeur Angular
* Développeur C#
* Data Engineer
* Développeur Backend

---

# 🎓 Gestion des formations

L'application permet de centraliser les formations et établissements ciblés.

Fonctionnalités :

* Ajouter une formation
* Modifier une formation
* Supprimer une formation
* Consulter une formation
* Rechercher une formation
* Ajouter l'établissement
* Ajouter le niveau de formation
* Ajouter le coût
* Ajouter la localisation
* Ajouter le type de formation
* Ajouter un lien vers la formation
* Ajouter des notes personnelles

Exemples :

* Master Informatique
* Mastère Full Stack
* Mastère Développement
* POEI
* Formation professionnelle
* Formation en alternance

---

# 🏢 Gestion des entreprises

L'application permet de gérer les entreprises ciblées.

Fonctionnalités :

* Ajouter une entreprise
* Modifier une entreprise
* Supprimer une entreprise
* Consulter les informations
* Rechercher une entreprise
* Ajouter le secteur d'activité
* Ajouter la localisation
* Ajouter le site internet
* Ajouter le lien LinkedIn
* Ajouter des technologies utilisées
* Ajouter des notes

---

# 📩 Gestion des candidatures

Une candidature peut être associée à une entreprise et à un métier.

### Statuts disponibles

```text
À contacter
Candidature à préparer
Candidature envoyée
En attente
Entretien
Test technique
Relance
Refus
Accepté
```

Informations enregistrées :

* Entreprise
* Métier
* Formation éventuelle
* Type de contrat
* Date de candidature
* Date de relance
* Statut
* Lien vers l'offre
* Salaire
* Localisation
* Télétravail
* Notes

---

# 🔎 Recherche et filtres

L'application propose plusieurs outils de recherche.

### Recherche

Recherche par :

* nom
* entreprise
* métier
* formation
* technologie
* localisation

### Filtres

Exemples :

```text
Type de contrat
├── CDI
├── CDD
├── Alternance
├── Stage
└── Immersion
```

```text
Statut
├── À contacter
├── Envoyée
├── Entretien
├── Relance
├── Refus
└── Acceptée
```

---

# 📊 Dashboard

Le tableau de bord permet d'avoir une vision globale des recherches.

Exemple :

```text
┌──────────────────────────────────────┐
│           CAREERTARGET               │
├──────────────────────────────────────┤
│                                      │
│  Métiers ciblés          12          │
│  Formations               8          │
│  Entreprises             35          │
│  Candidatures            24          │
│                                      │
├──────────────────────────────────────┤
│ Candidatures                         │
│                                      │
│ 🟡 En attente             8          │
│ 🔵 Entretiens             4          │
│ 🟠 Relances               5          │
│ 🔴 Refus                  6          │
│ 🟢 Acceptées              1          │
│                                      │
└──────────────────────────────────────┘
```

Le dashboard pourra également afficher :

* nombre de candidatures
* nombre d'entretiens
* nombre de réponses
* nombre de refus
* candidatures récentes
* prochaines relances
* technologies les plus recherchées

---

# 🏗️ Architecture

Le projet utilise une architecture séparant le frontend et le backend.

```text
                    ┌─────────────────────┐
                    │      Utilisateur     │
                    └──────────┬──────────┘
                               │
                               ▼
                    ┌─────────────────────┐
                    │       Angular       │
                    │     Frontend        │
                    └──────────┬──────────┘
                               │
                         HTTP / REST
                               │
                               ▼
                    ┌─────────────────────┐
                    │    Spring Boot      │
                    │      Backend        │
                    └──────────┬──────────┘
                               │
                               ▼
                    ┌─────────────────────┐
                    │      MariaDB        │
                    │      Database       │
                    └─────────────────────┘
```

---

# 🧰 Technologies utilisées

## Frontend

* Angular
* TypeScript
* HTML5
* CSS3
* Angular Router
* Angular HttpClient
* Reactive Forms

## Backend

* Java
* Spring Boot
* Spring Web
* Spring Data JPA
* Spring Security
* API REST
* Maven

## Base de données

* MariaDB
* SQL
* Hibernate / JPA

## Authentification

* Spring Security
* JWT

## Outils

* Git
* GitHub
* Visual Studio Code
* IntelliJ IDEA
* Postman
* HeidiSQL

---

# 📁 Structure du projet

```text
CareerTarget/
│
├── frontend/
│   ├── src/
│   │   ├── app/
│   │   │   ├── components/
│   │   │   ├── pages/
│   │   │   ├── services/
│   │   │   ├── models/
│   │   │   ├── guards/
│   │   │   └── interceptors/
│   │   │
│   │   ├── assets/
│   │   └── environments/
│   │
│   ├── angular.json
│   ├── package.json
│   └── README.md
│
├── backend/
│   ├── src/
│   │   ├── main/
│   │   │   ├── java/
│   │   │   │   └── com/careertarget/
│   │   │   │       ├── controller/
│   │   │   │       ├── service/
│   │   │   │       ├── repository/
│   │   │   │       ├── entity/
│   │   │   │       ├── dto/
│   │   │   │       ├── security/
│   │   │   │       └── exception/
│   │   │   │
│   │   │   └── resources/
│   │   │       └── application.properties
│   │   │
│   │   └── test/
│   │
│   └── pom.xml
│
├── docs/
│   └── screenshots/
│
├── .gitignore
└── README.md
```

---

# 🗄️ Modèle de données

Les principales entités sont :

```text
User
 │
 └── Candidature
       │
       ├── Entreprise
       │
       ├── Métier
       │
       └── Formation
```

### Entités principales

```text
User
├── id
├── username
├── email
└── password

Metier
├── id
├── nom
├── domaine
├── description
├── niveauExperience
└── technologies

Formation
├── id
├── nom
├── organisme
├── niveau
├── prix
├── localisation
├── type
└── url

Entreprise
├── id
├── nom
├── secteur
├── localisation
├── siteWeb
├── linkedin
└── description

Candidature
├── id
├── entreprise
├── metier
├── formation
├── typeContrat
├── statut
├── dateCandidature
├── dateRelance
├── salaire
├── localisation
├── teletravail
├── urlOffre
└── notes
```

---

# 🔌 API REST

## Métiers

```http
GET    /api/metiers
GET    /api/metiers/{id}
POST   /api/metiers
PUT    /api/metiers/{id}
DELETE /api/metiers/{id}
```

## Formations

```http
GET    /api/formations
GET    /api/formations/{id}
POST   /api/formations
PUT    /api/formations/{id}
DELETE /api/formations/{id}
```

## Entreprises

```http
GET    /api/entreprises
GET    /api/entreprises/{id}
POST   /api/entreprises
PUT    /api/entreprises/{id}
DELETE /api/entreprises/{id}
```

## Candidatures

```http
GET    /api/candidatures
GET    /api/candidatures/{id}
POST   /api/candidatures
PUT    /api/candidatures/{id}
DELETE /api/candidatures/{id}
```

---

# 🔐 Sécurité

L'application utilise Spring Security pour sécuriser les endpoints.

L'authentification est basée sur des tokens JWT.

```text
Utilisateur
     │
     │ Login
     ▼
Spring Security
     │
     │ JWT
     ▼
Frontend Angular
     │
     │ Authorization: Bearer TOKEN
     ▼
API REST
```

Les utilisateurs non authentifiés ne peuvent pas accéder aux fonctionnalités protégées.

---

# 🧪 Tests

Le projet prévoit plusieurs niveaux de tests.

### Backend

* Tests unitaires
* Tests des services
* Tests des contrôleurs
* Tests des repositories

### Frontend

* Tests des services
* Tests des composants
* Tests des formulaires

### API

Les endpoints peuvent être testés avec Postman.

---

# 🚀 Installation

## Prérequis

Installer :

* Java 17 ou supérieur
* Node.js
* npm
* Angular CLI
* Maven
* MariaDB
* Git

---

## 1. Cloner le projet

```bash
git clone https://github.com/VOTRE-USERNAME/CareerTarget.git

cd CareerTarget
```

---

# 2. Configuration de la base de données

Créer une base MariaDB :

```sql
CREATE DATABASE careertarget;
```

Configurer ensuite le fichier :

```text
backend/src/main/resources/application.properties
```

Exemple :

```properties
spring.datasource.url=jdbc:mariadb://localhost:3306/careertarget
spring.datasource.username=root
spring.datasource.password=YOUR_PASSWORD

spring.jpa.hibernate.ddl-auto=update
spring.jpa.show-sql=true
```

> Ne jamais publier les vrais mots de passe dans GitHub.

---

# 3. Lancer le backend

```bash
cd backend

./mvnw spring-boot:run
```

Sous Windows :

```bash
mvnw.cmd spring-boot:run
```

Backend disponible sur :

```text
http://localhost:8080
```

---

# 4. Lancer le frontend

Dans un autre terminal :

```bash
cd frontend

npm install

ng serve
```

Frontend disponible sur :

```text
http://localhost:4200
```

---

# ☁️ Déploiement

L'objectif du projet est de disposer d'une version accessible en ligne.

Architecture de production :

```text
Internet
   │
   ├───────────────┐
   ▼               ▼
Frontend        Backend
Angular         Spring Boot
   │               │
   │               ▼
   │            MariaDB
   │
   └────── API REST ──────►
```

Les variables sensibles doivent être configurées avec des variables d'environnement.

Exemple :

```text
DATABASE_URL
DATABASE_USERNAME
DATABASE_PASSWORD
JWT_SECRET
```

---

# 📌 Roadmap

## Version 1.0

* [x] Création du repository
* [ ] Architecture frontend
* [ ] Architecture backend
* [ ] Base de données
* [ ] CRUD Métiers
* [ ] CRUD Formations
* [ ] CRUD Entreprises
* [ ] CRUD Candidatures
* [ ] Recherche
* [ ] Filtres
* [ ] Dashboard
* [ ] Authentification
* [ ] Tests
* [ ] Déploiement

## Version 2.0

* [ ] Notifications de relance
* [ ] Export CSV
* [ ] Export PDF
* [ ] Dark mode
* [ ] Statistiques avancées
* [ ] Historique des candidatures
* [ ] Système de favoris
* [ ] Recherche avancée
* [ ] Import d'offres
* [ ] PWA / application mobile

---

# 🎯 Objectifs du projet

Ce projet a plusieurs objectifs :

### Technique

Mettre en pratique :

* Java
* Spring Boot
* Spring Security
* API REST
* Angular
* TypeScript
* SQL
* MariaDB
* Git
* GitHub
* déploiement cloud

### Professionnel

Créer un projet concret permettant de démontrer :

* la capacité à concevoir une application full-stack
* la conception d'une base de données
* le développement d'une API REST
* l'intégration frontend/backend
* la sécurisation d'une application
* la gestion d'un projet de bout en bout
* le déploiement d'une application web

---

# 💼 Projet Portfolio

CareerTarget est également conçu comme un projet portfolio.

L'objectif est de présenter une application complète allant de la conception jusqu'au déploiement.

Le projet permet notamment de démontrer les compétences suivantes :

```text
Conception
    ↓
Base de données
    ↓
Backend Java / Spring Boot
    ↓
API REST
    ↓
Frontend Angular
    ↓
Authentification
    ↓
Tests
    ↓
Git / GitHub
    ↓
Déploiement
```

---

# 📚 Compétences développées

| Domaine         | Compétences                        |
| --------------- | ---------------------------------- |
| Backend         | Java, Spring Boot, Spring Data JPA |
| API             | REST, JSON, HTTP                   |
| Sécurité        | Spring Security, JWT               |
| Frontend        | Angular, TypeScript                |
| Base de données | MariaDB, SQL                       |
| Architecture    | MVC, séparation frontend/backend   |
| Tests           | JUnit, tests API                   |
| Versioning      | Git, GitHub                        |
| Déploiement     | Hébergement cloud                  |
| Documentation   | README, documentation API          |

---

# 👨‍💻 Auteur

**Mohamed Boucherba**

Développeur Java / Angular

Projet personnel réalisé dans le cadre du développement de compétences en développement full-stack.

---

# 📄 Licence

Ce projet est destiné à un usage personnel et pédagogique.

Une licence pourra être ajoutée ultérieurement selon les conditions de publication du projet.

---

# ⭐ Conclusion

CareerTarget est une application full-stack développée pour centraliser et suivre les opportunités professionnelles et de formation.

Le projet met en pratique une architecture moderne :

**Angular + Spring Boot + Spring Security + MariaDB + API REST + GitHub + Déploiement**

L'objectif final est de disposer d'une application fonctionnelle, documentée et accessible en ligne pouvant servir de **projet portfolio**.
