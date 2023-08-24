# mcd

**1) Mauvaises cardinalités sur le LIKE** entre USER et PRODUCT

Comme tu l'as entouré, la relation LIKE doit être en Many To Many et là elle est unique et même obligatoire à 1,1:

-   Un produit (mug) peut être like par plusieurs utilisateurs mais aussi par aucun utilisateurs
-   Un utilisateur peut like plusieurs produits ou aucun

**Les cardinalités 1-1 ne sont pas bonnes et doivent être en 0-N !**

* * *

**2) Mauvaises cardinalités sur CONTAIN** entre ORDER et PRODUCT

Pour cette exercice, on a un contexte avec une app ecommerce simplifiée. On veut juste pouvoir commander un produit comme l'indique la dernière phrase de l'énoncé. On ne veut pas forcément avoir à gérer une commande multiple, un panier d'achat, des factures etc...

On aurait donc plutôt **1,1 CONTAIN 0,N**:

Dans ce cas là, notre entité ORDER pourrait ne pas contenir la propriété total_amount puisqu'on a déjà l'amount dans PRODUCT.

* * *

**3) Mise en page !**

Ce n'est pas parce que tu as peu d'entités sur un schéma, que tu ne dois pas l'arranger visuellement. **Un MCD doit justement faciliter la lecture **et là on dirait que tu as arrangé les éléments un peu en vrac, c'est dommage !

**Penses aussi à bien représenter les relations, plutôt sous forme ovales.**

C'est peut être à cause de l'outil que tu as utilisé pour faire ton MCD ? S'il ne propose pas plus de formes, ou n'agence pas bien les éléments, tu peux utiliser un outil comme <https://www.drawio.com/> qui propose vraiment plein de formes et même des templates pour plein d'autres documents pratiques qu'on pourrait te demander en entreprise.

Il y a aussi <https://www.lucidchart.com/> qui est populaire mais il me semble qu'il est payant.

