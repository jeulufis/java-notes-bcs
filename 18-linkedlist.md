# LinkedList

LinkedList es una estructura de datos lineal.

```java
import java.util.LinkedList;

public class Main {
	public static void main(String[] args) {
	    	LinkedList<String> lista = new LinkedList<String>();
	    	lista.add("A");
	    	lista.add("B");
	    	lista.add("C");
	    	lista.add("D");
	    	
	    	lista.addFirst("Inicio:");
	    	lista.addLast("Fin");
	    	
	    	for(int i = 0; i < lista.size(); i++) {
	    	    System.out.println(lista.get(i));
	    	}
	    	
	    	System.out.println("Primero:" +lista.getFirst());
	    	System.out.println("Ultimo:" +lista.getLast());
	    	
	    	// Remover primero o ultimo
	    	// lista.removeFirst();
	    	// lista.removeLast();
	}
}
```
