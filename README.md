# RetailPro — Análisis de ventas

## Descripción del proyecto

RetailPro es un proyecto de análisis de datos orientado a estudiar las ventas de un negocio de retail. El objetivo es organizar la información comercial, realizar consultas SQL para obtener indicadores de negocio y utilizar Power BI para facilitar la interpretación de los resultados.

El proyecto forma parte de un proceso de aprendizaje de análisis de datos y combina la gestión de bases de datos con la elaboración de consultas y herramientas de visualización.

## Herramientas utilizadas

- **SQL Server Management Studio (SSMS):** creación y consulta de la base de datos.
- **SQL Server:** almacenamiento y organización de los datos mediante tablas relacionadas.
- **GitHub:** almacenamiento y documentación de los archivos del proyecto.
- **Power BI:** transformación de datos y elaboración de informes y visualizaciones.

## Estructura del repositorio

| Archivo | Descripción |
|---|---|
| `ventas_tech_db.sql` | Crea la base de datos `Ventas_Tech_DB`, define las tablas, carga datos de ejemplo y permite validar los registros. |
| `m4_consultas_negocio.sql` | Contiene consultas de facturación mensual, ranking de productos, clientes recurrentes y comparación con el promedio mensual. |
| `m5_consultas_joins.sql` | Incluye consultas con `INNER JOIN`, `LEFT JOIN` y `UNION ALL` para combinar información e identificar clientes y productos sin ventas. |
| `Pipeline_ETL_Apellido_Nombre.pbix` | Archivo de Power BI relacionado con el proceso ETL del proyecto. |
| `Werbin_Juliana_Checkpoint2.pbix` | Archivo de Power BI correspondiente a un checkpoint del proyecto. |

## Modelo de datos

La base de datos `Ventas_Tech_DB` contiene cuatro tablas principales:

- **categorias:** identifica las categorías de productos.
- **clientes:** almacena información de los clientes, como nombre, email, ciudad y fecha de registro.
- **productos:** contiene los productos, su categoría, precio, stock y estado.
- **ventas:** registra las operaciones comerciales, incluyendo cliente, producto, cantidad, precio unitario y fecha.

Las tablas se relacionan mediante claves primarias y foráneas para integrar la información y realizar consultas de análisis.

## Cómo ejecutar los scripts SQL

### Requisitos previos

- Tener instalado SQL Server.
- Contar con SQL Server Management Studio (SSMS).
- Disponer de permisos para crear y consultar bases de datos.

### Pasos de ejecución

1. Descargar o clonar el repositorio de GitHub.
2. Abrir SSMS y conectarse a una instancia de SQL Server.
3. Abrir `ventas_tech_db.sql` y ejecutar el script para crear la base de datos, las tablas y cargar los datos de ejemplo. Si la base ya existe, revisar el script antes de volver a ejecutarlo.
4. Abrir `m4_consultas_negocio.sql`, verificar que la base `Ventas_Tech_DB` esté seleccionada y ejecutar las consultas.
5. Abrir `m5_consultas_joins.sql` y ejecutar las consultas de combinación de tablas.
6. Para trabajar con los archivos `.pbix`, abrirlos con Power BI Desktop y comprobar que las conexiones a los datos estén configuradas correctamente.

**Importante:** antes de ejecutar el script de creación en SSMS, verificá que la sentencia `CREATE DATABASE Ventas_Tech_DB` esté separada del resto del código por una instrucción `GO`, ya que SQL Server requiere que la creación de la base se ejecute en su propio lote.

## Objetivo del análisis

El proyecto busca transformar los registros de ventas en información útil para el análisis comercial, permitiendo estudiar la facturación, el comportamiento de los clientes, el desempeño de los productos y otros indicadores que contribuyan a comprender los resultados del negocio.

## Repositorio

[Consultar los archivos del proyecto en GitHub](https://github.com/julianawerbin-byte/Proyecto-RetailPro)
