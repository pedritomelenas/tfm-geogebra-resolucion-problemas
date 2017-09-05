# Integración por Montecarlo

## Por bombardeo

1. Con la opción deslizadores, creo dos, uno llamado `a` para un parametro del que depende la función, y otro `n` del que dependerá el número de puntos aleatorios.
2. En la casilla entrada escribo la función que depende del parámetro.
3. En la hoja de cálculo del programa, creo 4 columnas las dos primeras generan n números aleatorios comprendidos entre 0 y `a`, mediante la orden `random()a`, la tercera crea puntos de dos coordenadas 1ª coordenada es 1ª columna y la 2ª coordenada es la 2ª columna, y la última nos devuelve un 1 si la segunda coordenada del punto es menor que la imagen mediante la función de la primera coordenada y 0 en caso contrario.
4. En la casilla de entrada mediante la orden `Secuencia(Celda(3,k),k,1,n)` creo una primera lista formada por los puntos de la tercera columna.
5. En la casilla de entrada mediante la orden `Secuencia(Celda(4,k),k,1,n)` creo una lista formada por los elementos de la última columna.
6. En la casilla de entrada mediante la orden `Suma(lista2)`` sumo los elementos de dicha lista y la llamo suma.
7. Mediante la orden intersección marco los puntos de corte de la función con los ejes de coordenadas.
8. Mediante la orden poligono regular construyo un cuadrilatero, donde la longitud de sus lados será la longitud del segmento de origen el 0 y final el punto de corte.
9. En la casilla de entrada llamo proporción al numero que sale de multiplicar, el cociente que sale de dividir suma entre `n`, por el area del cuadrilatero.
10. Mediante la orden boton, escribiendo en dicho boton, en el programa de guion la orden `ActualizaConstrucción[]`, creamos un boton que cada vez que lo pulsamos actualiza los números aleatorios.
11. En la casilla de entrada mediante la orden `Integral(función,a,b)`, calculo el valor real de la integral.

El valor aproximado es el valor del número proporción.


## Mediante evaluación en puntos aleatorios

1. Mediante la orden deslizador, creo uno llamado `N` que controlará el numero de elementos.
2. En la casilla de entrada, escribo la función.
3. En la casilla de entrada, mediante la orden `UniformeAleatoria(0,1,N)`, crea una lista de `N` números aleatorios que van desde el 0 al 1.
4. En la casilla de entrada, mediante la orden Secuencia, creo una lista con las imagenes mediante la función de los elementos de la lista anterior.
5. En la casilla de entrada, mediante la orden Secuencia creo una tercera lista formados por puntos en los que la primera coordenada son los elementos de la primera lista, y la segunda coordenada
 son los elementos de la segunda lista.
6. En la casilla de entrada, mediante la orden suma, sumamos los elementos de la lista imágenes, la llamamos suma.
7. En la casilla de entrada, mediante la orden `Integral(f(x),0,1)`, calculamos el valor real de la integral.
8. En la casilla de entrada, obtenemos el cociente entre el valor de la suma y `N`.
Éste es el valor aproximado de la integral.
