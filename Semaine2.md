## Compte rendu de la semaine 2 ##

Bonjour bonjour, déjà 7 jours que notre projet est lancé.

Pour débuter quoi de mieux qu'une belle citation :
> "Quel est le rêve de toute cellule, devenir deux cellules". François Jacob
  
Plus concrétement, nous avons continué le travail avec pour objectif d'avancer dans l'écriture du code et dans nos recherches sur la petite vie des bactéries. Ainsi nous avons déterminer les "Règles de la modélisation" sur la page d'accueil, et coder ces mêmes règles dans une nouvelle fonction sur notre programme avec une importante quantité de **conditions** et de **paramètres** pour un fonctionnement optimal.  
  Voici un extrait de la fonction
``` 
if (c == 1): #Bactérie
        if (globules >= nb_gb_necessaires):
            return 0
        elif (nutriments == 0):
            return 0
        elif(bacteries >= nb_b_surpop):
            return 0
        else:
            return 1
```
  
Lors de la création de cette fonction, suite à une erreur *"list out of the range"*, nous avons décidé de mettre de coté l'option "infini" pour y revenir plus tard.
  
Nous pouvons maintenant optenir à partir d'une matrice initiale, la matrice à l'état suivant. Et le tout grace à une super bouton *click me*, une magnifique trouvaille de Alexandre.
