# Collection Legami

Petite page web personnelle pour suivre une collection de stylos effaçables Legami (« Erasable – The Real Ones »). Un seul fichier HTML, sans installation ni serveur.

> Site personnel non officiel, non affilié à Legami. Les photos appartiennent à Legami.

## Utilisation

1. Ouvrir `legami.html` dans un navigateur.
2. À la première ouverture, saisir le prénom du premier enfant.
3. Pour chaque stylo, cliquer sur :
   - **✓ J'ai** : le stylo est dans la collection ;
   - **♡ J'aimerais** : le stylo est ajouté à la liste d'envie (le cœur devient ♥). Cliquer à nouveau pour décocher.

## Fonctions

- **Plusieurs enfants** (jusqu'à 10), chacun avec son propre inventaire : `＋ Enfant` pour ajouter, ✎ pour renommer, 🗑 pour supprimer.
- **Filtres** : Tous, Ma collection, Liste d'envie, À trier, plus un filtre par année et une recherche (nom, personnage, phrase, référence).
- **Statistiques** : progression, nombre de stylos, budget total de la collection.
- **🖨 Imprimer en PDF** : ouvre la fenêtre d'impression du navigateur, choisir « Enregistrer au format PDF ». Le PDF reprend le filtre affiché (par exemple la liste d'envie seule), en A4 sur 4 colonnes, avec l'état de chaque stylo et le prénom de l'enfant.
- **⬇ Sauvegarder / ⬆ Restaurer** : export et import de tous les inventaires dans un fichier `.json`. L'import accepte aussi les anciens CSV (un seul enfant), où « je n'ai pas » devient « J'aimerais ».

## Données

- Les coches sont enregistrées dans le navigateur (`localStorage`), sur cet appareil uniquement. Vider les données du navigateur les efface : penser à utiliser **Sauvegarder** régulièrement.
- La liste des stylos est intégrée dans le fichier. Si un `legami.xlsx` est présent à côté de la page servie en ligne (par exemple GitHub Pages), il est lu à la place.
- Les images sont cherchées dans un dossier `images/` à côté du fichier. Sans ce dossier, les fiches s'affichent avec une image pâle.

## Fichiers

| Fichier | Rôle |
|---|---|
| `legami.html` | La page, avec les données intégrées |
| `images/` | Photos des stylos (optionnel) |
| `legami.xlsx` | Données à jour (optionnel, mode en ligne) |
