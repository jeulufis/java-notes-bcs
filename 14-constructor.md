# Constructor

Sirven para crear e inicializar objetos de una clase.

¿Para qué sirven los constructores?

- Inicializar atributos del objeto al momento de su creación.
- Permitir crear objetos con valores personalizados.
- Controlar cómo se crean las instancias (por ejemplo, puedes hacer que ciertos atributos sean obligatorios).

```java
class Fruta {
    String nombre;
    String color;
    int peso;
    
    public Fruta (String nombre, String color , int peso) {
        this.nombre = nombre;
        this.color = color;
        this.peso = peso;
    }
    
    void imprimePeso(){
        if(this.peso >= 2) {
            System.out.println("Esta fruta se exporta");
        } else {
            System.out.println("Esta fruta se queda");
        }
    }
}

public class Main {
  public static void main(String[] args) {
    Fruta manzana = new Fruta("Manzana", "Rojo", 2);
    manzana.imprimePeso();
  }
}
```   
