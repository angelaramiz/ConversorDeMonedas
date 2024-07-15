
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

## Contribuciones

Las contribuciones son bienvenidas. Por favor, sigue estos pasos:

1. Haz un fork del proyecto.
2. Crea una nueva rama (`git checkout -b feature/AmazingFeature`).
3. Realiza tus cambios y haz commit (`git commit -m 'Add some AmazingFeature'`).
4. Sube los cambios a tu rama (`git push origin feature/AmazingFeature`).
5. Abre un Pull Request.

## Contacto

Angel Aramiz - [angelaramiz22@gmail.com]

---

¡Gracias por usar ConversorDeMonedas
