# SAYNA-MERISESQL-ECOMMERCE

#Relations :
Client peut passer plusieurs Commandes, mais chaque Commande est passée par un seul Client (Relation 1-N entre Client et Commande).
Un Utilisateur/Administrateur peut gerer plusieurs Commandes, mais chaque Commande ne peut être gerer que par un seul Utilisateur/Administrateur (Relation 1-N entre Utilisateur/Administrateur et Commande).
Une Commande peut contenir plusieurs Produits, et un Produit peut être contenu dans plusieurs Commandes (Relation N-M entre Commande et Produit via Détail de la commande).
Un Produit appartient à une seule Catégorie, mais une Catégorie peut avoir plusieurs Produits (Relation 1-N entre Catégorie et Produit).
Dans une relation "plusieurs à plusieurs" (N-M) entre les tables Commande et Produit, il est nécessaire d'introduire une table de transition pour gérer cette relation.
Dans cette structure, la table Detail_commande sert de table transition pour gérer la relation N-M entre Commande et Produit. Chaque enregistrement dans Detail_commande représente un produit spécifique inclus dans une commande spécifique, avec la quantité et le montant correspondants.
Cela permet à un produit d'appartenir à plusieurs commandes et à une commande de contenir plusieurs produits.
