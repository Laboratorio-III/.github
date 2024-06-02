### Trabajo Práctico: Implementación de un Chat Multiusuario en Python

#### Descripción del Trabajo

El objetivo de este trabajo práctico es desarrollar un programa de chat multiusuario en Python, utilizando hilos para manejar múltiples conexiones simultáneas. El intercambio de mensajes debe realizarse en formato JSON y seguir un protocolo de comunicación específico. El programa debe contar con funcionalidades básicas de un mensajero, como enviar mensajes a todos los usuarios conectados y enviar mensajes a un usuario específico. Además, debe incluir una interfaz gráfica de usuario (GUI) para facilitar la interacción.

#### Requisitos

##### Para Aprobar:

1. **Implementación de Hilos**:
  
  - El programa debe utilizar hilos para gestionar múltiples conexiones de usuarios simultáneamente.
2. **Intercambio de Mensajes en Formato JSON**:
  
  - Los mensajes deben intercambiarse en formato JSON.
    
  - Se debe especificar y seguir un protocolo de intercambio de mensajes. Por ejemplo:
    
    - Mensaje a todos los usuarios:
      
      ```json
      {
          "tipo": "broadcast",
          "origen": "mi_nick",
          "memsaje": "mensaje"
      }
      ```
      
    - Mensaje a un usuario específico:
      
      ```json
      {
          "tipo": "privado",
          "origen": "mi_nick",
          "destino": "nick",
          "mensaje": "mensaje"
      }
      ```
      
3. **Enviar Mensajes a Todos los Usuarios Conectados**:
  
  - Implementar la funcionalidad para que un usuario pueda enviar mensajes que serán recibidos por todos los usuarios conectados.
4. **Enviar Mensajes a un Usuario Específico**:
  
  - Implementar la funcionalidad para que un usuario pueda enviar mensajes privados a otro usuario específico conectado.
5. **Cliente con Interfaz Gráfica de Usuario (GUI)**:
  
  - Desarrollar una GUI para el cliente de chat que permita a los usuarios intercambiar mensajes de forma intuitiva.
6. **Uso de Sockets TCP**:
  
  - Implementar el servidor utilizando sockets TCP para asegurar una comunicación confiable entre los clientes y el servidor.

##### Para Promocionar:

1. **Implementación de una Base de Datos**:
  
  - Utilizar SQLite para implementar una base de datos.
    
  - La base de datos debe contener al menos una tabla de usuarios para autenticación.
    
  - Ejemplo de tabla de usuarios:
    
    ```sql
    CREATE TABLE users (
        id INTEGER PRIMARY KEY AUTOINCREMENT,
        username TEXT NOT NULL UNIQUE,
        password TEXT NOT NULL
    );
    ```
    
2. **Programación Orientada a Objetos (POO)**:
  
  - El programa debe seguir principios de POO.
  - Organizar el código en clases y objetos adecuados para la funcionalidad del chat.

#### Entregables

1. Código fuente del servidor de chat.
2. Código fuente del cliente de chat con GUI.
3. Esquema de la base de datos y scripts de inicialización (si corresponde).
4. Documentación del protocolo de intercambio de mensajes.
5. Instrucciones claras para ejecutar el programa.

#### Pautas de Evaluación

- **Funcionalidad Básica**: Se evaluará la correcta implementación de los hilos, el intercambio de mensajes en formato JSON, y las funcionalidades de envío de mensajes tanto a todos los usuarios como a un usuario específico.
- **Interfaz Gráfica de Usuario**: Se evaluará la usabilidad y funcionalidad de la GUI del cliente.
- **Uso de Base de Datos**: Para los alumnos que busquen la promoción, se evaluará la correcta implementación de la base de datos SQLite y su integración con el programa.
- **Programación Orientada a Objetos**: Se evaluará el uso adecuado de POO en el diseño e implementación del programa.
- **Uso de Sockets TCP**: Se evaluará la correcta implementación y uso de sockets TCP para garantizar una comunicación confiable entre el servidor y los clientes.

#### Recursos Sugeridos

- **Bibliotecas de Python**:
  
  - `socket` para la comunicación en red.
  - `threading` para la gestión de hilos.
  - `json` para el intercambio de mensajes en formato JSON.
  - `sqlite3` para la gestión de la base de datos.
  - `tkinter` o `PyQt` para la creación de la GUI.
- **Documentación**:
  
  - [Documentación de Python](https://docs.python.org/3/)
  - [Guía de SQLite](https://www.sqlite.org/docs.html)
  - [Tutorial de Tkinter](https://docs.python.org/3/library/tkinter.html)
  - [Tutorial de PyQt](https://www.riverbankcomputing.com/static/Docs/PyQt5/)

Este trabajo práctico tiene como objetivo proporcionar una experiencia completa en el desarrollo de aplicaciones de red, manejo de concurrencia, desarrollo de interfaces gráficas y uso de bases de datos, siguiendo principios de programación orientada a objetos.
Apuntes para Laboratorio de programación 3
## Temas
- git
  * Clonado de repositorios remotos. Comandos status, fetch, merge, add, push.
- markdown
  * Titulos, Citas, énfacis, listas , listas numeradas, código, link, imagenes, links. 
-Entonros Virtuals, Intalador de paquetes para Python (pip)
  * pip\: list. install, freeze
  * virtualenv
- Modelo OSI
- Estándar TCP/IP
- Cliente/Servidor en Python
- Servidores WEB
- ECMA-404 The JSON Data Interchange Standard.
- API-REST
- Frontend/Backend
- RSA
