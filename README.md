# athletes-paris2024

<img width="256" alt="Screenshot 2024-11-23 at 11 13 34" src="https://github.com/user-attachments/assets/017ba419-8e93-49c5-ba62-d076d540ea53">


Ces scripts et codes ont été produits pour constituer un jeu de données brut et propre ([_tidy_](https://blog.avanci.fr/tidy-data-le-concept-de-donnees-propres)) sur les athlètes des Jeux Olympiques de Paris 2024. Ils ont été pensés pour permettre l'organisation d'un datasprint pédagogique, organisé par [Réseau Canopé](https://www.reseau-canope.fr/) avec [l'académie de Créteil](https://www.linkedin.com/company/academie-de-creteil/). 

## Les différents éléments que vous trouverez dans ce repo : 

1. Le script pour [scraper](https://fr.wikipedia.org/wiki/Web_scraping) la [page du site officiel](https://olympics.com/fr/paris-2024/athletes) du CIO sur les athlètes ayant participé aux JO de Paris 2024. Ce script doit être copié-collé dans [webscraper.io]() (outil no-code, qui s'installe comme une extension sur votre navigateur).
**En sortie : un jeu de données brut**

2. Les notebooks (dans le dossier `notebook`) qui vont permettre de nettoyer les données brutes. Chaque notebook s'occupe d'un certain nombre d'étapes de traitement, chaque étape venant ajouter une dimension/variable d'intérêt au jeu de données. **En sortie : un jeu de données brut et propre**

3. Le jeux de données (dans le dossier `data`):
* Brut: `2.0_complete_olympics_athlete.csv`
* Brut et propre: `paris_olympians_data`

   
## Variables du jeu de données 

* nom : nom de l'athlète
* lien_vers_biographie-href : lien vers la page de biographie du CIO
* discipline : discipline sportive lors des JO
* naissance : date de naissance
* pays : nationalité
* cleaned_age : age
* cleaned_fonction : rôle (`Athlète` ou `Athlète remplaçant`)
* cleaned_taille : taille en cm
* cleaned_sexe : sexe (`Homme`ou `Femme`)
* competition_site : site(s) sur lesquels les athlètes ont concourru (nom du site ou si les athlètes ont concurru sur plusieurs sites : `multi-sites`)
* competition_count : nombre de compétitions auxquelles ils ont participé (par exemple, Léon Marchant a participé à 14 compétition, incluant les séries, demi-finales et finales)
* first_date : date de la première compétition à laquelle un athlète a participé
* last_date : date de la dernière compétition à laquelle un athlète a participé
* unique_competition_days : nombre de jours de compétition
* nombre_or : nombre de médailles d'or
* nombre_argent : nombre de médailles d'argent
* nombre_bronze : nombre de médailles de bronze
* record_olympique_count : nombre de records olympiques battus lors des JO
* record_monde_count : nombre de records du monde battus lors des JO

