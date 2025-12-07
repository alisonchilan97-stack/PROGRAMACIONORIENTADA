
ABSTRACCION 
// Clase abstracta que define lo esencial de un vehículo
abstract class Vehiculo {
    abstract void encender();   // Método abstracto
    abstract void apagar();     // Método abstracto
}

// Clase concreta que implementa solo lo necesario
class Auto extends Vehiculo {

    @Override
    void encender() {
        System.out.println("El auto se está encendiendo...");
    }

    @Override
    void apagar() {
        System.out.println("El auto se ha apagado.");
    }
}

public class Main {
    public static void main(String[] args) {
        Vehiculo miAuto = new Auto();
        miAuto.encender();
        miAuto.apagar();
    }
}
