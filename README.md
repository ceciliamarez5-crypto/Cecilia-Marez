# Cecilia-Marez
# 📌 Mini Aplicación To-Do – Backend en C++
📖 Descripción

Este proyecto es una mini aplicación de tareas (To-Do) desarrollada en C++, con:

Backend web implementado mediante CGI en C++

Interfaz web simple en HTML

Almacenamiento de datos en un archivo local (tareas.json)

La aplicación permite:

Agregar tareas

Listar tareas

Guardar la información de forma persistente en un archivo

🛠️ Requisitos

Sistema operativo Linux

Compilador g++

Servidor web Apache con soporte CGI habilitado

Navegador web moderno

📂 Estructura del proyecto
/cgi-bin/
   tareas.cpp   → Backend en C++ (CGI)
   tareas.cgi   → Ejecutable compilado
/www/
   index.html   → Interfaz web
tareas.json     → Archivo de almacenamiento

▶️ Cómo ejecutar la solución
1️⃣ Compilar el backend en C++

Desde la terminal:

g++ tareas.cpp -o tareas.cgi
chmod +x tareas.cgi


Colocar el archivo tareas.cgi dentro del directorio:

/var/www/cgi-bin/

2️⃣ Configurar Apache para CGI

Verificar que Apache tenga habilitado CGI con la siguiente configuración:

ScriptAlias /cgi-bin/ "/var/www/cgi-bin/"
<Directory "/var/www/cgi-bin">
    Options +ExecCGI
    AddHandler cgi-script .cgi
    Require all granted
</Directory>


Reiniciar Apache:

sudo service apache2 restart

3️⃣ Ejecutar la aplicación

Abrir el navegador y acceder a:

http://localhost/index.html


Desde ahí se pueden agregar tareas y comunicarse con el backend en C++.

⚠️ Aclaraciones importantes

El backend está implementado en C++ usando CGI, una tecnología sencilla y adecuada para fines académicos.

No se utilizan librerías externas (JSON se maneja de forma básica).

El diseño es intencionalmente simple para priorizar la lógica y el funcionamiento.

La aplicación no está pensada para producción, solo para aprendizaje.

⭐ Extras

Persistencia de datos mediante archivo local

Backend web real en C++

Comunicación HTTP básica

Backend web real en C++
👤 Autor

  Cecilia Marez
ejercicios tecnicos – Programación en C++






