# 📊 Exploration des Données Commerciales : Tableau de Bord Power BI

## 1-Présentation:
Ce projet est un tableau de bord interactif réalisé avec Power BI pour explorer les données commerciales d’une entreprise sur les années 2020 et 2021. Il permet d’analyser les ventes sous différents angles (géographique, produits, boutiques…) et d’identifier des tendances clés.

## 2- Objectifs du projet:
- Nettoyer et transformer les données pour les rendre exploitables.
- Créer des mesures pertinentes (Chiffre d’Affaires, Nombre de Ventes, Remises…).
- Construire des visualisations interactives et intuitives.
- Comparer les performances commerciales entre les deux années.


## Structure des données et transformations effectuées

### 1. Tables et transformations appliquées

#### Table Boutique :
  - Conversion des colonnes idBoutique et idGeographique en format texte.
  - Remplacement des champs vides dans la colonne status par “open”.

    
#### Table Catégorie Produits :
  - Conversion de idCategorieProduit en format texte.

#### Table Géographie :
  - Conversion de idGeographie en format texte.

#### Table Produit :
  - Conversion des colonnes idProduit et idSousCategorieProduit en format texte.
	- Conversion des colonnes coût unitaire et prix unitaire en nombre décimal fixe.

#### Table SousCategorieProduits :
  - Conversion des colonnes idSousCategorieProduits et idCategorieProduit en format texte.

#### Table Ventes :
  - Importation des fichiers CSV de chaque trimestre des années 2020 et 2021.
	-	Fusion des fichiers CSV en une seule table.
	-	Suppression des colonnes inutiles (idPromotion, montant de retour, coût total, etc.).
	-	Conversion des colonnes idVente, idBoutique et idProduit en format texte.

### 2. Création de mesures et de tables

#### Table DateTable
  -  Ajout d’une table de dates avec les colonnes : année, date, jour, mois, numéro du mois et trimestre pour faciliter l’analyse temporelle.

#### Mesures ajoutées
  - Nb Boutique → Nombre total de boutiques.
	-	PaysSelected → Mesure permettant de filtrer les données par pays.
	-	Nb Produit → Nombre total de produits.
	-	CA → Chiffre d’Affaires.
	-	CA-1 → Chiffre d’Affaires de l’année précédente.
	-	Nb Vente → Nombre total de ventes.
	-	Montant Vente → Somme des ventes.
	-	Montant Vente après remise → Somme des ventes après application des remises.
	-	Remise → Montant total des remises accordées.

⸻

## 📊 Visualisations disponibles dans le tableau de bord

- Carte interactive des boutiques par pays et statut.
- Nombre de ventes par boutique et par catégorie de produit.
- Répartition des produits par catégorie et sous-catégorie.
- Évolution du chiffre d’affaires et comparaison avec l’année précédente.
- Impact des remises sur les ventes.

⸻

### Comment utiliser ce projet ?

#### 1. Télécharger le fichier Power BI
##### 1. Clone ce dépôt GitHub :
        git clone https://github.com/elmotchou/Tableau-bord-Power-BI.git
##### 2. Ouvre le fichier .pbix avec Power BI Desktop.

#### 2. Explorer le tableau de bord
  - Utilise les filtres pour analyser les ventes par année, trimestre, mois ou pays.
	-	Consulte les cartes et graphiques interactifs pour une meilleure compréhension des tendances.
