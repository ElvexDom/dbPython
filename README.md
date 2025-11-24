# Exercice SQLAlchemy avec SQLite

## Objectif

Cet exercice consiste à manipuler une base de données SQLite à l’aide de Python et SQLAlchemy. Les opérations incluent :

1. Exécuter des requêtes SELECT et afficher les résultats.
2. Insérer de nouvelles lignes dans une table (`actor`).
3. Mettre à jour des données existantes conditionnellement.
4. Calculer des statistiques sur une table (`film`).

Une seule fonction `executer_query` est utilisée pour gérer **toutes les requêtes SQL** (SELECT, INSERT, UPDATE, DELETE).

---

## Prérequis

* Python 3.11 ou supérieur
* Bibliothèques Python :

  * `sqlalchemy`
  * `pandas`
  * `tabulate`
* Base SQLite `sakila.db`

Installation des dépendances :

```bash
pip install -r requirements.txt
```

### requirements.txt

```
sqlalchemy
pandas
tabulate
```

---

## Contenu du script

### 1️⃣ Connexion à la base SQLite
### 2️⃣ Fonction unique `executer_query`
### 3️⃣ Afficher les 5 titres de films
### 4️⃣ Statistiques sur la durée des films
### 5️⃣ Insertion d’un nouvel acteur
### 6️⃣ Modification conditionnelle d’un acteur

---

## Points clés

* Utilisation d’une seule fonction `executer_query` pour toutes les requêtes SQL.
* Vérification de l’existence avant insertion ou mise à jour pour éviter les doublons.
* Utilisation de `datetime.now().strftime("%Y-%m-%d %H:%M:%S")` pour `last_update`.
* Affichage des résultats avec `pandas` pour un rendu clair.

---

## Résultat attendu

* Affichage des 5 premiers titres de films.
* Statistiques sur la durée des films.
* Insertion d’un acteur si inexistant.
* Modification
