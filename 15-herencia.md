# Herencia

Permite que una clase herede atributos y métodos de otra clase.

```java
class Trabajador {
  String nombre;
  int sueldo;

  Trabajador(String nombre, int sueldo) {
    this.nombre = nombre;
    this.sueldo = sueldo;
  }

  void informacion() {
    System.out.println("Nombre: " + nombre);
    System.out.println("Sueldo: $" + sueldo);
  }
}

class Profesor extends Trabajador {
  String profesion;

  Profesor(String nombre, int sueldo, String profesion) {
    super(nombre, sueldo);
    this.profesion = profesion;
  }

  void informacion() {
    super.informacion();
    System.out.println("Profesión: " + profesion);
  }
}

class Medico extends Trabajador {
  String profesion;

  Medico(String nombre, int sueldo, String profesion) {
    super(nombre, sueldo);
    this.profesion = profesion;
  }

  void informacion() {
    super.informacion();
    System.out.println("Estudió: " + profesion);
  }
}

public class Main {
  public static void main(String[] args) {
    Profesor profesorInformatico = new Profesor("Juan", 100, "Ing. Informático");
    profesorInformatico.informacion();

    System.out.println("--------");

    Medico medico = new Medico("David", 1000, "Medicina");
    medico.informacion();
  }
}

```
