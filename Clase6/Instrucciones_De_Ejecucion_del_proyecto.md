# Guía de Instalación y Ejecución del Proyecto fxJava

## Requisitos Previos

Antes de clonar y ejecutar el proyecto, asegúrate de tener instaladas
las siguientes herramientas en tu sistema:

-   Java JDK 17 o superior\
    Verifica la instalación ejecutando:

    ``` bash
    java -version
    ```

-   Apache Maven 3.8+\
    Verifica la instalación ejecutando:

    ``` bash
    mvn -version
    ```

-   Git\
    Verifica la instalación ejecutando:

    ``` bash
    git --version
    ```

-   IDE recomendado:

    -   IntelliJ IDEA\
    -   VS Code con la extensión Java Extension Pack\
    -   Eclipse con soporte para JavaFX y Maven

------------------------------------------------------------------------
# Enlace del Proyecto

Puedes acceder al repositorio del proyecto en el siguiente enlace:

[https://github.com/alen1238/fxJava.git](https://github.com/alen1238/fxJava.git)

---

## Clonar el Repositorio

Abre una terminal y ejecuta el siguiente comando para clonar el proyecto
desde GitHub:

``` bash
git clone https://github.com/alen1238/fxJava.git
```

Luego, entra en el directorio del proyecto:

``` bash
cd fxJava
```

------------------------------------------------------------------------

## Compilar el Proyecto

Compila las dependencias y verifica que todo esté correctamente
configurado:

``` bash
mvn clean install
```

------------------------------------------------------------------------

## Ejecutar la Aplicación

Para ejecutar el proyecto JavaFX con Maven, utiliza el siguiente
comando:

``` bash
mvn javafx:run
```

Esto iniciará la aplicación JavaFX localmente, cargando la interfaz
gráfica definida en el proyecto.

------------------------------------------------------------------------

## Estructura del Proyecto

    fxJava/
    ├── src/
    │   ├── main/
    │   │   ├── java/            # Código fuente del proyecto
    │   │   ├── resources/       # Archivos FXML, imágenes y estilos CSS
    │   └── test/                # Pruebas unitarias
    ├── pom.xml                  # Archivo de configuración Maven
    └── README.md                # Documentación del proyecto

------------------------------------------------------------------------

## Notas Adicionales

-   Si usas IntelliJ IDEA, asegúrate de configurar el SDK de Java 17 en:

        File > Project Structure > Project SDK

-   En caso de errores con JavaFX, verifica que el plugin
    `javafx-maven-plugin` esté correctamente definido en el archivo
    `pom.xml`.

-   Si deseas ejecutar desde el IDE, selecciona la clase principal y
    ejecútala como *JavaFX Application*.
