# Funciones
Su nombre proviene de las funciones arimeticas, donde generalmente se trabaja de esta manera:

$$
y = f(x)
$$

Donde $y$ es el producto o el resultado de nuestra funcion, y $x$ es la variable que se puede cambiar en la formula para que de como resultado distintos valores de $y$

En programacion se trabaja de una manera similar:
```c++
tipo_de_resultado funcion(entrada 1, entrada 2)
{
    // funcion o programa a realizar
    devuelve resultado;
}
```
## Ejemplo
si se tuviera una funcion que sume dos numeros se puede escribir algo simple como una suma, suponiendo que estamos sumando solo enteros

$$
y = suma(a,b)
$$

mas detallado se veria asi:

$$
y = a + b
$$

en programacion se veria algo similar a:
```c++
int suma(int a, int b)
{
    // ponemos una variable para guardar el resultado de la suma
    int y;
    // luego sumamos
    y = a + b;
    // luego devolvemos el resultado para que lo use el resto del programa
    return y;
}
```
## `voids`
las funciones declaradas como `void` no necesita devolver ningun valor