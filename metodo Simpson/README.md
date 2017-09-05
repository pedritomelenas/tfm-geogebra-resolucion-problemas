# Integración usando el método de Simpson

Applet explicando el [método de Simpson](https://es.wikipedia.org/wiki/Regla_de_Simpson) para integración.

1. En la casilla de entrada, introducimos la función.
2. En la casilla de entrada, definimos la lista `{(a,f(a)),(a+b/2,f(a+b/2)),(b,f(b))}`.
3. En la casilla de entrada, definimos la función `g(x)=Ajustepolinómico(lista anterior,2)`.
4. En la casilla de entrada, mediante la orden `Integral(g(x),a,b)`, calculamos la integral entre a y b del polinomio ajustado.
Ésta será la aproximación de la integral.

Esta versión está inspirada en este [applet](https://www.geogebra.org/material/show/id/497635). 
