UTILISATION : 
Il suffit de taper le pr�dicat solution, et le nom d'une liste. 
?- solution(nom_liste).
Donne tous les combinaisons possibles : 
M = [[10, [buzz-woody]], [5, [buzz]], [25, [rex-jambon]], [10, [woody]], [10, [woody-buzz]]] ;
M = [[10, [buzz-woody]], [5, [buzz]], [25, [jambon-rex]], [10, [woody]], [10, [woody-buzz]]] ;
M = [[10, [buzz-woody]], [10, [woody]], [25, [rex-jambon]], [5, [buzz]], [10, [buzz-woody]]] ;
M = [[10, [buzz-woody]], [10, [woody]], [25, [jambon-rex]], [5, [buzz]], [10, [buzz-woody]]] ;
M = [[10, [woody-buzz]], [10, [woody]], [25, [rex-jambon]], [5, [buzz]], [10, [buzz-woody]]] ;
M = [[10, [woody-buzz]], [10, [woody]], [25, [jambon-rex]], [5, [buzz]], [10, [buzz-woody]]] ;
M = [[10, [woody-buzz]], [5, [buzz]], [25, [rex-jambon]], [10, [woody]], [10, [woody-buzz]]] ;
M = [[10, [woody-buzz]], [5, [buzz]], [25, [jambon-rex]], [10, [woody]], [10, [woody-buzz]]] ;
false.


INTERPRETATION : 

OBSTACLES : 
- Seulement deux jouets peuvent traverser ensemble le ponts.
- Ils n'ont qu'une seule lampe-torche, qui ne dure que 60 minutes.
- Ils ont besoin de la lampe-torche pour traverser (donc ils doivent se la retourner).
- Chaque jouets ont un temps diff�rent pour traverser.

PROBLEMATIQUE : Dans quel ordre les 4 jouets doivent traverser le pont � temps (c�d 60 minutes) pour �chapper � Zurg 

RESOLUTION : 
D'apr�s l'interpr�te, il y a pr�cisement deux solutions :
 
1ere solution : 
	- Buzz et Woody traverse le pont en premier,
	- Buzz retourne (pour donner la lampe-torche aux restants), et reste. 
	- Rex et Jambon traverse le pont (ils ont la lampe - torche)
	- Woody retourne de l'autre c�t� du pont, et rejoint Buzz (avec la lampe - torche donn�e par Rex et Jambon)
	- Buzz et Woody re - traverse le pont (ils ont la lampe - torche). 
	- Les jouets sont r�unis, en 60 minutes exactement. 

2eme solution : 
	- Buzz et Woody traverse le pont en premier,
	- Woody retourne (pour donner la lampe-torche aux restants), et reste. 
	- Rex et Jambon traverse le pont (ils ont la lampe - torche)
	- Buzz retourne de l'autre c�t� du pont, et rejoint Woody (avec la lampe - torche donn�e par Rex et Jambon)
	- Buzz et Woody re - traverse le pont (ils ont la lampe - torche). 
	- Les jouets sont r�unis, en 60 minutes exactement.