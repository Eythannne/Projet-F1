Projet F1 — Python - Java - JavaScript



Python :

1) La chaine de caractere est modifié avec un strip et j'ai ajouter un split avec ":" pour pouvoir separer les minutes des secondes, et le resultats et rarondi à 3 décimales. Si la chaine de caractere est vide la fonction renvoie "none".

2) J'ai d'abord commencer par importer le csv pour que la fonctione puisse y avoir acces, le csv renvoie une liste de donnée, la position est convertis en entier, si le statut est "abandon" alors la position vaut "0 donc la case sera vide". le meilleur tour est convertis en seconde.

3) D'abord commencer par crée un nouveau fichier au propre, on commence par l'en-tete puis on fait une boucle for pour afficher ligne par ligne avec des valeurs séparer par un ";". le temps est affiché avec 3 décimales et on laisse vide si il y a un abandon

---------------------------------------------------------------------------------------------------------------------------------

Java : 

1) La fonction permet de savoir combien de point son obtenu selon la position, si la position est entre 1 et 10 la methode va chercher combien de points seront donnée aevc le tableau "BAREME", il faut mettre -1 car le tableau commence a 0. Si jamais il y a un abandon la valeur sera de 0 et si 10e ou plus ça sera 0 aussi

2) La fonction permet de construire le calssement des pilotes a partir des lignes de courses. Le for permet de questionner si le pilote est deja dans le classement et le crée si il n'y ai pas. Ensuite on ajoute les points aux pilotes et on compte ses victoires. Puis on tri la liste pas ordre decroissant des points, puis par victoire, puis par ordre alphabétique en cas d'égalité

3) On commence par chercher si l'écurie du pilote est bien dans le classement et si elle n'y est pas on l'a crée, ensuite on ajoute les points en les additionnant puis on fait le tri (de la meme facon que le tri des pilotes)

4) Le code commence par parcourir toute les lignes et on garde que celle du pilote demandé, en ignorant ses abandon (position 0). Pour chaque course terminé, on aditionne sa position et on compte une course de plus. Ensuite, si le pilote n'a fini aucune course, on renvoie 0. Sinon, on divise la somme par le nombre de courses (avec un `(double)` pour avoir un résultat décimal) et on arrondit à 2 décimales avec `Math.round`.

---------------------------------------------------------------------------------------------------------------------------------

JavaScript

