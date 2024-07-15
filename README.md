# ConversorDeMonedas

Este proyecto es una aplicación de conversión de monedas desarrollada en Java. La aplicación permite consultar tasas de cambio y convertir entre diferentes monedas de manera sencilla.

## Estructura del Proyecto

- `ConsultarMoneda.java`: Clase que se encarga de consultar las tasas de cambio actuales desde una API externa.
- `ConvertirMonedas.java`: Clase que realiza la conversión entre las diferentes monedas utilizando las tasas de cambio obtenidas.
- `Monedas.java`: Clase que define los diferentes tipos de monedas que se pueden convertir.
- `Principal.java`: Clase principal que contiene el método `main` para ejecutar la aplicación.

## Bibliotecas Utilizadas

- [Gson](https://github.com/google/gson): Biblioteca de Java para convertir objetos Java a su representación JSON y viceversa.

## Requisitos

- Java 17
- Maven 2.8.9

## Instalación

1. Clona el repositorio:
    ```sh
    git clone https://github.com/angelaramiz/ConversorDeMonedas.git
    ```
2. Navega al directorio del proyecto:
    ```sh
    cd ConversorDeMonedas
    ```
3. Compila el proyecto con Maven:
    ```sh
    mvn clean install
    ```

## Uso

1. Ejecuta la aplicación:
    ```sh
    java -jar target/ConversorDeMonedas-1.0-SNAPSHOT.jar
    ```
2. Sigue las instrucciones en la consola para consultar y convertir monedas.

## Ejemplo de Uso

```java
public class Principal {
    public static void main(String[] args) {
        Monedas moneda = new Monedas();
        ConvertirMonedas convertir = new ConvertirMonedas();

        // Consultar tasa de cambio
        double tasa = ConsultarMoneda.obtenerTasa("USD", "EUR");
        System.out.println("Tasa de cambio USD a EUR: " + tasa);

        // Convertir monedas
        double cantidadConvertida = convertir.convertir("USD", "EUR", 100);
        System.out.println("100 USD en EUR: " + cantidadConvertida);
    }
}
