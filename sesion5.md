<!-- No borrar o modificar -->
[Inicio](./index.md)

## Sesión 5 


<!-- Su documentación aquí -->

## Actividad 5: Ejercicios de bucles
Resolver los siguientes ejercicios:

### Ejercicios - while
- Pedir al usuario que ingrese un número y mostrar su tabla de multiplicar hasta el número 10.
```

import java.util.Scanner;

public class Act5 {

    public static void main(String[] args) {

        Scanner entradaDatos = new Scanner(System.in);
        System.out.println("Ingresar un número: ");
        int numero = entradaDatos.nextInt();

        int i = 1;
        while (i <= 10) {
            System.out.println(numero * i);
            i++;
        }
    }
}
```

- Pedir al usuario que ingrese una cadena de caracteres y contar la cantidad de caracteres que son números.
```

import java.util.Scanner;

public class Act5 {

    public static void main(String[] args) {

        Scanner sc = new Scanner(System.in);
        System.out.println("Ingrese una cadena de caracteres: ");
        String cadena = sc.nextLine();

        int i = 0;
        int contadorNumeros = 0;

        while (i < cadena.length()) {
            char caracter = cadena.charAt(i);
            if (caracter == '0' || caracter == '1' || caracter == '2' || caracter == '3' || caracter == '4'
                    || caracter == '5' || caracter == '6' || caracter == '7' || caracter == '8' || caracter == '9') {
                contadorNumeros++;
            }
            i++;
        }
        System.out.println("La cadena ingresada contiene " + contadorNumeros + " números.");
    }
}
```

### Ejercicios - do while
- Escribe un programa en Java que imprima los números del 1 al 100, pero que se detenga si el usuario introduce un número negativo.
```

import java.util.Scanner;

public class Act5 {

    public static void main(String[] args) {
        Scanner entradaDatos = new Scanner(System.in);

        int i;
        int detener = 0;

        do {
            i = 1;
            while (i <= 100) {
                System.out.println(i);
                i++;
            }
            System.out.println("Escriba un número negativo para detener o un número postivo para continuar");
            detener = entradaDatos.nextInt();
        } while (detener >= 0);
    }
}
```

- Escribe un programa en Java que pida al usuario un número entero e imprima la tabla de multiplicar de ese número, pero que se detenga si el usuario introduce el número 0.
```

import java.util.Scanner;

public class Act5 {

    public static void main(String[] args) {
        Scanner entradaDatos = new Scanner(System.in);

        int numero;
        int i = 1;

        do {
            System.out.println("Escriba un número o 0 para salir");
            numero = entradaDatos.nextInt();
            while (i <= 10) {
                System.out.println(numero * i);
                i++;
            }

        } while (numero > 0);
    }
}
```

### Ejercicios - for
- Imprimir los números impares del 1 al 50.
```

public class Act5 {

    public static void main(String[] args) {
        for (int i = 1; i <= 50; i += 2) {
            System.out.println(i);

        }
    }
}
```

- Imprimir los números primos del 1 al 100.
```

public class Act5 {

    public static void main(String[] args) {

        for (int i = 1; i <= 100; i++) {
            int x = 1;
            int contador = 0;
            while (x <= i) {
                if (i % x == 0) {
                    contador++;
                }
                x++;
            }
            if (contador == 2) {
                System.out.println(i + " Es primo");
            }

        }

    }
}
```





