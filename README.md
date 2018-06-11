# Actividad 04 - Funciones y probabilidad básica

* Para poder realizar esta actividad debes haber revisado la lectura correspondiente a la semana.
* Crea una carpeta de trabajo y guarda todos los archivos correspondientes (notebook y csv).
* Una vez terminada la actividad, comprime la carpeta y sube el `.zip` a la sección correspondiente.

## Ejercicio 1: Generación de funciones

* Genere funciones para calcular la media y varianza de un vector. Debe cumplir con los siguientes requistos:
    - Ambas funciones deben ingresar un argumento `x`.
    - Las funciones deben contener `docstrings` con la documentación asociada a la variable.
    - Deben __retornar__ el resultado (_tip_: utilice `return`).
    - La función de la varianza debe llamar a la función de la media.
* Utilice las funciones para reportar la información sobre `goles_favor`, `goles_contra`, `puntos`.


## Ejercicio 2: A continuación se presenta el siguiente código para obtener la media y varianza de una variable para distintos continentes
* En base a la información disponible, genere una función con los argumentos `group_by` y `var` para ingresar una lista de submuestras y una variable a analizar, respectivamente.
* La función debe retornar un `DataFrame`.
* Implemente la función para extraer la información sobre la cantidad de goles a favor, en contra y la cantidad de puntos.
* Reporte en qué continente se encuentra la mayor cantidad de goles a favor, en contra y cantidad de puntos.

## Ejercicio 3: Simulaciones

* Genere una función `generate_pet` que devuelva de forma aleatoria un string `'perro'` o `'gato'`. Ejecútela un par de veces.
    - _tip:_ Puede utilizar la función `np.random.choice` para retornar elementos al azar.

* Aplique la función `generate_pet` 20 veces mediante un loop y guarde los resultados en una lista.
    - _tip:_ Puede generar una lista vacía con `[ ]` y asignarla a un objeto. Puede añadir elementos a la lista con `.append`.
* ¿Cuál es la probabilidad de elegir un perro al azar? ¿Y un gato?

* Agrege `np.random.seed(2)` al inicio del chunk. ¿Qué hace éste método en la simulación?

## Ejercicio 4: Función simuladora

* Genere un método llamado `simulate_pets_prob` que tome como argumento un número finito de simulaciones a generar.
* El método debe simular dos situaciones `young_pet` y `old_pet`, y contar la ocurrencia de los siguientes casos:
    1. De los dos animales simulados, contar las ocasiones donde por lo menos uno de los animales sea un perro.
    - De los dos animales simulados, contar las ocasiones donde por lo menos uno sea un perro viejo.
    - De los dos animales simulados, contar las ocasiones donde los dos sean perros
* El método debe tener una semilla pseudoaleatoria de 1.
* De los tres escenarios, ¿Cuál es el menos probable? ¿Cuál es el más probable?
