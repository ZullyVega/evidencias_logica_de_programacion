<!-- No borrar o modificar -->
[Inicio](./index.md)

## Sesión 10 


<!-- Su documentación aquí -->

## Actividad: Prueba, ejecución y explicación de ejercicios de lógica de programación.

Selecciona dos ejercicios de la sesión 10, impleméntalos, ejecútalos y proporciona una explicación detallada de cada uno

### 1. Calcular la cantidad de materiales necesarios para construir una pared de ladrillos.

```

import java.util.Scanner;

public class CantidadLadrillos {
   public static void main(String[] args) {
      Scanner input = new Scanner(System.in);
      double largo, alto, ancho, areaPared, cantidadLadrillos, largoLadrillo, altoLadrillo, anchoLadrillo;
      
      // Solicita las dimensiones de la pared
      System.out.print("Ingrese el largo de la pared en metros: ");
      largo = input.nextDouble();
      System.out.print("Ingrese el alto de la pared en metros: ");
      alto = input.nextDouble();
      System.out.print("Ingrese el ancho de la pared en metros: ");
      ancho = input.nextDouble();

      // Solicita las dimensiones del ladrillo
      System.out.print("Ingrese el largo del ladrillo en metros: ");
      largoLadrillo = input.nextDouble();
      System.out.print("Ingrese el alto del ladrillo en metros: ");
      altoLadrillo = input.nextDouble();
      System.out.print("Ingrese el ancho del ladrillo en metros: ");
      anchoLadrillo = input.nextDouble();

      // Calcula el área de la pared y del ladrillo
      areaPared = largo * alto;
      double areaLadrillo = largoLadrillo * altoLadrillo;

      // Calcula la cantidad de ladrillos necesarios
      cantidadLadrillos = Math.ceil(areaPared / (areaLadrillo * ancho / anchoLadrillo));

      // Muestra el resultado en la consola
      System.out.printf("Para construir la pared se necesitan %.0f ladrillos.", cantidadLadrillos);
   }
}
```
Primero utilizamos la clase Scanner para leer la entrada del usuario desde la consola.
Se ingresa el tipo de dato, en este caso un double con los datos que se necesitan para calcular la cantidad de materiales para la construcción de una pared de ladrillos.
Se solicita al usuario que ingrese el largo, alto y ancho de la pared, y el largo, alto y ancho del ladrillo.
Luego se calcula el área de la pared y del ladrillo a través de la formula largo * alto
Luego se necesita calcular la cantidad de ladrillos necesarios, esto se realiza dividiendo el área de la pared entre el área del ladrillo y el ancho de la pared dividido por el ancho del ladrillo. Con la función Math.ceil redondeamos dicho resultado.
Para ver el resultado se utiliza el System.out.printf para dar formato a los datos que se imprimen.
El % indica que en esa posición se va a escribir el valor, el .0 indica el número de decimales que queremos observar y la f indica que el número es de tipo float o double. 

### 2. Calcular el movimiento rectilíneo uniforme

```

import java.util.Scanner;

public class MRU {
   public static void main(String[] args) {
      Scanner input = new Scanner(System.in);
      double velocidad, tiempo, distancia;
      
      // Solicita la velocidad y el tiempo
      System.out.print("Ingrese la velocidad en metros por segundo: ");
      velocidad = input.nextDouble();
      System.out.print("Ingrese el tiempo en segundos: ");
      tiempo = input.nextDouble();

      // Calcula la distancia recorrida
      distancia = velocidad * tiempo;

      // Muestra el resultado en la consola
      System.out.printf("La distancia recorrida es de %.2f metros.", distancia);
   }
}
```
Primero utilizamos la clase Scanner para leer la entrada del usuario desde la consola.
Se ingresa el tipo de dato, en este caso un double con los datos que se necesitan para calcular el movimiento rectilíneo uniforme.
Se solicita al usuario que ingrese la velocidad y el tiempo.
Luego se calcula la distancia a través de una multiplicación velocidad * tiempo.
Para ver el resultado se utiliza el System.out.printf para dar formato a los datos que se imprimen.
El % indica que en esa posición se va a escribir el valor, el .2 indica el número de decimales que queremos observar y la f indica que el número es de tipo float o double. 
