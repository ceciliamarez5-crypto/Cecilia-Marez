# Cecilia-Marez
# 📝 Mini Aplicación To-Do – Backend en C++

Mini aplicación de tareas (To-Do) desarrollada en **C++**, con un **backend web usando CGI** y una **interfaz web simple en HTML**.  
La información se almacena de forma persistente en un **archivo local (`tareas.json`)**.

---

## 🚀 Funcionalidades

- Agregar tareas
- Listar tareas
- Guardar tareas en archivo local (JSON simple)
- Backend web implementado en C++
- Interfaz web básica

---

## 🛠️ Tecnologías utilizadas

- **C++**
- **CGI (Common Gateway Interface)**
- **Apache**
- **HTML**
- **Archivo local (JSON)**

---

## 📂 Estructura del proyecto

---

##  Cómo ejecutar la solución

### 1 Requisitos

- Sistema operativo **Linux**
- **g++** instalado
- **Apache** con soporte CGI habilitado
- Navegador web

---

### 2️ Compilar el backend

```bash
g++ tareas.cpp -o tareas.cgi
chmod +x tareas.cgi

Mover el archivo compilado a:

/var/www/cgi-bin/
Ejecutar la aplicación

Abrir el navegador y acceder a:

http://localhost/index.html


Desde ahí se pueden agregar tareas y comunicarse con el backend en C++.

Aclaraciones importantes

El backend está implementado en C++ usando CGI, una tecnología sencilla y adecuada para fines académicos.

No se utilizan librerías externas para manejar JSON.

El diseño es simple y enfocado en el aprendizaje.

No es una aplicación pensada para producción.

 Extras

Persistencia de datos en archivo local

Comunicación HTTP básica

Backend web real en C++

👤 Autor

  Cecilia Marez
ejercicios tecnicos – Programación en C++






