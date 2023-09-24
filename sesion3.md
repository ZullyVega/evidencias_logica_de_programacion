<!-- No borrar o modificar -->
[Inicio](./index.md)

## Sesión 3 


<!-- Su documentación aquí -->

## Actividad 3: Ejercicios de operaciones básicas en Java.

- Suma y multiplicación: Escribe un programa que solicite al usuario dos números enteros y luego imprima la suma y multiplicación de esos números.

```

import java.util.Scanner;

public class Zully {

    public static void main(String[] args) {
        Scanner entradaDatos = new Scanner(System.in);

        System.out.println("Ingrese el primer numero: ");
        int num1 = entradaDatos.nextInt();

        System.out.println("Ingrese el segundo numero: ");
        int num2 = entradaDatos.nextInt();

        int suma = num1 + num2;
        int multiplicacion = num1 * num2;

        System.out.println("la suma es " + suma);
        System.out.println("la multiplicacion es " + multiplicacion);
    }
}
```

- Resta y división: Escribe un programa que tome dos números enteros ingresados por el usuario y calcule la resta y división de esos números.

```

import java.util.Scanner;

public class Zully {

    public static void main(String[] args) {
        Scanner entradaDatos = new Scanner(System.in);

        System.out.println("Ingrese el primer numero: ");
        int num1 = entradaDatos.nextInt();

        System.out.println("Ingrese el segundo numero: ");
        int num2 = entradaDatos.nextInt();

        int resta = num1 - num2;
        int division = num1 / num2;

        System.out.println("la resta es " + resta);
        System.out.println("la division es " + division);
    }
}
```

- Operaciones combinadas: Escribe un programa que solicite al usuario tres números enteros y realice las siguientes operaciones: suma de los tres números, multiplicación del primer número por el segundo y división del resultado entre el tercer número.

```

import java.util.Scanner;

public class Zully {

    public static void main(String[] args) {
        Scanner entradaDatos = new Scanner(System.in);

        System.out.println("Ingrese el primer numero: ");
        int num1 = entradaDatos.nextInt();

        System.out.println("Ingrese el segundo numero: ");
        int num2 = entradaDatos.nextInt();

        System.out.println("Ingrese el tercer numero: ");
        int num3 = entradaDatos.nextInt();

        int suma = num1 + num2 + num3;
        int multiplicacion = num1 * num2;
        int division = ((num1 * num2) / num3);

        System.out.println("la suma es " + suma);
        System.out.println("la multiplicacion es " + multiplicacion);
        System.out.println("la division es " + division);

    }
}
```

- Operaciones con decimales: Escribe un programa que solicite al usuario dos números decimales y realice las siguientes operaciones: suma, resta, multiplicación y división.

```

import java.util.Scanner;

public class Zully {

    public static void main(String[] args) {
        Scanner entradaDatos = new Scanner(System.in);

        System.out.println("Ingrese el primer numero decimal: ");
        double num1 = entradaDatos.nextDouble();

        System.out.println("Ingrese el segundo numero decimal: ");
        double num2 = entradaDatos.nextDouble();

        double suma = num1 + num2;
        double resta = num1 - num2;
        double multiplicacion = num1 * num2;
        double division = num1 / num2;

        System.out.println("la suma es " + suma);
        System.out.println("la resta es " + resta);
        System.out.println("la multiplicacion es " + multiplicacion);
        System.out.println("la division es " + division);

    }
}
```

- Incremento y decremento: Escribe un programa que declare una variable entera y la inicialice con un valor. Luego, incrementa su valor en 1 y muestra el resultado. Después, decrementa su valor en 1 y muestra el resultado nuevamente.

```

public class Zully {

    public static void main(String[] args) {

        int numero = 150;
        numero++;
        
        System.out.println("El número inicial es 150, se incrementa a: " + numero);
        
    }
}
```

```

public class Zully {

    public static void main(String[] args) {

        int numero = 150;
        numero--;
        
        System.out.println("El número inicial es 150, se decrementa a: " + numero);
        
    }
}
```

- Operador de asignación compuesta: Escribe un programa que declare una variable entera y la inicialice con un valor. Utiliza el operador de asignación compuesta para sumar 5 a la variable y luego mostrar su valor.

```

public class Zully {

    public static void main(String[] args) {

        int edad;
        edad =25;
        
        int suma = edad +=5;
        System.out.println("La suma es " + suma);
        
    }
}
```

- Operadores lógicos: Escribe un programa que tome dos valores booleanos ingresados por el usuario y muestre el resultado de las operaciones lógicas AND, OR y NOT entre esos valores.

```

import java.util.Scanner;

public class EjercicioZV {

    public static void main(String[] args) {
        Scanner entradaDatos = new Scanner(System.in);
        System.out.println("Es mayor de edad: ");
        boolean edad = entradaDatos.nextBoolean();

        System.out.println("Es estudiante: ");
        boolean estudiante = entradaDatos.nextBoolean();

        boolean resultado1 = edad && estudiante;
        boolean resultado2 = edad || estudiante;
        boolean resultado3 = !edad;
        boolean resultado4 = !estudiante;

        System.out.println("El resultado 1 es: " + resultado1);
        System.out.println("El resultado 2 es: " + resultado2);
        System.out.println("El resultado 3 es: " + resultado3);
        System.out.println("El resultado 4 es: " + resultado4);

    }
}
```

- Operador ternario: Escribe un programa que tome un número entero ingresado por el usuario y utilice el operador ternario para determinar si el número es positivo o negativo. Luego, muestra el resultado en la salida.

```

import java.util.Scanner;

public class EjercicioZV {

    public static void main(String[] args) {
        Scanner entradaDatos = new Scanner(System.in);

        System.out.println("Ingrese un número: ");
        int numero = entradaDatos.nextInt();

        String resultado = (numero >= 0) ? "Positivo" : "Negativo";

        System.out.println("El número es: " + resultado);

    }
}
```



