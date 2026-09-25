Projet F1 — Python - Java - JavaScript



Python :

1) J'ai nettoyé la chaîne de caractères avec `strip`, puis j'ai ajouté un `split` avec ":" pour séparer les minutes des secondes. Le résultat est arrondi à 3 décimales. Si la chaîne est vide, la fonction renvoie `None`.


2) J'ai d'abord commencé par importer `csv` pour que la fonction puisse lire le fichier. La fonction renvoie une liste de données, la position est convertie en entier, et si le statut est "ABANDON" alors la position vaut 0 et le temps reste vide. Le meilleur tour est converti en secondes.


3) J'ai d'abord commencé par créer un nouveau fichier propre, puis j'ai écrit l'en-tête. Ensuite j'ai fait une boucle `for` pour écrire ligne par ligne avec les valeurs séparées par un ";". Le temps est écrit avec 3 décimales et on le laisse vide s'il y a un abandon.

---------------------------------------------------------------------------------------------------------------------------------

Java : 

1) J'ai commencé par vérifier si la position est entre 1 et 10. Si c'est le cas, je vais chercher les points dans le tableau `BAREME` avec `position - 1`, car un tableau commence à 0. Sinon la méthode renvoie 0 (abandon ou au-delà de la 10e place).

2) J'ai commencé par parcourir toutes les lignes et chercher si le pilote est déjà dans le classement. S'il n'y est pas, je le crée. Ensuite j'ajoute ses points, ses victoires (position 1) et ses 2e places. Puis je fais le tri avec `sort` : d'abord les points, puis les victoires, puis les 2e places, et enfin l'ordre alphabétique.

3) J'ai commencé par chercher si l'écurie du pilote est déjà dans le classement, et si elle n'y est pas je la crée. Ensuite j'additionne les points, victoires et 2e places de chaque pilote, puis je fais le tri de la même façon que pour les pilotes.

4) J'ai commencé par parcourir toutes les lignes et je ne garde que celles du pilote demandé, en ignorant ses abandons. J'additionne ses positions et je compte ses courses terminées. S'il n'en a fini aucune, je renvoie 0. Sinon je divise la somme par le nombre de courses (avec `(double)` pour avoir un résultat décimal) et j'arrondis à 2 décimales avec `Math.round`.
---------------------------------------------------------------------------------------------------------------------------------

JavaScript

1) J'ai commencé par faire une copie de la liste avec `[...liste]`. Ensuite je l'ai trié avec la méthode `sort`, celui qui a le plus de points passe devant. Si il y a des égalités, celui qui a le plus de victoires passe devant.Puis on affiche tout. 

2) J'ai commencé par récupérer le tableau avec `getElementById` et je l'ai vidé avec `innerHTML = ""`. Ensuite j'ai fait une boucle `for` : pour chaque élément, je crée une ligne `<tr>` avec ses 5 cellules (rang, nom, écurie, points, victoires). Puis je l'ajoute dans le tableau avec `appendChild`.

3) J'ai commencé par récupérer toutes les lignes du tableau avec `querySelectorAll`. Ensuite j'ai fait une boucle `for` : pour les 3 premières, j'ajoute la classe `podium`, et pour les autres je la retire.
