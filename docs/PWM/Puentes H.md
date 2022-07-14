# Puentes H
Si bien el arduino es capaz de mover motores DC de pequeño tamaño, no esta diseñado para esta tarea por la poca potencia que maneja en sus puertos, en su lugar, se ocupa otro chip que es capaz de manejar la corriente necesaria para esto, uno de esos chips son los puentes H. Los mas comunes son

- L293D
- L298N
- A4988 y similares

# L293 y L298
estos son de bajo costo y manejan ambos 2 motores como maximo
## Esquematico
## Codigo
### Uso Basico
#### Ejemplo: Giro
=== "Setup"

    ```arduino
    void setup() {
        pinMode(3, OUTPUT); // 3~
        pinMode(4, OUTPUT); // IN1
        pinMode(5, OUTPUT); // IN2
    }
    ```

=== "Loop"

    ```arduino
    void loop() {
        analogWrite(3, velocidad);
        digitalWrite(4, HIGH);
        digitalWrite(5, LOW);
    }
    ```

#### Ejemplo: Aceleracion
#### Ejemplo: Controlado por Potenciometro
#### Ejemplo: Dos Motores
### Uso con Funciones
#### Ejemplo: Funcion `motorl298`
# A4988