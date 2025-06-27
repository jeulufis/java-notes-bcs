# Switch

El switch en Java es una estructura de control que permite ejecutar diferentes bloques de código según el valor de una expresión. Es una alternativa al uso de múltiples sentencias if-else cuando se desea comparar una variable con varios valores posibles.

```java
public class EjemploSwitch {

    public static void main(String[] args) {
        // Ejemplo con int
        int dia = 3;

        switch (dia) {
            case 1:
                System.out.println("Lunes");
                break;
            case 2:
                System.out.println("Martes");
                break;
            case 3:
                System.out.println("Miércoles");
                break;
            default:
                System.out.println("Día no válido");
        }

        // Ejemplo con String
        String fruta = "manzana";

        switch (fruta) {
            case "naranja":
                System.out.println("Es una naranja");
                break;
            case "manzana":
                System.out.println("Es una manzana");
                break;
            default:
                System.out.println("Fruta desconocida");
        }
    }
}

```
