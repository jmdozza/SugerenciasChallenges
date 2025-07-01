A continuación veremos el paso a paso para llegar al resultado del output. 

A la izquierda se ve una matriz con los nombres de cada entidad y a la derecha una matriz para ver el estado de cada entidad.

#### Tipo de entidad pasado como parametro en el test case: *Goblin*

### 1. Posición [0][0]
<img src="images/mn1.png" width="200"/> <img src="images/me1.png" width="200"/>

🟢: Entidad a activar (Goblin) 
🔵: Celdas vecinas

En primer lugar GoblinVerde ya esta activo, entonces no es necesario volverlo activar. Como Trampa y GoblinBlanco estan Inactivas, pasan a estar activas. Por lo que la matriz de estados queda así:

![Matriz Estados](images/mn2.png)

### Posición [0][1]

En trampa no hacemos nada ya que la entidad que se paso como parametro a activar fue *Goblin*, por lo tanto no es necesario revisar los vecinos de Trampa. La matriz de estados no presenta cambios

![Matriz Entidad](images/me3.png)

### Posición [0][2]

En Fantom tampoco es necesario revisar algo , la matriz de estados no presentara cambios.

![Matriz Entidad](images/me4.png)

### Posición [1][0]

<img src="images/me5.png" width="200"/> <img src="images/mn2.png" width="200"/>

De nuevo volvemos a encontrar una entidad de tipo Goblin así que revisamos su estado y el estado de sus celdas vecinas. Actualmente esta entidad se encuentra *Activa*, entonces no cambia su estado. Respecto a sus vecina encontramos que en la posición [0][0] encontramos un goblin que esta activo por lo tanto le asigamos un estado de *Inactiva*. En la posición [1][1] encontramos una entidad de tipo Espectro con estado *Activa*, sin embargo Espectro no implementa *Desactivable*, por lo tanto se deja en *Activa* y no cambia su estado. La matriz de estados resultante es la siguiente:

![Matriz Estados](images/ms3.png)

### Posición [1][1]

En esta posición nos encontramos con una entidad de tipo Espectro, sin embargo no nos interesa inspeccionarla.

![Matriz Estados](images/me6.png)

#### Finalmente se obtiene la siguiente matriz de estados como resultado:

![Matriz Estados](images/ms3.png)




