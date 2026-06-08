# Proyecto SQL – Base de Datos Sakila (PostgreSQL)
# 🧩 Descripción del proyecto
Este proyecto tiene como objetivo practicar y consolidar conocimientos de SQL mediante la resolución de una colección de ejercicios sobre la base de datos relacional Sakila.

La base de datos Sakila simula el funcionamiento de un videoclub e incluye información sobre películas, actores, categorías, clientes, alquileres, pagos, empleados y tiendas.

Durante el desarrollo del proyecto se han realizado consultas SQL de distintos niveles de complejidad utilizando PostgreSQL, aplicando conceptos fundamentales de bases de datos relacionales.

# 🎯 Objetivos
-Comprender la estructura de una base de datos relacional.

-Aprender a consultar información mediante SQL.

-Utilizar correctamente las relaciones entre tablas.

-Aplicar funciones de agregación.

-Realizar consultas con múltiples JOIN.

-Utilizar subconsultas.

-Crear vistas y tablas temporales.

-Interpretar y resolver problemas de negocio mediante consultas SQL.

# 🧹 Tecnologías utilizadas
PostgreSQL, 
pgAdmin, 
SQL

# 📊 Estructura de la base de datos 
Las principales tablas utilizadas durante el proyecto son:

Film -> Contiene la información de las películas:

*film_id

*title

*description

*release_year

*language_id

*rental_duration

*rental_rate

*length

*replacement_cost

*rating

Actor -> Información de los actores:

*actor_id

*first_name

*last_name

Category -> Categorías de las películas:

*category_id

*name

Customer -> Información de los clientes:

*customer_id

*first_name

*last_name

*email

Rental -> Información de los alquileres:

*rental_id

*rental_date

*inventory_id

*customer_id

*return_date

Payment -> Información de los pagos:

*payment_id

*customer_id

*rental_id

*amount

*payment_date

# 📈 Relaciones entre tablas 
Actores y películas : actor → film_actor → film

Películas y categorías: film → film_category → category

Películas alquiladas: film → inventory → rental

Clientes y alquileres: customer → rental

Ingresos generados: payment

# 📌 Conceptos SQL utilizados
SELECT -> 
Obtención de información específica de una tabla.

WHERE -> 
Filtrado de registros según una condición.

ORDER BY -> 
Ordenación de resultados.

DISTINCT -> 
Eliminación de registros duplicados.

GROUP BY -> 
Agrupación de datos para realizar cálculos por grupos.

HAVING -> 
Filtrado de resultados agregados.

JOIN -> Relación entre tablas. Tipos utilizados:
INNER JOIN

LEFT JOIN

CROSS JOIN

Funciones de agregación -> 
COUNT()
SUM()
AVG()
MAX()
MIN()

Subconsultas ->
Consultas anidadas para obtener información dependiente de otros resultados.

Vistas ->
Creación de vistas para reutilizar consultas complejas.

Tablas temporales ->
Creación de tablas temporales para almacenar resultados intermedios.


# Ejercicios realizados

Entre las consultas desarrolladas se encuentran:
-Búsqueda de actores por apellido.

-Recuento de películas por clasificación.

-Cálculo de ingresos totales.

-Obtención de clientes y sus alquileres.

-Identificación de actores por categoría de película.

-Cálculo de duración media de películas.

-Creación de vistas.

-Creación de tablas temporales.

-Consultas mediante subconsultas correlacionadas.

-Análisis de alquileres por cliente y categoría.

# Aprendizajes obtenidos
Durante el proyecto se han reforzado conocimientos relacionados con:

*Modelado relacional.

*Claves primarias y foráneas.

*Relaciones uno a muchos y muchos a muchos.

*Optimización de consultas SQL.

*Interpretación de requisitos de negocio.

*Manejo de PostgreSQL.

# Conclusión

Este proyecto ha permitido desarrollar una comprensión sólida de SQL y de las bases de datos relacionales mediante la resolución práctica de problemas reales utilizando la base de datos Sakila. Se han aplicado consultas simples y avanzadas, así como técnicas de agregación, agrupación, relaciones entre tablas y creación de objetos de base de datos como vistas y tablas temporales.

# 📌 Estructura del repositorio

├── Archivo SQL.sql/          # Archivos de visualización de consultas

├── BBDD_Proyecto_shakila /                # Base de datos Sakila

├──Informe proyecto SQL/             # Informe explicativo

└── README.md           # Documentación del proyecto

# 🚀 Cómo usar este proyecto
Revisar el informe Informe proyecto SQL /report

Explorar el archivo .sql
