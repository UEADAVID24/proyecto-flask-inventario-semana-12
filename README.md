Sistema Avanzado de Gestión de Inventario – Flask
Descripción del Proyecto

Este proyecto corresponde a un Sistema Avanzado de Gestión de Inventario desarrollado con Flask, como continuación del proyecto iniciado en las semanas 9, 10 y 11.

El sistema permite administrar productos de una tienda (ferretería) aplicando Programación Orientada a Objetos (POO), uso de colecciones, operaciones CRUD conectadas a una base de datos SQLite y diferentes mecanismos de persistencia de datos.

Además, el sistema incorpora almacenamiento de datos en archivos TXT, JSON y CSV, permitiendo visualizar la información almacenada en cada formato desde la aplicación web.

Objetivos

Aplicar Programación Orientada a Objetos (POO) para estructurar el sistema.

Utilizar colecciones de Python para la gestión de datos.

Implementar operaciones CRUD reales (Crear, Leer, Actualizar, Eliminar).

Almacenar la información en una base de datos SQLite.

Implementar persistencia de datos en archivos TXT, JSON y CSV.

Integrar formularios web para la gestión del inventario.

Utilizar SQLAlchemy ORM para la conexión con SQLite.

Tecnologías Utilizadas

Python 3

Flask

Flask-SQLAlchemy

SQLite

HTML + Jinja2

CSS

Visual Studio Code

Git y GitHub

Estructura del Proyecto
Mi_proyecto_flask_Clinton_Alvarado/
│
├── app.py
├── db.py
├── init_db.py
├── requirements.txt
│
├── models/
│   ├── producto.py
│   └── inventario.py
│
├── database/
│   └── database.db
│
├── data/
│   ├── datos.txt
│   ├── datos.json
│   └── datos.csv
│
├── templates/
│   ├── base.html
│   ├── index.html
│   ├── productos.html
│   ├── agregar_producto.html
│   ├── editar_producto.html
│   ├── clientes.html
│   └── datos.html
│
├── static/
│   └── styles.css
│
└── README.md
Programación Orientada a Objetos (POO)

El sistema se basa en dos clases principales:

Clase Producto

Representa un producto del inventario con los atributos:

id

nombre

cantidad

precio

Clase Inventario

Gestiona los productos del sistema y contiene los métodos para realizar las operaciones CRUD conectadas a SQLite.

Persistencia de Datos

El sistema permite almacenar información en diferentes formatos:

TXT

Se utiliza la función open() para guardar y leer registros en archivos de texto.

JSON

Se utiliza la librería json para convertir los datos a diccionario y almacenarlos en formato JSON.

CSV

Se utiliza la librería csv para guardar y leer registros en formato tabular.

Los datos almacenados pueden visualizarse desde las rutas:

/ver_txt
/ver_json
/ver_csv
Base de Datos SQLite

El sistema utiliza SQLite para el almacenamiento persistente de los productos.

La base de datos contiene la tabla:

productos

La conexión a la base de datos se gestiona desde el archivo:

db.py
Operaciones CRUD Implementadas

El sistema permite realizar las siguientes operaciones:

Crear
Agregar nuevos productos mediante formularios web.

Leer
Mostrar la lista de productos almacenados en la base de datos.

Actualizar
Modificar la cantidad o el precio de un producto existente.

Eliminar
Eliminar productos del inventario.

Interfaz de Usuario

La aplicación web permite:

Visualizar el inventario

Buscar productos

Agregar productos

Editar productos

Eliminar productos

Visualizar datos almacenados en TXT, JSON y CSV

Ejecución del Proyecto

1️⃣ Activar el entorno virtual

.\venv\Scripts\activate

2️⃣ Crear la base de datos

py init_db.py

3️⃣ Ejecutar la aplicación

py app.py

4️⃣ Abrir en el navegador
http://127.0.0.1:5000

Autor

Clinton David Alvarado Chongo

Proyecto académico – Desarrollo de aplicaciones web con Flask
