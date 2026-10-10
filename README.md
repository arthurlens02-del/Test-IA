# Tonnerre · Boutique en ligne de démonstration

> Projet de démonstration : aucun paiement réel, aucun produit à livrer. Je voulais juste voir un exemple de ce que l'ia claude est capable de créer en quelques minutes . Test d'une fonctionnalité IA

Une boutique en ligne fictive de pédales d'effet pour guitare, créée pour mon portfolio. Elle montre l'expérience d'achat côté visiteur : parcourir un catalogue, voir un produit, remplir un panier.

**Voir le site :** https://claude.ai/artifact/JCKM4YMMnRf9ojHWebjMrL


## Fonctionnalités

- Catalogue de 8 produits avec filtres par type (Fuzz, Overdrive, Delay, Reverb, Modulation)
- Tri par prix croissant ou décroissant
- Fiche détaillée pour chaque produit (description, caractéristiques)
- Panier avec modification des quantités et suppression
- Total en euros et barre de progression vers la livraison offerte (dès 150 €)
- Panier conservé quand on recharge la page
- Alerte « plus que X en stock » pour les produits presque épuisés
- Mode clair et mode sombre
- Affichage adapté au téléphone et à l'ordinateur
- Accessibilité : navigation au clavier, fermeture avec Échap, respect de la préférence « réduire les animations »

## Technologies

- HTML, CSS et JavaScript, dans un seul fichier, sans framework
- Illustrations des produits en SVG générées par le code (aucune image à charger)
- `localStorage` pour mémoriser le panier et le thème
- Polices Google Fonts : Unbounded et Instrument Sans

## Lancer le projet

Aucune installation nécessaire. Télécharge `boutique.html` et ouvre-le dans ton navigateur.

## Modifier les produits

Les produits sont dans la liste `PRODUCTS` au début du script. Pour en ajouter un, copie un bloc existant et change :

```js
{ id: 9, name: "Mon produit", cat: "Fuzz", price: 99, color: "#e8452c",
  tint: "#f6c7bd", stock: 10, desc: "Ma description.", specs: ["Caractéristique 1"] }
```

## Limites

C'est une vitrine, pas une vraie boutique. Il manque ce qui demande un serveur :

- paiement en ligne
- comptes clients
- base de données des produits et des commandes
- envoi d'e-mails de confirmation

## Utilisation de l'IA

J'ai réalisé ce projet avec l'aide de Claude (Anthropic).

- **Moi :** le choix du projet, la relecture et la modification du code, les tests, la mise en ligne.
- **L'IA :** la proposition de thème et de design, la première version du code.

## Ce que j'ai appris

- Structurer une page web avec plusieurs parties qui interagissent (catalogue, fiche, panier)
- Gérer un état en JavaScript (le contenu du panier) et l'afficher à l'écran
- Utiliser `localStorage` pour garder des données dans le navigateur
- Publier un projet sur GitHub avec un README clair
