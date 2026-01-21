# coffee-shop-db-normalization
Migración y normalización de datos de una cafetería desde múltiples fuentes (CSV/Excel) a PostgreSQL


Sistema de Gestión de Datos: Coffee Shop Project ☕
Este proyecto forma parte de un caso práctico de ingeniería de datos y diseño de bases de datos relacionales. El objetivo principal es centralizar información proveniente de múltiples fuentes (Excel y CSV) en un sistema unificado y normalizado utilizando PostgreSQL y MySQL.

📝 Escenario del Proyecto
La empresa de café tiene datos distribuidos en diferentes departamentos:

Sede (HQ): Información de personal y puntos de venta en hojas de cálculo.

Puntos de Venta (POS): Datos de transacciones en archivos CSV.

CRM: Datos de clientes en archivos CSV.

Proveedores: Listado de productos en Excel.

Mi tarea es diseñar el esquema, normalizar las tablas, definir las relaciones y crear objetos de base de datos para facilitar la generación de reportes operativos.

🚀 Objetivos del Laboratorio

[*] Identificar Entidades y Atributos: Extraer el modelo lógico de los archivos fuente.

[ ] Diseño de ERD: Crear el Diagrama de Entidad-Relación en pgAdmin.

[ ] Normalización: Asegurar la integridad de los datos y eliminar redundancias.

[ ] Implementación SQL: Generar y ejecutar scripts de creación de objetos.

[ ] Optimización: Crear Vistas y Vistas Materializadas para reportes rápidos.

🛠️ Herramientas Utilizadas
Diseño: pgAdmin ERD Tool.

Base de Datos Principal: PostgreSQL.

Gestión y Migración: MySQL & phpMyAdmin.

Control de Versiones: Git & GitHub.

📂 Estructura del Repositorio
/data: Archivos fuente originales (CSV/Excel).

/design: Diagramas de Entidad-Relación (ERD) y documentación del modelo.

/scripts: Código SQL para creación de tablas, relaciones y vistas.

/docs: Capturas de pantalla de resultados y reportes.

🏗️ Modelo de Datos (ERD)
(Próximamente: Aquí se incluirá la imagen del diagrama generado en pgAdmin)

Cómo usar este repositorio
Clona el repositorio: git clone https://github.com/tu-usuario/coffee-shop-db-normalization.git

Los scripts de creación se encuentran en la carpeta /scripts.

Sigue el orden de ejecución indicado en los archivos SQL para mantener la integridad referencial.