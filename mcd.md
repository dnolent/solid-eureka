# Retours sur le MCD

## Address

Il pourrait être utile d'ajouter d'autres propriétés pour que le client puisse préciser
un nom/prénom différent du site pour l'adresse, ainsi qu'une société éventuellement.
Un titre / une civilité pourrait également être proposée pour que cela soit plus précis.

Il serait bien de pouvoir également préciser un pays pour l'adresse.
Dans ce cas nous pourrions créer une entité permettant de les stocker.

Une adresse contiendrait un pays et un pays pourrait être relié à plusieurs adresses.

## User

Un utilisateur pourrait avoir d'autres propriétés, comme par exemple un nom/prénom,
une civilité.

## Order & Product

En reliant Order et Product directement, cela pose un problème pour l'historique.
En effet, si un utilisateur souhaite accéder à l'historique de ses commandes et
aux produits d'une commande en particulier, il aura les informations à jour.

C'est-à-dire que si le prix et/ou le nom d'un article change entre temps,
cela impactera toutes les commandes déjà passées.

De plus ici il n'est pas possible de préciser une quantité supérieure à 1.

La solution est de sauvegarder le nombre, la quantité et le prix de chaque
produit commandés pour chaque commande.