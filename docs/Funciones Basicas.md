# Funciones Basicas
El arduino se puede operar de manera sencilla usando funciones predefinidas en el IDE
## `pinMode`
Esta funcion especifica de que modo se va a utilizar un pueto en el arduino, pide 2 parametros
| Parametro | Valores |
| ------ | ------ |
| `pin` | El pin a configurar |
| `modo` | en que modo se configurara, si como salida(`OUTPUT`) o entrada(`INPUT`) |
```arduino
// se configura el pin 6 como una salida
pinMode(6, OUTPUT);
// se configura el 2 como una entrada
pinMode(2, INPUT);
```
## `digitalRead`
Esta funcion obtiene un valor digital de la señal que le llega al numero de puerto especificado, este valor es un `HIGH`(un 1 digital) o `LOW` (un 0). Se puede pasar este valor a un `int` tnto como a un `boolean`
```arduino
// se lee el valor en el pin 3
int valor = digitalRead(3)
// se puede pasar este valor tambien a un boolean
bool abierto = digitalRead(5)
```
## `analogRead`
`analogRead` obtiene el valor analogico que llega a un puerto, en otra palabras, mide el voltaje que esta llegando a este puerto. el puerto tiene una resolucion de 10 bits, lo que quiere decir que esta funcion otorga un valor entre 0 y 1024 segun el voltaje de llegada.

Esta funcion solo se puede usar en los pies marcados con `ANALOG` en la placa
```arduino
// se lee el valor de pin A0 y se pasa este al entero "valor"
int valor = analogRead(A0);
```
## `digitalWrite`
Esta funcion escribe un valor digital de `HIGH` o `LOW` al puerto que se especifique

| Parametro | Valores |
| ------ | ------ |
| `pin` | El pin a configurar |
| `salida` | `HIGH` o `LOW` |

```arduino
// se encendera el led que esta en el pin 13 del arduino
digitalWrite(13, HIGH);
// se espera 1 segundo
delay(1000);
// y luego se apaga el led
digitalWrite(13, LOW);
```

## `analogWrite`
Escribe un valor analogico al pin especificado usando PWM, a diferencia de `analogRead` que se puede usar en los pines marcados como analogicos, `analogWrite` se puede usar en todos los pines que estan marcados con salida PWM(`~`).

| Parametro | Valores |
| ------ | ------ |
| `pin` | El pin a configurar |
| `salida` | 0 (cero actividad) - 255 (completamente encendido) |

```arduino
// se utliza un led RGB y se le imprime un color en especifico
analogWrite(9, 128);
analogWrite(10, 200);
analogWrite(11, 255);
```
