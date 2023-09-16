# RETO-3
## Algoritmo para encontrar numero primo hasta n 
diagrama de flujo:

```mermaid
flowchart TD
   A(inicio) --> B
    B[numero n] -->C
    C[primos:= ] -->D
    D[ i := 2] -->E{i % j = 0?}
    E-->|si|F(n no es primo)
    E-->|no|G(n es primo)
    F-->H( i := i + 1)
    G-->H
    H-->J{i <= n}
    J-->|no|E
```
Este es el pseudocodigo
```pseudocode
var i, j, primos: entero
  primos := []
  inicio
  i:= 2 
  mientras i <= n hacer
  para j := 2 hasta i - 1 hacer
      si i % j = 0 entonces
      sal
      fin_si
    fin_para
 // Si el número es primo, se agrega a la lista (i)
       i := i + 1
  fin_mientras
  fin
  ```
## Algoritmo para raices cuadradas
diagrama de flujo:
```mermaid
flowchart TD
    A(inicio)--> B
    B(y=0)-->C(while true)
    C-->D(y= y+1)
    D-->E[y^2 = y*y]
    E-->F{y^2 es igual a x?}
    F-->|no|G{y^2 < x?}
    G--->|no|H[y = y - 1]-->I(fin)
    F-->|si|J(return y)
```
```pseudocodigo
def raíz_cuadrada(x):
  y = 0
  while True:
    y = y + 1
    y2 = y * y
    if y2 == x:
      return y
    elif y2 < x:
      return y
    else:
      y = y - 1
```
