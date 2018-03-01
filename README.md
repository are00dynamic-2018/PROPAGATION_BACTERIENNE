# PROPAGATION_BACTERIENNE

![image](https://www.aquaportail.com/pictures1309/bacteria-bacteries-virus.jpg)


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
  
  
  
## Description du projet : ##

L'objectif est de comprendre l'évolution système immunitaire simplifié.
Autrement dit comprendre l’efficacité des globules blanc sur les bactéries en fonctions de différents paramètres.
  
  
  
## Règle de la modélisation : ##  
##### Pour cette Modélisation, afin de faciliter le modèle d’étude, nous nous concentrerons simplement sur les lymphocyte NK (Natural Killer). Ce sont des Globules blanc qui développent une cytotoxicité pouvant lyser les bactéries.
  
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
+ Si une bactérie est entourée de m (variable) globule(s) blanc(s) : décès de la bactérie.
+ Si une bactérie est sans nutriments à proximité : décès de la bactérie.
+ Si une bactérie est entourée uniquement d'autres bactéries : décès de la bactérie.
+ Si un nutriment est à proximité d'une bactérie : le nutriment devient une bactérie.
+ Si un globule blanc est entourée de k (variable) bactérie(s) : décès du globule blanc.

  
  
## Lien du Google Docs : ##

<https://docs.google.com/document/d/1I5axaokHjcQKSrqvp-DZnSG8qAAc6KvY1ZnKoHlSVAg/edit?usp=sharing>
  
  
  
## Compte rendu : ##

[Semaine 1](https://are00dynamic-2018.github.io/PROPAGATION_BACTERIENNE/Semaine1)  
[Semaine 2](https://are00dynamic-2018.github.io/PROPAGATION_BACTERIENNE/Semaine2)  
