Coffee Shop Data Engineering: Normalization & Multi-DB Migration
Centralización, normalización y ETL de datos transaccionales para una arquitectura de bases de datos híbrida.

📝 Visión General del Proyecto
Este proyecto aborda la problemática real de la fragmentación de datos en una cadena de cafeterías en expansión. La información operativa residía en silos de datos heterogéneos (HQ, CRM, POS y Proveedores) en formatos como Excel y CSV.

El objetivo fue diseñar e implementar un ecosistema de datos centralizado en PostgreSQL, optimizado para el rendimiento mediante vistas materializadas y preparado para una migración fluida hacia entornos MySQL y IBM DB2.

🚀 Objetivos Estratégicos
Ingeniería Inversa y Modelado: Extracción de lógica de negocio desde archivos planos para la creación de un Modelo Lógico/Físico.

Normalización Avanzada: Refactorización de esquemas para eliminar redundancias y garantizar la integridad referencial.

Pipeline de Datos (ETL): Implementación de procesos de extracción y transformación para la unificación de datos.

Arquitectura de Portabilidad: Generación de activos agnósticos al motor de base de datos para garantizar la interoperabilidad multicloud.

🛠️ Stack Tecnológico
Base de Datos Principal: PostgreSQL 15+

Entornos de Destino: MySQL (phpMyAdmin) & IBM DB2.

Herramientas de Diseño: pgAdmin 4 ERD Tool.

Infraestructura: Entornos basados en Linux (Shell/Bash).

Control de Versiones: Git con flujo de trabajo basado en Rebase para un historial limpio.

🏗️ Ciclo de Vida del Desarrollo
1. Diseño y Normalización (ERD)
Se identificaron y corrigieron errores críticos de integridad referencial en el diseño original. Se implementó un esquema de 7 tablas relacionadas que cubren desde el personal (staff) hasta el detalle granular de las ventas (sales_detail).

2. Implementación y Troubleshooting
Durante el despliegue, se superaron restricciones de interfaz gráfica mediante scripts avanzados de consola SQL.

Dominio de SQL COPY: Uso del comando COPY para la exportación directa desde el servidor, evadiendo bloqueos de portapapeles y permisos de navegador.

Administración de Sistemas: Gestión de directorios de sistema (/tmp y caché de credenciales) para la manipulación de archivos CSV de gran tamaño.

3. Optimización de Consultas
Creación de Vistas Materializadas para acelerar el acceso a datos críticos de marketing y reportes de nómina, permitiendo una reducción significativa en el tiempo de ejecución de consultas complejas.

📂 Estructura del Ecosistema
/scripts: Diccionario de datos SQL (DDL/DML) y reportes CSV generados.

/docs: Evidencias de ejecución (Tasks 5A - 10) y documentación de validación.

GeneratedScript_personal.sql: Lógica de negocio optimizada y corregida.

💡 Nota de Ingeniería y Portabilidad
Estado del Proyecto: El pipeline se completó exitosamente hasta la fase de Exportación y Validación de Datos.

Ante restricciones de infraestructura externa para la carga final en DB2, se entregaron archivos CSV estandarizados y saneados. Estos activos han sido validados para garantizar una carga de datos zero-error en cualquier motor relacional compatible, cumpliendo con los estándares de interoperabilidad requeridos por la empresa.

Cómo explorar este proyecto
Revisar el Modelo: Dirígete a /docs para visualizar el esquema lógico corregido.

Ejecutar el Esquema: Utiliza GeneratedScript_personal.sql en una instancia de PostgreSQL.

Consultar Datos: El archivo CoffeeData.sql contiene los registros reales listos para análisis.