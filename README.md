# Sistema de Gestión de Base de Datos MySQL

## Descripción General

Este proyecto es una aplicación de consola escrita en Python que permite a los usuarios interactuar con una base de datos MySQL. Los usuarios pueden conectarse a una base de datos, listar bases de datos y tablas, insertar, consultar, modificar y eliminar registros en las tablas.

## Requisitos

- Python 3.x
- Biblioteca `mysql.connector` para Python
- Acceso a una instancia de MySQL

## Instalación

1. Asegúrate de tener Python 3.x instalado en tu sistema.
2. Instala la biblioteca `mysql.connector` usando pip:
```bash
pip install mysql-connector-python
```

## Uso

### Conexión a la Base de Datos

El programa solicitará al usuario ingresar su nombre de usuario y contraseña para establecer una conexión con la base de datos MySQL.

### Interacción con la Base de Datos

Una vez conectado, el usuario podrá realizar las siguientes operaciones:

- **Listar Bases de Datos**: El programa muestra todas las bases de datos disponibles en el servidor MySQL.
- **Seleccionar Base de Datos**: El usuario puede seleccionar una base de datos de la lista para trabajar con ella.
- **Listar Tablas**: Una vez seleccionada la base de datos, el programa muestra todas las tablas disponibles en esa base de datos.
- **Insertar Registro**: Permite al usuario ingresar un nuevo registro en una tabla especificada.
- **Consultar Registros**: Muestra todos los registros de una tabla seleccionada.
- **Modificar Registro**: Permite al usuario modificar un registro existente en una tabla.
- **Eliminar Registro**: Permite al usuario eliminar un registro existente en una tabla.
- **Salir**: Cierra la conexión a la base de datos y termina el programa.

## Ejemplo de Uso

1. Ejecuta el script.
2. Ingresa tus credenciales de acceso a MySQL cuando se te solicite.
3. Sigue las indicaciones en pantalla para seleccionar una base de datos y luego una tabla.
4. Utiliza las opciones del menú para realizar las operaciones deseadas sobre los registros de la tabla.

## Funciones Principales

### `obtener_bases_de_datos()`
- Descripción: Obtiene y devuelve una lista de todas las bases de datos disponibles en el servidor MySQL.
- Parámetros: Ninguno.
- Retorno: Lista de nombres de bases de datos.

### `seleccionar_base_de_datos()`
- Descripción: Solicita al usuario seleccionar una base de datos de la lista disponible.
- Parámetros: Ninguno.
- Retorno: Nombre de la base de datos seleccionada.

### `obtener_tablas()`
- Descripción: Obtiene y devuelve una lista de todas las tablas disponibles en la base de datos actualmente seleccionada.
- Parámetros: Ninguno.
- Retorno: Lista de nombres de tablas.

### `seleccionar_tabla()`
- Descripción: Solicita al usuario seleccionar una tabla de la lista disponible.
- Parámetros: Ninguno.
- Retorno: Nombre de la tabla seleccionada.

### `insertar_registro(tabla)`
- Descripción: Inserta un nuevo registro en la tabla especificada.
- Parámetros: Nombre de la tabla.
- Retorno: Mensaje de éxito o error.

### `leer_registros(tabla)`
- Descripción: Lee y muestra todos los registros de la tabla especificada.
- Parámetros: Nombre de la tabla.
- Retorno: N/A

### `modificar_registro(tabla)`
- Descripción: Modifica un registro existente en la tabla especificada.
- Parámetros: Nombre de la tabla.
- Retorno: Mensaje de éxito o error.

### `baja_registro(tabla)`
- Descripción: Elimina un registro existente en la tabla especificada.
- Parámetros: Nombre de la tabla.
- Retorno: Mensaje de éxito o error.

### `cerrar_conexion()`
- Descripción: Cierra la conexión a la base de datos y termina el programa.
- Parámetros: Ninguno.
- Retorno: N/A

