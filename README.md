# PROPAGATION_BACTERIENNE

![image](https://www.aquaportail.com/pictures1309/bacteria-bacteries-virus.jpg)  
  
  
## Description du projet : ##

L'objectif est de comprendre l'évolution du système immunitaire simplifié.
Autrement dit comprendre l’efficacité des globules blanc sur les bactéries en fonctions de différents paramètres.
  
  
  
## Règles de la modélisation : ##  
#### Pour cette Modélisation, afin de faciliter le modèle d’étude, nous nous concentrerons simplement sur les lymphocyte NK (Natural Killer). Ce sont des Globules blanc qui développent une cytotoxicité pouvant lyser les bactéries.
  
Nous simulons notre modélisation dans une matrice. Les cellules de cette matrice peuvent prendre les valeurs suivantes :
+ Globule Blanc (GB) => 2
+ Bactérie (B) => 1
+ Le vide (-) => 0
+ Nutriment (N) => 3
  
  
  
Pour passer d'une étape à une autre on analyse le voisinage de chaque cellule de la matrice. Ce voisignage sera une “mini-matrice” de 3*3, soit les 8 nombres entourant d'une cellule.
Que faire si on est aux extrémités ? On observe alors deux types de cas pour le voisinage :
* Soit boite pétrie : milieu fini - ne pas prendre les voisins hors de la matrice.
* Soit corps humain : milieu infini (sphère) - au extrémité prendre les voisins. 
  
  
  
Voici les différentes règles survie des organisme (Nutriments, Agression) possibles :
+ Si une cellule est vide : probabilité (proba_apparition_nutriments) de se transformer en un nutriment.
+ Si une cellule vide est entourée d'une certain nombre (variable : nb_gb_reproduction) de globule(s) blanc(s) : tranformation en un globule blanc 
 
+ Si une bactérie est entourée d'un certain nombre (variable : nb_gb_nécessaires) globule(s) blanc(s) : décès de la bactérie.
+ Si une bactérie est entourée d'un certain nombre (variable : nb_b_surpop) de bactérie(s) : décès de la bactérie.

+ Si un globule blanc est entourée d'un certain nombre (variable : nb_b_nécessaires) bactérie(s) : décès du globule blanc.
+ A chaque on fait apparaitre un nombre (nb_gb_apparition) de globule(s) blanc(s) aléatoirement sur une case vide. 
+ Probabilité (proba_apoptose) que les globules blanc meurt : apparition d'une case vide

+ Si un nutriment est à proximité d'une bactérie : le nutriment devient une bactérie.
  
  
## Membres du groupe : ##
  
Alma Draeger.
alma-draeger@live.fr

Alexandre Janin.
alexandrejanin92@gmail.com

Fabien Benthami.
fabien.benthami@yahoo.fr

Nadir Ait Kheddache.
nadir.aitkheddache@gmail.com

Idriss Alaoui Soulimani.
idrissalaouisoulimani@gmail.com
  
  
## Lien du Google Docs pour les membres du groupe : ##

<https://docs.google.com/document/d/1I5axaokHjcQKSrqvp-DZnSG8qAAc6KvY1ZnKoHlSVAg/edit?usp=sharing>
  
  
  
## Compte rendu : ##

[Semaine 1](https://are00dynamic-2018.github.io/PROPAGATION_BACTERIENNE/Semaine1)  
[Semaine 2](https://are00dynamic-2018.github.io/PROPAGATION_BACTERIENNE/Semaine2)
[Semaine 3](https://are00dynamic-2018.github.io/PROPAGATION_BACTERIENNE/Semaine3)
