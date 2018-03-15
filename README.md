# PROPAGATION_BACTERIENNE

![image](https://www.aquaportail.com/pictures1309/bacteria-bacteries-virus.jpg)  
  
  
## Description du projet : ##

L'objectif est de comprendre l'évolution du système immunitaire simplifié.
Autrement dit comprendre l’efficacité des globules blanc sur les bactéries en fonctions de différents paramètres.
  
  
  
## Règles de la modélisation : ##  
#### Pour cette Modélisation, afin de faciliter le modèle d’étude, nous nous concentrerons simplement sur les globules blancs et la bactérie : Escherichia Coli (bactérie de référence).
  
Nous simulons notre modélisation dans une matrice. Les cellules de cette matrice peuvent prendre les valeurs suivantes :
+ Globule Blanc (GB) => 2
+ Bactérie (B) => 1
+ Le vide (-) => 0
+ Nutriment (N) => 3
  
  
  
Pour passer d'une étape à une autre on analyse le voisinage de chaque cellule de la matrice. Ce voisignage sera une “mini-matrice” de 3*3, soit les 8 nombres entourant d'une cellule.
Que faire si on est aux extrémités ? On observe alors deux types de cas pour le voisinage :
* Soit boite pétrie : milieu fini - ne pas prendre les voisins hors de la matrice.
* Soit corps humain : milieu infini (sphère) - au extrémité prendre les voisins. 
  
  
  
Voici les différentes règles de survie des organismes (version finale 15/03) :
+ Si une cellule est vide : elle possède une probabilité (proba_apparition_nutriments) de se transformer en un nutriment.
 
+ Si une bactérie est entourée d'un certain nombre de globule(s) blanc(s) (variable : nb_gb_nécessaires) : décès de la bactérie.
+ Si une bactérie n'a pas au moins un nutriment depuis un nombre t de tours : décès de la bactérie. (variable : t_survie_b).
  
+ A chaque tour, un nombre de globule(s) blanc(s) proportionnel au nombre de bactérie (variable : gb_par_bact) apparait sur une case vide adajacente à une bactérie.
+ Un globule blanc meurt par apopthose au bout d'un nombre t de tours. (variable : t_survie_gb).

+ Si un nutriment est à proximité d'une bactérie (aucun globule blanc adjacent) : le nutriment devient une bactérie.
+ Un nutriment meurt au bout d'un nombre t de tours. (variable : t_survie_n).


  
  
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
[Semaine 4](https://are00dynamic-2018.github.io/PROPAGATION_BACTERIENNE/Semaine4)
