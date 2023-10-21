# CESI-Projet-Algo-Avancée-2022
Projet scolaire A3 - Algorithmique avancée (Python)

# Simulated Annealing pour le problème du voyageur de commerce

Ce notebook utilise l'approche de "Simulated Annealing" pour résoudre le problème du voyageur de commerce (TSP). L'idée est de trouver le chemin le plus court pour visiter un ensemble de villes sans passer deux fois par la même ville.

## Variables :
- **city_name**: Dictionnaire des noms de villes avec leurs indices.
- **external_dataset**: Utilisation d'une base de données externe.
- **namefile**: Nom du fichier de base de données externe.
- **n**: Utilisation d'une température linéaire.
- **nb_iterations**: Nombre d'itérations.
- ... [autres paramètres comme **nb_cities**, **max_xy**, etc.]

## Fonctions :

### Génération de villes :
- **generate_cities_randomly**: Génère aléatoirement des villes.
- **generate_cities_by_csv**: Importe les villes depuis un fichier CSV.

### Distance :
- **distance_between_cities**: Calcule la distance entre deux villes.
- **global_distance**: Calcule la distance totale d'une tournée.

### Température :
- **linear_temperature**: Génère une température linéaire.
- **dynamic_temperature**: Modifie la température de manière dynamique.

### Affichage :
- **live_plot**: Affiche un graphique en direct.
- **plot_history**: Affiche l'historique des distances.
- **explain_tour**: Détaille une tournée.
- **display_truck**: Affiche la division en camions.

- **report**: Ecrit dans un fichier de rapport.

### Simulated Annealing :
- **metaheuristic**: La fonction principale qui effectue l'algorithm de "Simulated Annealing" pour trouver la meilleure tournée.

## Simulated Annealing :

L'algorithme commence par générer une tournée aléatoire. Pour chaque température, il effectue un certain nombre de modifications sur la tournée actuelle. Si la nouvelle tournée a une distance inférieure, elle est acceptée. Sinon, elle est acceptée avec une certaine probabilité. L'objectif est d'éviter de rester coincé dans un optimum local.

---

## Pour utiliser ce notebook :
1. Assurez-vous d'avoir toutes les dépendances nécessaires installées.
2. Exécutez le code pour initialiser les fonctions et les variables.
3. Utilisez la fonction **metaheuristic** pour démarrer l'algorithme.
4. Vous pouvez afficher et analyser les résultats grâce aux fonctions d'affichage.

