# Encapsulamiento

La encapsulación permite ocultar la complejidad interna de una clase, proporcionando una interfaz controlada para interactuar con los objetos.

Cuando las variables son private no hay acceso directo desde otra clase.

```java
class Persona {
    private String nombre;
    private String apellido;
    public int edad;
    
    Persona (String nombre, String apellido, int edad) {
        this.nombre = nombre;
        this.apellido = apellido;
        this.edad = edad;
    }
    
    public String getNombre () {
        return this.nombre;
    }
    
    public String getApellido() {
        return this.apellido;
    }
    
    public void setNombre (String nombre) {
        this.nombre = nombre;
    }
    
    public void setApellido (String apellido) {
        this.apellido = apellido;    
    }
}

public class Main {
  public static void main(String[] args) {
      Persona personaUno = new Persona("Juan", "Eulufi", 23);
      System.out.println("Nombre: " +personaUno.getNombre() +" Apellido: " +personaUno.getApellido());
  }
}

```
