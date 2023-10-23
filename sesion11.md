<!-- No borrar o modificar -->
[Inicio](./index.md)

## Sesión 11 


<!-- Su documentación aquí -->

## Actividad: Ejercicios de Lógica de Programación

Basándose en el algoritmo 1 de la sesión 11, aplicar la siguiente variante: Dado un conjunto de números enteros, se debe determinar si existe algún número que aparezca más de una vez. Si es así, se deben imprimir todos los números que aparezcan más de una vez.

```

import java.util.ArrayList;

public class EjercicioZV {

    public static void main(String[] args) {
        int[] numeros = {1, 2, 3, 4, 5, 2, 4, 10, 12, 10};
        int numRepetido = 0;
        ArrayList<Integer> numerosRepetidos = new ArrayList<>();

        for (int i = 0; i < numeros.length; i++) {
            for (int j = 0; j < i; j++) {
                if (numeros[i] == numeros[j]) {
                    numRepetido = numeros[i];
                    if (numeros[i] == numeros[j] && !numerosRepetidos.contains(numeros[i]));
                    numerosRepetidos.add(numeros[i]);
                    break;

                }
            }
        }
        if (numRepetido != 0) {
            System.out.println("Los números repetidos son: " + numerosRepetidos);
        } else {
            // No hay ningún número repetido
            System.out.println("No hay ningún número repetido");
        }
    }
}
```

Desarrollar un algoritmo que realice la conversión de binario a decimal.




