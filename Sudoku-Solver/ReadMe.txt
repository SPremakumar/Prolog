EXPLICATION : 
Comment r�soudre les sudokus avec Prolog ?

Premi�rement, nous avons cr�er le pr�dicat "affiche_sudoku". Il permet d'afficher les valeurs du sudoku r�solu, avec des espaces entres eux (write(' ')), et en colonne c'est � dire � la ligne (nl). Deuxi�mement, nous allons initialiser les nombres.

Troisi�mement, nous avons cr�er le pr�dicat "different". Il permet de trouver les diff�rences entre les colonnes et les lignes. L'operateur '=\=' permet d'�valuer X et Y, et r�ussit s'il ne sont pas �gaux.

Quatri�mement, nous avons cr�er le pr�dicat "solution" en utilisant le pr�dicat "different" (d�finit pr�c�demment). Celui - ci (le pr�dicat solution), permet de trouver les diff�rences pour toutes les valeurs, entre les lignes, entre les colonnes et par carr�.

Et pour finir, nous avons cr�er le pr�dicat "sudoku", c'est la fonction principale, car il permet de trouver et afficher les valeurs du sudokus.



UTILISATION : 
Vous avez le choix avec plusieurs grilles de sudoku : 4x4; 6x6; 9x9 

Pour utiliser, il faut d'abord taper le pr�dicat, ensuite inserer les valeurs du sudoku : c'est � dire les nombres (de 1 � 9), et des cases vides (qu'il faut �crire _,) chacune espac�e. L'interpr�te de Prolog se s'agira de trouver la solution, et de vous l'afficher. 

?- sudoku(_, 1, _, 2, 4, _, _, _, _, _, _, 3, 1, _, 2, _).



