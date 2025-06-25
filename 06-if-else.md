# Sentencias de Control

Permite ejecutar diferentes bloques de codigos dependiendo si su valor es verdadero o falso.

```java
public main() {
  public static void main(String[] args) {
     int hora = 24;
        
    if (hora <= 12) {
      System.out.println("Buenos dias");
    } else if (hora >= 13 && hora <= 18) {
      System.out.println("Buenas tardes");
    } else {
      System.out.println("Buenas noches");
    }
  }
}
```
