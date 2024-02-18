# OPERADORES LÓGICOS

Los operadores lógicos son utilizados para hacer comparaciones entre dos valores, con el objetivo de regresar un valor booleano `bool` como `true` o `false`.

## Tipos de operadores lógicos

- **Igualdad** (**==**): Este operador lógico compara dos valores para saber si ambos son **iguales**, o si son diferentes. En caso de ser iguales devolverá `true` en el caso contrario devolverá `false`.
    ```cpp
    5 == 10 // false
    5 == 5  // true
    ```
- **Desigualdad** (**!=**): Este operador lógico compara dos valores para saber si ambos son **diferentes**, o si son iguales. En caso de ser diferentes devolverá `true` en el caso contrario devolverá `false`.
- Mayor que (**>**):
    ```cpp
    5 != 10 // true
    5 != 5  // false
    ```
- **Menor que** (**<**): Este operador lógico compara dos valores para saber si el de la izquierda es **menor** al valor de la derecha, en caso de ser así devolverá `true`, de lo contrario devolverá `false`.
    ```cpp
    5 < 10  // true
    5 < 5   // false
    10 < 5  // false
    ```
- **Mayor que** (**>**): Este operador lógico compara dos valores para saber si el de la izquierda es **mayor** al valor de la derecha, en caso de ser así devolverá `true`, de lo contrario devolverá `false`.
    ```cpp
    5 > 10  // false
    5 > 5   // false
    10 > 5  // true
    ```
- **Menor o igual** (**<=**): Este operador lógico compara dos valores para saber si el valor de la izquierda es **menor o igual** que el valor de la derecha, de ser así devolverá `true`, de lo contrario devolverá `false`.
    ```cpp
    5 <= 10  // true
    5 <= 5   // true
    10 <= 5  // false
    ```
- Menor o igual (**>=**): Este operador lógico compara dos valores para saber si el valor de la izquierda es **mayor o igual** que el valor de la derecha, de ser así devolverá `true`, de lo contrario devolverá `false`
    ```cpp
    5 >= 10  // false
    5 >= 5   // true
    10 >= 5  // true
    ```