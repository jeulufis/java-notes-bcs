# ArrayList

El ArrayList es una de las estructuras de datos. Permite modificar y almacenar dinámicamente una colección de objetos.

```java
import java.util.ArrayList;

public class Main {
	public static void main(String[] args) {
		ArrayList <Integer> listaNumeros = new ArrayList<Integer>();
		
		listaNumeros.add(4);
		listaNumeros.add(10);
		
		System.out.println(listaNumeros); // [4, 10]
		System.out.println(listaNumeros.get(0)); // 4
		System.out.println(listaNumeros.get(1)); // 10
		
		System.out.println(listaNumeros.size()); // 3
		
		for(int i = 0; i < listaNumeros.size(); i++) {
		    System.out.println(listaNumeros.get(i));
		}
		
		int buscaNumeroDiez = listaNumeros.indexOf(10); // 1
		System.out.println(buscaNumeroDiez);
		
		boolean verdaderoSiExiste = listaNumeros.contains(10); // true
		System.out.println(verdaderoSiExiste);
	}
}
```

```java
class Frutas {
    String nombre;
    
    Frutas(String nombre) {
        this.nombre = nombre;
    }
    
    void muestraInfo() {
        System.out.println("Nombre: " + this.nombre);
    }

    @Override
    public String toString() {
        return "Fruta: " + nombre;
    }
}

public class Main {
    public static void main(String[] args) {
        ArrayList<Frutas> arrayFrutas = new ArrayList<Frutas>();
        
        Frutas frutaManzana = new Frutas("Manzana");
        Frutas frutaPera = new Frutas("Pera");
        arrayFrutas.add(frutaManzana);
        arrayFrutas.add(frutaPera);
        
        System.out.println(arrayFrutas); // Muestra lista completa
        arrayFrutas.get(0).muestraInfo(); // Muestra info específica
        arrayFrutas.get(1).muestraInfo();
        
        int contador = 0;
        
        for(int i = 0; i < arrayFrutas.size(); i++) {
            System.out.println(arrayFrutas.get(i));
            contador++;
        }
        
        System.out.print(contador);
    }
}

```
