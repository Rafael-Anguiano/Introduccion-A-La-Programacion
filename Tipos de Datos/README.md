# TIPOS DE DATOS

## ¿Qué son los tipos de datos?

C++, que es el lenguaje que estaremos utilizando, es lo que denominamos un *"Lenguaje Tipado"* lo que significa que debemos especificar en nuestro programa el tipo de dato que será cada una de nuestras variables (entero, flotante, booleano, character, ...).

La forma de definir un tipo de dato es la siguiente:

```cpp
int variable = valorDeLaVariable;

```
Siendo en este caso `int` el tipo de dato a utilizar.

## Los tipos de datos

En C++ encontramos varios tipos de datos, los principales son:
- Entero (***int***): Este tipo de dato indica que la variable solo podrá aceptar valores numéricos que estén en el rango de los números enteros.
    > Por ejemplo: 1, 2, 3, 0, -3, -15, 100000.

    La forma de definir este tipo de dato es la siguiente:
    ```cpp
    int variable = valorDeLaVariable;
    ```

- Flotante (***float***): Este es un tipo de dato numérico que tiene el rango de los números decimales. Se le llama float por el denominado "punto flotante" utilizado en binario para representar números que decimales.

    > Por ejemplo: 1.5, 0.2, 5.123, 0.0, -14.2.
    
    La forma de definir este tipo de dato es la siguiente:
    ```cpp
    float variable = valorDeLaVariable;
    ```

- Double (***double***): Este tipo de dato está en el rángo de los decimales, sin embargo, cuenta con una mayor precisión que float, de ahí que su nombre sea double, ya que cuenta con el doble de precisión y rango.
    
    La forma de definir este tipo de dato es la siguiente:
    ```cpp
    double variable = valorDeLaVariable;
    ```

- Booleano (***bool***): Este tipo de dato utiliza solamente 1 byte, por lo que solo puede representar valores como: 1 o 0. Sin embargo, en lugar de usar 1 o 0, utilizamos las palabras `true` y `false`.
    
    La forma de definir este tipo de dato es la siguiente:
    ```cpp
    bool variable = true;
    bool variable = false;
    ```

- Caracter (***char***): Este tipo de dato es utilizado para guardar valores alfanuméricos, específicamente letras.

    > Por ejemplo: 'a', 'b', 'c'.    
    
    La forma de definir este tipo de dato es la siguiente:
    ```cpp
    char variable = 'c';
    char variable = 'b';
    ```

    > [!NOTE]
    > Es importante el uso de una sola comilla, ya que las comillas dobles están reservadas para los strings.

## Otros tipos de datos:

- Cadenas de Caracteres (***string***): Este tipo de dato nos ayuda para guardar multiples caracteres, como frases completas, o palabras.

    > Por ejemplo: "hello", "world", "This is my project".    
    
    La forma de definir este tipo de dato es la siguiente:
    ```cpp
    #include <string>
    string variable = "Hello World";
    string variable = "Welcome";
    ```

    > [!IMPORTANT]
    > Este **NO** es un tipo de dato nativo de C++, sin embargo, podemos acceder a él haciendo uso de la importación de la librería.

- Arreglos (***Arrays***): Este no es específicamente un tipo de dato, pero nos permite guardar múltiples valores de un mismo tipo de dato.
   
    La forma de definir este tipo de dato es la siguiente:
    ```cpp
    int[] variable = { 1, 2, 3 };
    char[] variable = { 'H', 'e', 'l', 'l', 'o'}
    ```