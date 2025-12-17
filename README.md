# 💼 GestionSalaires-JavaFX-S7

**GestionSalaires-JavaFX** est une application de bureau robuste permettant de gérer les ressources humaines d'une entreprise. Elle automatise le calcul des salaires selon le type d'employé et assure la persistance des données via une base de données MySQL.

---

## 🚀 Fonctionnalités

- **Gestion CRUD complète** : Ajouter, modifier et supprimer des employés.
- **Typologie d'employés** : Gestion spécifique pour les *Vendeurs*, *Représentants*, *Producteurs* et *Manutentionnaires*.
- **Calcul automatisé** : Calcul des salaires en fonction des performances (chiffre d'affaires ou unités produites) et des primes de risque.
- **Interface intuitive** : Interface graphique moderne conçue avec **JavaFX** et **Scene Builder**.
- **Statistiques** : Affichage en temps réel du salaire moyen de l'entreprise.
- **Persistance** : Connexion JDBC avec MySQL pour sauvegarder les données.

---

## 🛠️ Technologies utilisées

* **Langage** : Java 11+
* **Interface Graphique** : JavaFX (FXML)
* **Base de données** : MySQL 8.0
* **Design** : Scene Builder
* **Gestionnaire de dépendances** : Maven (ou Gradle)

---

## 📂 Architecture du projet

Le projet suit une architecture structurée pour séparer la logique métier de l'interface :

```text
src/
 ├─ application/   # Point d'entrée de l'application (Main.java)
 ├─ controller/    # Logique de contrôle entre la View et le Model
 ├─ db/            # Gestion de la connexion et requêtes SQL (DAO)
 ├─ model/         # Classes métiers (Héritage et Polymorphisme)
 └─ view/          # Fichiers FXML et feuilles de style CSS
