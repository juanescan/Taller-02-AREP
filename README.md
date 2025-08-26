# Taller-02-AREP

## Gestor de Tareas - Servidor Web en Java

Este proyecto consiste en un framework web ligero desarrollado en Java, diseñado para facilitar la creación de aplicaciones web que integren servicios REST y la gestión de archivos estáticos (HTML, CSS, JavaScript, imágenes, entre otros).

El framework ofrece:

- Mecanismos sencillos para definir rutas REST mediante funciones lambda.

- Configuración flexible para establecer la ubicación de los archivos estáticos que el servidor expone

- Eliminar tareas con un clic.

- Persistencia en memoria (las tareas se manejan en un arreglo JSON durante la ejecución del servidor).

## ⚙️ Instalación

1. Clona este repositorio o descarga los archivos:  
   ```bash
   git clone https://github.com/juanescan/Taller-01-AREP.git
   cd Taller-01-AREP
2. Compila el proyecto con Maven:
   ```bash
   mvn clean install
3. Asegúrate de tener Java 11+ y Maven instalados.
## ▶️ Ejecución
     mvn exec:java -Dexec.mainClass="eci.arep.juancancelado.mavenproject1.HttpServer"

 El servidor se ejecutará en el puerto 8080:
 
 👉 http://localhost:8080

 ## 🏗️ Arquitectura

El sistema está compuesto por dos capas principales:

1. Servidor HTTP en Java (Backend)

- Maneja conexiones mediante ServerSocket.

- Responde archivos estáticos desde la carpeta public/.

- Expone un API REST /tasks con soporte para:

- GET /tasks → Listar tareas en JSON.

- POST /tasks?name=X&type=Y → Agregar tarea.

- DELETE /tasks?name=X&type=Y → Eliminar tarea.

2. Aplicación Web (Frontend)
- index.html: interfaz gráfica.

- style.css: estilos.

- script.js: comunicación con el servidor usando fetch() (asíncrono).

- La lista de tareas se actualiza dinámicamente en la página.

## Pruebas
 
 ![imagenes](/imagenes/prueba1.png)

![imagenes](/imagenes/prueba2.png)

## APP

![App](/imagenes/APP1.png)

![App](/imagenes/APP2.png)

![App](/imagenes/APP3.png)

![App](/imagenes/APP4.png) 

![App](/imagenes/APP5.png) 

## Built With

- Java SE - Lenguaje de programación

- Maven - Herramienta de gestión de dependencias y construcción

## Authors 
- Juan Esteban Cancelado Sanchez - *AREP* *Taller 1* - [juanescan](https://github.com/juanescan)