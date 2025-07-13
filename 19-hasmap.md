# Hashmap

Un HashMap es una estructura de datos que almacena pares clave-valor. Es muy eficiente para buscar, insertar y eliminar datos en tiempo constante promedio.

```java
import java.util.HashMap;

public class Main {
    public static void main(String[] args) {
        // Crear un HashMap
        HashMap<String, Integer> edades = new HashMap<>();

        // Agregar elementos
        edades.put("Juan", 25);
        edades.put("Ana", 30);
        edades.put("Carlos", 28);

        // Acceder a un valor por su clave
        System.out.println("Edad de Ana: " + edades.get("Ana"));

        // Verificar si una clave existe
        if (edades.containsKey("Carlos")) {
            System.out.println("Carlos está en el mapa.");
        }

        // Eliminar un elemento
        edades.remove("Juan");

        // Recorrer el HashMap
        for (String nombre : edades.keySet()) {
            System.out.println(nombre + " tiene " + edades.get(nombre) + " años.");
        }
    }
}
```
