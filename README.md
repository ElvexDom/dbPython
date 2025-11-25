# Exercice SQLAlchemy avec SQLite

## Objectif

Cet exercice consiste à manipuler une base de données SQLite à l’aide de Python et SQLAlchemy. Les opérations incluent :

1. Exécuter des requêtes SELECT et afficher les résultats.
2. Insérer de nouvelles lignes dans une table (`actor`).
3. Mettre à jour des données existantes conditionnellement.
4. Calculer des statistiques sur une table (`film`).
5. Visualiser des données avec des graphiques.

Une seule fonction est utilisée pour gérer toutes les requêtes SQL.

---

## Prérequis

* Python 3.11 ou supérieur
* Bibliothèques Python :

  * `sqlalchemy`
  * `pandas`
  * `tabulate`
  * `seaborn`
  * `matplotlib`

---

## Contenu de l’exercice

### 1️⃣ Connexion à la base SQLite

Se connecter à la base de données SQLite via SQLAlchemy.

### 2️⃣ Fonction unique pour exécuter les requêtes

Une seule fonction gère toutes les requêtes SQL (SELECT, INSERT, UPDATE, DELETE) avec gestion des exceptions.

### 3️⃣ Afficher les 5 titres de films

Afficher les 5 premiers titres de films dans l’ordre alphabétique.

### 4️⃣ Statistiques sur la durée des films

Calculer la durée moyenne, minimum, maximum, le nombre total et la somme des durées des films.

### 5️⃣ Insertion d’un nouvel acteur

Insérer un acteur si celui-ci n’existe pas déjà, en calculant automatiquement un nouvel ID et en ajoutant la date/heure actuelle.

### 6️⃣ Modification conditionnelle d’un acteur

Modifier le prénom d’un acteur existant en ciblant son ID unique et mettre à jour la date/heure.

### 7️⃣ Visualisation des données

#### Histogramme des `rental_rate`

Visualiser la distribution des tarifs de location des films.

#### Barplot de la durée moyenne par classification (`rating`)

Comparer visuellement la durée moyenne des films selon leur classification avec un graphique en barres.

---

## Points clés

* Utilisation d’une seule fonction pour toutes les requêtes SQL.
* Vérification de l’existence avant insertion ou mise à jour pour éviter les doublons.
* Utilisation de la date/heure actuelle pour `last_update`.
* Visualisation des données pour mieux comprendre la distribution et comparer les catégories.

---

## Résultat attendu

* Affichage des 5 premiers titres de films.
* Statistiques sur la durée des films.
* Insertion d’un acteur si inexistant.
* Modification d’un acteur ciblé par ID.
* Histogramme des tarifs de location.
* Barplot des durées moyennes par classification.
