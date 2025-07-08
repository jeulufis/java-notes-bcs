# Clases

Concepto fundamental, que sirve como plantilla para crear objetos, estos definen sus atributos(estructura) y metodos(comportamiento).

![image](https://github.com/user-attachments/assets/a9055930-a647-46ca-9ddb-1e2bfcc5b141)

# Ejemplo

```java
class Coche {
  String color;
  int puerta;
  int velocidad;
  
  // Constructor
  public Coche(String color, int puerta, int velocidad) {
    this.color = color;
    this.puerta = puerta;
    this.velocidad = velocidad;
  }
  
  public void arrancar() {
  }

  public void frenar() {
  }

  public void acelerar() {
    this.velocidad = this.velocidad + 1;
    System.out.println("Tu velocidad es 1 mayor:" +this.velocidad);
  }

  public void cambiarColor(String color) {
    this.color = color;
    System.out.println("Tu nuevo color es:" +this.color);
  }
}

public class Main {
  public static void main(String[] args) {
    Coche cochesito = new Coche("Amarillo", 4, 20);
    cochesito.acelerar();
    cochesito.cambiarColor("Rojo");
  }
}
```
