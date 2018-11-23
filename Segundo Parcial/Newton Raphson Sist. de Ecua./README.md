En esta variante del metodo los valores de las derivadas que intervienen en la expresion de la matriz jacobiana se aproximan
mediante formulas en diferencias finita. 

Esta variante consiste en utilizar durante la k primeras iteraciones (siendo k un numero a predeterminar por el usuario del 
metodo) como aproximacion de la matriz tangente la matriz Jf(x(0)). Con ello en estas k iteraciones solo se realiza una vez 
el calculo de la matriz jacobiana y de su inversa (y si se optase por la resoluci´on del sistema Jf(x(0))· δx(i) = f(x(i)) 
bastara con factorizar una vez la matriz Jf(x(0)) en la primera iteraci´on y conservar las matrices de la factorizacion). 
Realizadas estas k primeras iteraciones se calcula Jf(x(k)) y se utiliza esta matriz en las k siguientes iteraciones tras las
cuales se vuelve a actualizar obteniendose Jf(x(2·k)) y continuando ası el proceso.
