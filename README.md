# Desafío Técnico para Ingeniero de Datos Jr 🚀

## Objetivo 👈
El objetivo de este desafío es construir un pipeline de datos que consuma información de la PokeAPI y de archivos CSV, almacenando los datos en una base de datos PostgreSQL y creando las relaciones necesarias entre las tablas.

## Requerimientos Funcionales 🔎

### Primera Etapa:
- Consumir la PokeAPI para obtener los datos de Pokémon: `https://pokeapi.co/api/v2/pokemon/`
- Almacenar en la base de datos las siguientes tablas:
  - **pokemon**
  - **type**
  - **pokemon_type**

### Segunda Etapa:
- Consumir los archivos CSV `legendaries.csv` y `rares.csv`.
- Añadir a la base de datos las tablas correspondientes y sus relaciones:
  - **legendaries**
  - **rares**

### Tercera Etapa:
Crear vistas en la base de datos.
   - **`pokemon_by_type`**: Muestra todos los Pokémon agrupados por su tipo.
   - **`legendary_pokemon`**: Muestra solo los nombres de los Pokémon que son legendarios.
   - **`rare_pokemon`**: Muestra solo los nombres de los Pokémon que son raros.
   - **`pokemon_stats`**: Proporciona el conteo de tipos por Pokémon.
   - **`legendary_and_rare_pokemon`**: Muestra todos los Pokémon y su clasificación de rareza (legendario, raro o normal).
   - **`type_and_legendaries`**: Proporciona el conteo de Pokémon legendarios agrupados por tipo.

## Requerimientos Técnicos 🔧

- **Python 3.8+**: El código debe ser compatible con cualquier versión de Python >= 3.8.
- **Ejecución**: Configurar el programa para que se ejecute automáticamente con CRON todos los días a las 8:00 AM.
- **.env**: Debe existir un archivo `.env` que contenga los datos de conexión a la base de datos PostgreSQL.
- **Logs**: El programa debe generar registros adecuados sobre su ejecución utilizando la librería `logging`.
- **Entorno virtual**: Utilizar `venv` para crear un entorno virtual y guardar las librerías instaladas en un archivo `requirements.txt`

## Bases de Datos 📚
- **Scripts de Creación de Tablas**: Dejar disponibles los scripts necesarios para la creación de las tablas utilizadas en el proyecto.
- **Conexión a la Base de Datos**:
  - Los datos deben almacenarse en una base de datos PostgreSQL.
  - La conexión a la base de datos debe implementarse utilizando la librería y ORM `SQLAlchemy`.
