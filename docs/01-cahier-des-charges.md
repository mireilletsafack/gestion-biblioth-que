# 📚 Cahier des charges fonctionnel – Projet MyBookShelf

## 🧭 Objectif du projet

Créer une application de gestion de bibliothèque personnelle permettant de suivre les livres lus ou à lire, d’ajouter des commentaires, et de rechercher efficacement parmi les livres.

---

## 🔧 Fonctionnalités principales de l’application

### 📘 Gestion des livres
- Ajouter un livre : titre, auteur, année, genre, statut (lu / à lire)
- Modifier un livre existant
- Supprimer un livre
- Lister tous les livres

### 🔍 Recherche et filtres
- Rechercher par titre ou auteur
- Filtrer par genre
- Filtrer par statut (lu / à lire)

### 📝 Notes personnelles
- Ajouter un commentaire à un livre
- Modifier ou supprimer un commentaire

### 📤 Export
- Exporter la liste des livres au format JSON
- (Optionnel) Export CSV

---

## 👤 Utilisateur cible
- Un utilisateur unique (pas de gestion multi-compte)
- Utilisation via une interface API (Postman ou Swagger)

---

## 📋 Cas d’usage (User Stories)

### US01 – Ajouter un livre
> En tant qu’utilisateur, je veux ajouter un livre avec ses informations pour enrichir ma bibliothèque.

### US02 – Modifier les informations d’un livre
> En tant qu’utilisateur, je veux modifier les données d’un livre pour corriger ou mettre à jour ses détails.

### US03 – Rechercher un livre
> En tant qu’utilisateur, je veux rechercher un livre par titre, auteur ou genre pour le retrouver rapidement.

### US04 – Marquer un livre comme lu
> En tant qu’utilisateur, je veux changer le statut d’un livre pour suivre ma progression de lecture.

### US05 – Ajouter une note personnelle
> En tant qu’utilisateur, je veux écrire un commentaire personnel sur un livre pour m’en souvenir.

### US06 – Exporter ma bibliothèque
> En tant qu’utilisateur, je veux exporter ma liste de livres pour l’imprimer ou l’utiliser ailleurs.

---

## ✅ Critères d’acceptation (exemples)

| ID | Fonctionnalité | Critère |
|----|----------------|---------|
| CA01 | Ajouter un livre | Tous les champs obligatoires doivent être renseignés |
| CA02 | Rechercher un livre | La recherche doit être insensible à la casse |
| CA03 | Export JSON | Le fichier exporté contient tous les livres actuels |
| CA04 | Supprimer un livre | Le livre est retiré de la liste et n'apparaît plus à l'export |

---

## 🛠 Technologies envisagées

| Côté technique | Choix |
|----------------|-------|
| Backend | ASP.NET Core Web API |
| Base de données | SQLite ou PostgreSQL |
| Test manuel | Postman, XMind, tableur Excel |
| Test automatisé | xUnit, SpecFlow (optionnel) |
| CI/CD | GitHub Actions |
| Qualité code | SonarCloud (optionnel) |

---

## 📌 Livrables QA prévus

- Cahier de test manuel (scénarios + résultats)
- Tests automatisés API (unitaires + intégration)
- Rapport d'exécution
- README explicatif
