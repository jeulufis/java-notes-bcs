# For each

```java
import java.util.ArrayList;
import java.util.HashMap;

public class Main {
    public static void main(String[] args) {
        // Arreglo de enteros
        int[] numeros = {1, 2, 3, 4};
        for (int i : numeros) {
            System.out.println(i);
        }

        // Arreglo de cadenas
        String[] nombres = {"Juan", "Javiera"};
        for (String nombre : nombres) {
            System.out.println(nombre);
        }

        // ArrayList de frutas
        ArrayList<String> arrayFrutas = new ArrayList<>();
        arrayFrutas.add("Manzana");
        arrayFrutas.add("Pera");
        for (String fruta : arrayFrutas) {
            System.out.println(fruta);
        }

        // HashMap con deportes y cantidades
        HashMap<String, Integer> cantidadPelotas = new HashMap<>();
        cantidadPelotas.put("Futbol", 10);
        cantidadPelotas.put("Basquet", 20);
        for (String deporte : cantidadPelotas.keySet()) {
            int cantidad = cantidadPelotas.get(deporte);
            System.out.println(deporte + ": " + cantidad);
        }
    }
}

```
