<!-- No borrar o modificar -->
[Inicio](./index.md)

## Sesión 7 


<!-- Su documentación aquí -->

## Actividad: Ejecicios Array - ArrayList

Crear un ejemplo de Array y otro de ArrayList para visualizar sus diferencias.

### Array
```

public class Zully {

    public static void main(String[] args) {
        int[] numeros = {2, 3, 9, 10, 6, 15, 20};

        for (int i = 0; i < numeros.length; i++) {
            if (numeros[i] % 2 == 0) {
                System.out.println(numeros[i] + " Es par");
            } else {
                System.out.println(numeros[i] + " Es impar");
            }
        }
    }
}
```
### ArrayList
```

import java.util.ArrayList;
import java.util.Collections;

public class Actividad7 {

    public static void main(String[] args) {
        ArrayList<String> frutas = new ArrayList<>();

        frutas.add("Mango");
        frutas.add("Fresa");
        frutas.add("Sandia");
        frutas.add("Pera");
        frutas.add("Durazno");
        
        Collections.sort(frutas);
        
        for (String fruta : frutas) {
            System.out.println(fruta);
        }
        frutas.remove(2);
        System.out.println(frutas);
    }
}
```