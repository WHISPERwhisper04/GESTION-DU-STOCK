# Gestion de stock

Ce programme permet de gérer une liste de produits avec différentes fonctionnalités telles que l'ajout, la modification, la suppression, l'affichage, la recherche et le tri des produits.

## Fonctions disponibles

### 1. `ouvrir_fichier(FILE **fichier, const char *mode)`

Cette fonction ouvre le fichier de données des produits en mode lecture ou lecture/écriture. Si le fichier n'existe pas, il est créé.

### 2. `LoadProductFromFile(FILE *fichier, Produit *T, int *n, int *lastId)`

Charge les produits à partir du fichier dans un tableau de structures de type Produit. Met à jour le nombre de produits chargés et l'ID le plus élevé.

### 3. `SaveProductToFile(FILE *fichier, Produit *T, int n)`

Sauvegarde les produits depuis un tableau de structures de type Produit dans le fichier.

### 4. `ajouter_produit(FILE *fichier, int *lastId, int *n, Produit *P, char *nomUtilisateur)`

Ajoute un nouveau produit à la liste en demandant les détails à l'utilisateur et les sauvegarde dans le fichier.

### 5. `modifier_produit(FILE *fichier, Produit *produits, int nb_produits)`

Permet à l'utilisateur de modifier les détails d'un produit existant dans la liste.

### 6. `supprimer_produit(FILE *fichier, Produit *produits, int *nb_produits)`

Supprime un produit de la liste en demandant l'ID du produit à supprimer.

### 7. `afficher_produits(FILE *fichier)`

Affiche la liste de tous les produits avec leurs détails.

### 8. `rechercher_produit_par_utilisateur(FILE *fichier, const char *nomUtilisateur)`

Affiche les produits appartenant à un utilisateur spécifique.

### 9. `rechercher_produit_par_nom(FILE *fichier, const char *nomProduit)`

Affiche les produits avec un nom spécifique.

### 10. `trier_produits_par_nom(FILE *fichier, Produit *produits, int *nb_produits, int *lastId)`

Trie les produits par leur nom dans l'ordre alphabétique.

### 11. `trier_produits_par_prix_unitaire(FILE *fichier, Produit *produits, int *nb_produits, int *lastId)`

Trie les produits par leur prix unitaire du moins cher au plus cher.

## Utilisation

Le programme permet à l'utilisateur de choisir parmi plusieurs options pour gérer les produits, telles que l'ajout, la modification, la suppression, l'affichage, la recherche et le tri des produits. Les actions sont effectuées en fonction des autorisations de l'utilisateur.

## Installation

1. Clonez le dépôt sur votre machine locale.
2. Compilez le programme à l'aide de votre compilateur C de choix.
3. Exécutez le programme en lançant l'exécutable généré.

## Configuration

Vous pouvez modifier le nom du fichier de données des produits dans le code source si nécessaire. Par défaut, le nom du fichier est `PRODUITS.txt`.

## Contributions

Les contributions sont les bienvenues ! Si vous souhaitez contribuer à ce projet, veuillez forker le dépôt, effectuer vos modifications et soumettre une demande de tirage.
