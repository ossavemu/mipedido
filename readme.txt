INSTALACIÓN DE MIPEDIDO - APLICACIÓN WEB
=======================================

Este archivo te guiará paso a paso para instalar y ejecutar la aplicación.

REQUISITOS:
----------
- Tener instalado Python 3.8 o superior en Windows
- Si no tienes Python, descárgalo de: https://www.python.org/downloads/
  (¡IMPORTANTE! Al instalar Python marca la casilla "Add Python to PATH")

PASOS PARA INSTALAR:
------------------
1. Descomprime la carpeta del proyecto donde quieras en tu computadora

2. Abre el Símbolo del Sistema (CMD) de Windows:
   - Presiona la tecla Windows + R
   - Escribe "cmd" y presiona Enter

3. En el CMD, navega hasta la carpeta del proyecto:
   - Escribe: cd C:\ruta\donde\descomprimiste\el\proyecto
   - Ejemplo: cd C:\Users\TuUsuario\Desktop\mipedido

4. Crea un entorno virtual (esto mantiene ordenado tu sistema):
   - Escribe: python -m venv venv
   - Luego escribe: venv\Scripts\activate
   - Verás que aparece (venv) al inicio de la línea

5. Instala los programas necesarios:
   - Escribe: pip install -r requirements.txt
   - Espera a que termine la instalación

PARA EJECUTAR LA APLICACIÓN:
--------------------------
1. Asegúrate de estar en la carpeta del proyecto y con el entorno virtual activado
   (deberías ver (venv) al inicio de la línea en el CMD)

2. Escribe: uvicorn main:app --reload

3. Abre tu navegador web y escribe: http://localhost:8000

ESTRUCTURA DE CARPETAS:
---------------------
mipedido/
  ├── main.py              (archivo principal)
  ├── requirements.txt     (lista de programas necesarios)
  ├── static/             (archivos de diseño)
  │   └── css/
  │       └── styles.css
  └── templates/          (páginas web)
      └── index.html

SI ALGO NO FUNCIONA:
------------------
1. Asegúrate de que Python está instalado:
   - Abre CMD y escribe: python --version
   - Deberías ver algo como "Python 3.8.0" o superior

2. Si la página aparece sin diseño:
   - Revisa que todas las carpetas estén en su lugar
   - Especialmente la carpeta "static" y "templates"

3. Si el servidor no inicia:
   - Asegúrate de estar en la carpeta correcta
   - Verifica que el entorno virtual esté activado (venv)
   - Intenta instalar los requisitos nuevamente

PARA CERRAR TODO:
---------------
1. Para detener el servidor: presiona Ctrl + C en el CMD
2. Para desactivar el entorno virtual escribe: deactivate
3. Puedes cerrar el CMD

¡LISTO! Si tienes problemas, pide ayuda a alguien con experiencia. 