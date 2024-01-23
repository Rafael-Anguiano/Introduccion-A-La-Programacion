# Instalación:

Hola, en esta lección aprenderás a instalar el ambiente necesario para utilizar `C++` en el editor de texto **"Visual Studio Code"**.

> [!WARNING]
> Visual Studio Code es solo un editor de texto, existen muchas opciones que puedes elegir, algunas incluso mejores, así que sientete libre de elegir el ambiente que más sea de tu agrado.

## VS Code:
**1.** Para comenzar a utilizar [`Visual Studio Code`](https://code.visualstudio.com/Download), es necesario instalarlo primeramente, por lo que te sugiero clickear en el link anterior y descargar el instalar basandonos en tu sistema operativo (Windows / macOS / Linux).

**2.** Una vez descargado, por favor abre el instalador que se te ha descargado. Posteriormente puedes simplemente darle repetidas veces al botón de siguiente y aceptar.

**3.** Al abrir la aplicación, encontrarás al lado izquierdo un panel con diferentes íconos como los mostrados en la imagen siguiente, por favor selecciona el ícono que está mostrado en la imagen de abajo con un recuadro rojo.

![VS Code Icons](./images/VSCode%20Icons.png)

**3.** Ahora haremos la instalación de la extensión que nos hará la vida más fácil a la hora de correr nuestro código.

- En la barra de busqueda, escribe `C++`, algunas extensiones serán mostradas.
- Selecciona la que diga `C/C++`. Como muestra en la imagen siguiente.
- Haz click en el botón de `instalar`.

![Extension Instalation](./images/Extension%20Instalation.png)

**4.** Una vez que lo hayas instalado deberás cerrar y volver abrir `VS Code`.

## Compilador:
**1.** Para ser capaces de correr nuestro código es importante instalar el compilador necesario, en este caso estaremos utilizando el instalador `MSYS2` como compilador. Por favor descarga dicho instalador [aquí](https://github.com/msys2/msys2-installer/releases/download/2023-05-26/msys2-x86_64-20230526.exe) y ejecútalo posteriormente.

**2.** En el instalador tu solo necesitas hacer click en los botones de **"siguiente"** y **"Aceptar"**.
> [!NOTE]
> Asegurate de que al final el recuadro para abrir el programa esté marcado de forma positiva.
>
>  En caso de que no hayan marcado el recuadro busca dentro de tus programas `MSYS2`.


**3.** Verás que este programa ha abierto una termianl. Dentro de ella deberás pegar el siguiente comando.
> [!TIP]
> Probablemente vayas a tener problemas para pegar el comando dentro de la terminal. 
>
> En este caso te sugiero que en lugar de utilizar el teclado para pegar, utilices el click derecho de tu mouse.

```sh
    pacman -S --needed base-devel mingw-w64-ucrt-x86_64-toolchain
```

> [!CAUTION]
> El proceso de instalación del compilador empezará, sin embargo serás preguntado varias cosas para continuar.
>
> En un punto la terminal te preguntará para `ingresar una selección`, en este caso solo será necesario **`Presionar Enter`**.
>
> ![Default Selection](./images/Default%20selection.png)

> [!CAUTION]
> Posteriormente serás preguntado quieres proceder, en este caso utiliza tu teclado y escribe `Y` y `Presiona Enter`.
>
> ![Yes](./images/Yes.png)


**4.** Una vez que el proceso haya terminado, necesitaremos editar las variables de entorno para poder hacer uso de los comandos correspondientes.
    
- En tu buscador de Windows, busca: "Variables de Entorno".
- Ahí encontrarás un programa con un texto parecido a "Editar Variables de Entorno"
- Tendremos que buscar las variables de entorno **DE USUARIO**, seleccionaremos la variable **`Path`** y posteriormente seleccionaremos **`Edit`**.
![Path](./images/Path.png)
 - Ahora presionaremos el botón para agregar una `Nueva Variable` y añadiremos el folder destino del compilador MinGW-w64 el cuál (en caso de no haber cambiado nada) será el siguiente:
   ```sh
       C:\msys64\ucrt64\bin.
   ```
 ![Enviroment Variable](./images/EnviromentVariables.png)
- Presiona el botón de `Aceptar`. Para checar si fue correctamente instalado, deberás cerrar las terminales que tengas abiertas y reabrirlas.
  

**5.** Para checar si fue correctamente instalado, pega los siguientes comandos en tu terminal.

    ```sh
        gcc --version
        g++ --version
        gdb --version
    ```
> [!NOTE]
> Deberás ver información correspondiente a las versiones de los comandos. 
> Si por el contrario te apareció un error, o ves todo en rojo, de seguro hubo algún problema en la instalación. Levanta la mano y lo resolveremos sin problema. :) 
