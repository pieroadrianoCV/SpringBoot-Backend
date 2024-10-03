
# Proyecto Demo para Spring Boot

Este es un proyecto de demostración para explorar las funcionalidades de Spring Boot. Incluye dependencias para construir aplicaciones web y escribir pruebas unitarias. El proyecto utiliza Maven para la gestión de dependencias y la automatización del proceso de compilación.

## Información del Proyecto
- **Nombre del proyecto**: Demo
- **Versión**: 0.0.1-SNAPSHOT
- **Descripción**: Un proyecto demo de Spring Boot que muestra las características básicas del desarrollo web.
- **Proyecto Padre**: Hereda de `spring-boot-starter-parent` (versión 3.3.4), lo que simplifica la configuración proporcionando ajustes predeterminados para aplicaciones Spring Boot.
- **Versión de Java**: 17

## Compilación y Construcción
Este proyecto utiliza **Java 17** para la compilación y Maven como herramienta de construcción. La configuración de Maven es la predeterminada, y el proceso de construcción está gestionado por el plugin de Maven para Spring Boot.

### Detalles del Compilador:
- **Lenguaje**: Java 17
- **Compilador de Maven**: Configurado para Java 17.

## Dependencias
El proyecto hace uso de varias dependencias clave gestionadas por Maven:

1. **Spring Boot Starter Web** (`spring-boot-starter-web`):
   - Proporciona todas las bibliotecas necesarias para construir un servicio web RESTful utilizando Spring Boot.

2. **Spring Boot Starter Test** (`spring-boot-starter-test`):
   - Alcance: `test`
   - Incluye bibliotecas para probar la aplicación, como JUnit y Mockito, que se utilizan durante la fase de pruebas.

## Plugins de Maven
Se utiliza el siguiente plugin para construir y empaquetar la aplicación Spring Boot:

- **Spring Boot Maven Plugin** (`spring-boot-maven-plugin`):
  - Este plugin permite construir la aplicación en un archivo JAR ejecutable, lo que facilita ejecutar la aplicación Spring Boot como un servicio independiente.

## **Tutorial: Configuración de Spring Boot con Maven en Visual Studio Code**

### **Paso 1: Descargar e Instalar Java 17**

1. **Descargar JDK 17**:
   - Ve a la página oficial de [Oracle](https://www.oracle.com/java/technologies/javase-jdk17-downloads.html) o [AdoptOpenJDK](https://adoptopenjdk.net/).
   - Descarga la versión correspondiente a tu sistema operativo (Windows, macOS, Linux).

2. **Instalar JDK 17**:
   - Ejecuta el instalador descargado y sigue las instrucciones.
   - Asegúrate de agregar Java al **PATH** (debería hacerse automáticamente durante la instalación, pero verifica si no lo está).

3. **Verificar la instalación**:
   - Abre una terminal o símbolo del sistema (CMD) y escribe:
     ```bash
     java -version
     ```
   - Deberías ver algo como:
     ```bash
     java version "17.0.x"
     ```

### **Paso 2: Descargar e Instalar Maven**

1. **Descargar Maven**:
   - Ve al sitio oficial de Apache Maven: [https://maven.apache.org/download.cgi](https://maven.apache.org/download.cgi).
   - Descarga la versión binaria `.zip` o `.tar.gz` más reciente.

2. **Instalar Maven**:
   - Extrae los archivos en un directorio de tu elección (por ejemplo, `C:\Program Files\Maven`).
   - Agrega la carpeta `bin` de Maven a la variable de entorno `PATH`.
     - En Windows, ve a **Configuración del Sistema > Variables de entorno**.
     - Agrega la ruta a la carpeta `bin` de Maven.

3. **Verificar la instalación**:
   - Abre una terminal o símbolo del sistema (CMD) y escribe:
     ```bash
     mvn -version
     ```
   - Deberías ver la versión de Maven y la versión de Java utilizada.

### **Paso 3: Instalar Visual Studio Code y Extensiones**

1. **Descargar e Instalar Visual Studio Code**:
   - Ve al sitio oficial de VS Code: [https://code.visualstudio.com/](https://code.visualstudio.com/).
   - Descarga la versión para tu sistema operativo e instálala.

2. **Instalar Extensiones Requeridas**:
   - Abre VS Code y navega a la sección de **Extensiones** (icono de cuadrito en la barra lateral o `Ctrl+Shift+X`).
   - Busca e instala las siguientes extensiones:
     - **Extension Pack for Java** (incluye las herramientas necesarias para desarrollo en Java).
     - **Spring Boot Extension Pack** (para trabajar con Spring Boot).
     - **Maven for Java** (gestión de proyectos Maven).

### **Paso 4: Crear un Proyecto Maven con Spring Boot en Visual Studio Code**

1. **Iniciar la creación del proyecto con Spring Initializr**:
   - Una vez que tengas las extensiones instaladas en Visual Studio Code, presiona `Ctrl + Shift + P` para abrir la paleta de comandos.
   - En la barra de búsqueda que aparece, escribe y selecciona: **"Spring Initializr: Create a Maven Project..."**.
   
2. **Configurar el Proyecto**:
   - **Versión de Spring Boot**: Elige la versión `3.3.4`.
   - **Lenguaje del proyecto**: Selecciona `Java`.
   - **Nombre del Grupo**: Introduce `example.com`.
   - **ID del Proyecto**: Introduce `demo`.
   - **Tipo de empaquetado**: Selecciona `JAR`.
   - **Versión de Java**: Selecciona `17`.

3. **Seleccionar Dependencias**:
   - En la siguiente pantalla, selecciona la dependencia **Spring Web**.

4. **Elegir Carpeta de Proyecto**:
   - Selecciona la carpeta donde deseas guardar el proyecto en tu máquina.

Una vez completados estos pasos, Visual Studio Code generará automáticamente tu proyecto Maven con Spring Boot configurado y listo para compilar.