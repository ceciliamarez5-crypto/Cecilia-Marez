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

/cgi-bin/
tareas.cpp # Backend en C++ (CGI)
tareas.cgi # Ejecutable compilado
/www/
index.html # Interfaz web
tareas.json # Almacenamiento de datos
README.md

yaml
Copiar código

---

## ▶️ Cómo ejecutar la solución

### 1️⃣ Requisitos

- Sistema operativo **Linux**
- **g++** instalado
- **Apache** con soporte CGI habilitado
- Navegador web

---

### 2️⃣ Compilar el backend

```bash
g++ tareas.cpp -o tareas.cgi
chmod +x tareas.cgi
Mover el archivo compilado a:

bash
Copiar código
/var/www/cgi-bin/
3️⃣ Configurar Apache (CGI)
Agregar o verificar la siguiente configuración:

apache
Copiar código
ScriptAlias /cgi-bin/ "/var/www/cgi-bin/"
<Directory "/var/www/cgi-bin">
    Options +ExecCGI
    AddHandler cgi-script .cgi
    Require all granted
</Directory>
Reiniciar Apache:

bash
Copiar código
sudo service apache2 restart
4️⃣ Ejecutar la aplicación
Abrir el navegador y acceder a:

arduino
Copiar código
http://localhost/index.html
Desde ahí se pueden agregar tareas y comunicarse con el backend en C++.

⚠️ Aclaraciones importantes
El backend está implementado en C++ usando CGI, una tecnología sencilla y adecuada para fines académicos.

No se utilizan librerías externas para manejar JSON.

El diseño es simple y enfocado en el aprendizaje.

No es una aplicación pensada para producción.

⭐ Extras
Persistencia de datos en archivo local

Comunicación HTTP básica

Backend web real en C++
👤 Autor

  Cecilia Marez
ejercicios tecnicos – Programación en C++






