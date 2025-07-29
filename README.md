# Práctica 5: Serialización (Simple). 📌

Nombre: 

NumCuenta: 

En esta práctica se trabajará con la serialización de objetos y reforzar el tema de excepciones.

## Autores 😊
* **Salvador López Mendoza** - *Titular* - [Correo](slm@ciencias.unam.mx)
* **Gerardo Emiliano Figueroa Sandoval** - *Teoría* - [Emiliano-Fs](https://github.com/Emiliano-FS)
* **Ramsés Antonio López Soto** - *Laboratorio* - [ramseslopez](https://github.com/ramseslopez)
  
## Objetivos 🚀

- Entender qué es la persistencia de objetos.
- Comprender los conceptos de serialización y deserialización.

### Pre-requisitos 📋

- Sistema Operativo Linux (Ubuntu, Debian, Fedora, etc.)
- Git versión 2.43.0
- Java versión 21.0.7
- Perfil de GitHub

### Instalación 🔧

- Git

Para instalar la versión más reciente de Git:

```bash
sudo apt-get install git

```
Una vez finaliado, verifica la versión instalada.

```bash
git -v
```

- Java
  
Instala Java con el siguiente comando:

```bash
sudo apt-get install openjdk-21-jre
```

Al finalizar, verifica la versión instalada.

```bash
java --version
```
y también del compilador:

```bash
javac --version
``` 

## Recursos 📖

Puedes encontrar más información de los recursos a utilizar en:

- [Serializable](https://docs.oracle.com/javase/8/docs/api/java/io/Serializable.html)
- [Serialización de objetos](https://puntocomnoesunlenguaje.blogspot.com/2013/10/java-serializacion-persistencia.html)

## Ejercicio ⌨️

Lee con mucha atención las instrucciones:

### Contestadora

Esta práctica consiste en implementar una contestadora sencilla que guarda mensajes.

Implementa una clase _Mensaje_ que contenga la siguiente estructura y comportamiento:
  - Atributos
    - El cuerpo del mensaje.
    - El nombre del emisor.
    - El nombre del mensaje.
    - La fecha en la que se recibe el mensaje
    - La prioridad del mensaje (ordinario, casual o urgente).
  - Constructores
    - Constructor que inicializa los atributos.
  - Métodos
    - Métodos de acceso.
    - Método para comparar mensajes acorde a su prioridad.
    - Método para devolver el mensaje en forma de cadena.

Haciendo uso de la clase _Mensaje_, implementa una clase _Contestadora_ que contenga la siguiente estructura y comportamiento:

  - Atributos
    - Una lista de mensajes.
  - Constructores
    - Constructor que inicialice la lista con, a lo más, 15 mensajes.
  - Métodos
    - Un método de acceso.
    - Un método para guardar un mensaje.
    - Un método para leer un mensaje. Se debe de preguntar si se se desea eliminar el mensaje una vez se haya leído.
    - Un método para agregar el mensaje a la lista de mensajes.
    - Un método para obtener un mensaje dada una posición de la lista.
    - Un método para borrar un mensaje.
    - Un método para ordenar los mensajes de la `Contestadora` donde primero deben ir los urgentes, después los ordinarios y al final los casuales.
    - Un método para vaciar la `Contestadora`.
    - Un método para devolver la información de la `Contestadora`. Se debe poder ver el nombre del mensaje y la prioridad de este.

Deberás crear las siguientes excepciones:
   - `ContestadoraLlenaException` que se lanzará si se quiere guardar un mensaje cuando la contestadora ya esté llena.
   - `PosicionInvalidaException` si se desea obtener un mensaje de un  ́ındice que no existe.
   - `MensajeInexistenteException` si se desea borrar un mensaje que no existe.
   - `ContestadoraVaciaException` si se desea vaciar la `Contestadora` ya vacía.

Recuerda que tu programa debe ser +*ROBUSTO** y no debe terminar de forma inesperada;
debes indicar una forma de terminar la ejecución.

Además debes de utilizar la persistencia para preservar el estado de la `Contestadora`, es decir, si la `Contestadora` se apaga, el programa deben guardar todos los mensajes; si la `Contestadora` se prende, se deben mostrar los mensajes que se quedaron guardados la  ́ultima vez que se apagó.

No olvides docuemntar tu código y generar la documentación _html_ de cada clase que implementes y un archivo de prueba para visualizar el funcionamiento del programa.


## Intrucciones

* La práctica se entrega de forma individual.
* Debes de clonar el este repositorio con el comando `git clone`, agregar tu nombre en la parte de `Nombre: ` y seguido de tu número de cuenta en `NumCuenta: `.
* El código debe ser legible y el nombre varialbes y métodos debe ser adecuado. Debes de seguir las reglas correspondientes.
* Sube la solución de la práctica antes de las 23:59 del día de mañana con los comandos `git add`, `git commit` y `git push`.
* Una vez en el repositorio, debes de entregar en el Classroom la liga **HTTPS** que direcciona a tu repositorio.
* La calificación se determinará dependiendo del número de pruebas que pasen.
* Ningún tipo de copia y/o plagio será tolerado.

## Licencia 📄

Este proyecto está bajo la Licencia MIT - mira el archivo [LICENSE.md](LICENSE.md) para más detalles.