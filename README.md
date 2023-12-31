# Arduino
Primer y segunda parte Arduino Parcial
# Ejemplo Documentación 
![Tinkercad](./img/arduino.jpg)


## Integrantes 
- Nicolas Caliari
- Tobias Pasinato
- Luciano javier Lucero


## Proyecto: Contador binario.
![Tinkercad](./img/1.png)
![Tinkercad](./img/2.png)
![Tinkercad](./img/3.png)


## Descripción
Primera parte: Se encarga de sumar, restar y resetear un contador. Sumando de a uno al contador o restando de a uno y en el caso de resetar reinicia a cero el contador.

Segunda parte: Cumple la misma funcion que en la parte uno, ademas que mediante un switch podes cambiar de modo, a contador o muestra los numeros primos.

Tercera parte: Se remplazó la funcion de numeros primos para mostrar el nivel de luz que detecta el fotodiodo en los displays cuando el switch está activado.


## investigacion de motor cc
MOTOR CC
Un motor de corriente continua (CC) es una máquina giratoria que convierte energía eléctrica en energía mecánica. Esta funcionalidad está basada en el principio de inducción, bajo el cual se crea una fuerza electromagnética a partir de una corriente de entrada que, a la vez, crea un movimiento giratorio.
El motor de corriente continua se clasifica en dos tipos, es decir, el motor de excitación independiente y el motor autoexcitación.
Un motor de corriente continua se compone principalmente de dos partes: El estátor (carcasa exterior) crea un campo magnético. El rotor es la parte interior que gira, alimentado con corriente directa a través de delgas, que están en contacto alternante con escobillas fijas.
La eficiencia de un motor de CC es la relación entre la potencia de entrada y la potencia de salida medida en vatios. Muchas de las piezas y partes del motor influyen (reduciendo el impacto) en la eficiencia del motor, teniendo como resultado el calor generado. Esto también es aplicable a temperaturas muy altas o bajas del entorno inmediato, las cuales a menudo forman parte de los entornos de trabajo de los actuadores industriales.
No obstante, existen maneras de garantizar la alta eficiencia de un motor en el caso de los motores de CC en general.
Con el fin de conseguir un rendimiento óptimo del motor, necesitará un suministro estable de alimentación y deberá asegurarse de que el cableado y la tensión de entrada son los correctos, ya que son igualmente importantes a la hora de obtener la mayor eficiencia posible.

## investigacion del sensor de flexión

Un sensor de flexión, también conocido como sensor de flexión o sensor de doblado, es un dispositivo diseñado para medir la flexión o el grado de curvatura en un objeto o estructura. Estos sensores se utilizan para detectar cambios en la forma de un objeto al aplicar fuerzas que inducen una flexión o curvatura en él. Por lo general, constan de materiales conductores que cambian su resistencia eléctrica cuando se doblan.

Cuando un sensor de flexión se dobla, la resistencia eléctrica en su interior cambia debido a la deformación del material conductor. Esto produce una señal eléctrica que puede ser medida y utilizada para determinar la cantidad de flexión o el ángulo de curvatura. Estos sensores son comunes en aplicaciones donde es necesario medir la flexión o la curvatura de objetos, como en la industria automotriz para controlar sistemas de seguridad, en dispositivos médicos para monitorizar la postura del cuerpo, en la robótica para controlar el movimiento de articulaciones, y en muchas otras aplicaciones.

Los sensores de flexión son versátiles y se pueden encontrar en diversas formas y tamaños, lo que les permite adaptarse a una amplia gama de situaciones y aplicaciones.

## Fotodiodo investigación:
Un fotodiodo es un semiconductor construido con una unión PN, sensible a la incidencia de la luz visible o infrarroja. Para que su funcionamiento sea correcto se polariza inversamente, con lo que se producirá una cierta circulación de corriente cuando sea excitado por la luz. Debido a su construcción, los fotodiodos se comportan como células fotovoltaicas, es decir, iluminados en ausencia de una fuente exterior de energía generan una corriente muy pequeña con el positivo en el ánodo y el negativo en el cátodo.

## Función principal
Esta funcion se encarga de encender y apagar los displays.

A, B, C, D, E ,F ,G son #define que utilizamos para prender los leds del displays, asociandolo a pines de la placa arduino.

(Breve explicación de la función)

~~~ C (lenguaje en el que esta escrito)
void prendeUnNumero(int digit)
{
  digitalWrite(A, LOW);
  digitalWrite(B, LOW);
  digitalWrite(C, LOW);
  digitalWrite(D, LOW);
  digitalWrite(E, LOW);
  digitalWrite(F, LOW);
  digitalWrite(G, LOW);
  switch (digit)
  {
    case 1:
    {
      digitalWrite(B, HIGH);
      digitalWrite(C, HIGH);
      break;
    }
    case 2:
    {
      digitalWrite(A, HIGH);
      digitalWrite(B, HIGH);
      digitalWrite(D, HIGH);
      digitalWrite(E, HIGH);
      digitalWrite(G, HIGH);
      break;
    }

    case 3:
    {
      digitalWrite(A, HIGH);
      digitalWrite(B, HIGH);
      digitalWrite(C, HIGH);
      digitalWrite(D, HIGH);
      digitalWrite(G, HIGH);
      break;
    }
    case 4:
    {
      digitalWrite(B, HIGH);
      digitalWrite(C, HIGH);
      digitalWrite(F, HIGH);
      digitalWrite(G, HIGH);
      break;
    }

    case 5:
    {
      digitalWrite(A, HIGH);
      digitalWrite(C, HIGH);
      digitalWrite(D, HIGH);
      digitalWrite(F, HIGH);
      digitalWrite(G, HIGH);
      break;
    }
    case 6:
    {
      digitalWrite(A, HIGH);
      digitalWrite(C, HIGH);
      digitalWrite(D, HIGH);
      digitalWrite(E, HIGH);
      digitalWrite(F, HIGH);
      digitalWrite(G, HIGH);
      break;
    }

    case 7:
    {
      digitalWrite(A, HIGH);
      digitalWrite(B, HIGH);
      digitalWrite(C, HIGH);
      break;
    }
    case 8:
    {
      digitalWrite(A, HIGH);
      digitalWrite(B, HIGH);
      digitalWrite(C, HIGH);
      digitalWrite(D, HIGH);
      digitalWrite(E, HIGH);
      digitalWrite(F, HIGH);
      digitalWrite(G, HIGH);
      break;
    } 
    case 9:
    {
      digitalWrite(A, HIGH);
      digitalWrite(B, HIGH);
      digitalWrite(C, HIGH);
      digitalWrite(D, HIGH);
      digitalWrite(F, HIGH);
      digitalWrite(G, HIGH);
      break;
    } 

    case 0:
    {
      digitalWrite(A, HIGH);
      digitalWrite(B, HIGH);
      digitalWrite(C, HIGH);
      digitalWrite(D, HIGH);
      digitalWrite(E, HIGH);
      digitalWrite(F, HIGH);
      break;
    }
  }
}

~~~

## :robot: Links del proyecto
- [proyecto parte 1](https://www.tinkercad.com/things/8yg0p5JViK7-tp1-parte-1/editel)
- [proyecto parte 2](https://www.tinkercad.com/things/4Iubwx2xzL8-tp1/editel)
- [proyecto parte 2 sensor](https://www.tinkercad.com/things/6Vz955WHeC8-copy-of-tp1/editel?tenant=circuits)





