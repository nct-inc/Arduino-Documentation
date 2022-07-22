# Variables
## Definicion
Las variables son espacios en memoria en los que se pueden guardar determinados tipos de datos.

Los tipos de variables mas utilizados son los siguientes:

| Variable | Uso | Extension |
| ------ | ------ | -------- |
| `int` | Recibe / guarda numeros enteros positivos y negativos | `-32,768 - 32,767` |
| `long` | igual que `int` pero soporta mayores cantidades | `2,147,483,648 - 2,147,483,647` |
| `double/float` | se usan para guardar numeros decimales y al mismo tiempo puede usar una cantidad aun mas grande que un `long` | `8.5, -230.45687` |
| `char` | Guarda caracteres alfanumericos y simbolos | `a, A, b, z, 0...9, @, #, $, %` |
| `String` | Guarda grupos de caracteres como si fuera una lista: palabras u oraciones enteras | `"hola"`, `"Hola Mundo"`| 

!!! info "Nota"
    La extension maxima de las variables aplica al arduino Uno o placas equivalentes (que lleven de CPU un `ATMEGA328-P`)

## Sintaxis
Todos los tipos de variables se pueden usar de dos maneras:

- Creando una variable con un valor inicial

```c++
int mi_variable = 1234
String palabra = "asdfghjkl"
String oracion = "Hay una casa en la pradera."
float temperatura = 25.9
```

- Declarando solo la variable, usar un valor inicial no es necesario

```c++
int algo;
double altura;
String fecha;
```
!!! warning "Advertencia"
    - Por las capacidades limitadas del Arduino `float` y `double` funcionan de la misma manera.
    - `float` y `double` solo permiten ocupar de 6 a 7 numeros en total, si se usaran mas numeros, la variable va a descartar los numeros que tenga en exceso.
