# Proyecto Yamaha Medallion en Azure

![DALL·E 2024-01-28 17 08 45 - Create a futuristic technology banner with a central focus on the word 'AZURE' prominently displayed in the center  The backdrop should feature a dyna](https://github.com/AngeloCastilloPerez/Proyecto---YAMAHA/assets/107339963/4f2151e3-16fe-4154-8177-4c737b9f65dc)

## Descripción
Este proyecto implementa una solución end-to-end para Yamaha Motors utilizando Azure Data Factory (ADF) y Microsoft Storage Account en Azure. Se ha adoptado la metodología Medallion para estructurar el Data Lake y optimizar el flujo de datos desde la extracción hasta el análisis.

![Diagrama de Arquitectura](https://github.com/AngeloCastilloPerez/Proyecto---YAMAHA/assets/107339963/9769b559-b077-4f5c-aa8c-f2ead7f3b8b3)

## Arquitectura
La arquitectura Medallion implementada permite la capa de almacenamiento y procesamiento de datos en tres zonas:
- **Bronze (Raw Data)**: Datos crudos sin procesar almacenados en formato original.
- **Silver (Cleansed Data)**: Datos que han pasado por procesos de limpieza y transformación.
- **Gold (Consumption Data)**: Datos enriquecidos y listos para ser consumidos por aplicaciones de negocio.

![Flujo Pipelines](https://github.com/AngeloCastilloPerez/Proyecto---YAMAHA/assets/107339963/b372b35d-a3d2-472f-af65-79aaf56129e6)

## Componentes Principales
- **Azure Data Factory**: Utilizado para la orquestación de datos, la integración y la transformación.
- **Azure Blob Storage**: Almacenamiento de datos en bruto en la capa Bronze.
- **Azure Data Lake Storage**: Almacenamiento de datos procesados en las capas Silver y Gold.

![Triggers](https://github.com/AngeloCastilloPerez/Proyecto---YAMAHA/assets/107339963/d3caef34-cfd5-4b85-ab5c-da1e6df5f2f2)

## Retos Principales
- **Integración de Datos**: Conectar y consolidar datos de diversas fuentes.
- **Transformación de Datos**: Limpiar y transformar datos en formatos no estructurados a un formato analizable.
- **Automatización**: Configurar pipelines de ADF para automatizar flujos de trabajo y triggers.

## Proceso de Desarrollo
1. **Extracción de Datos**: Configuración de Linked Services y Datasets en ADF para extraer datos de fuentes como SharePoint.
2. **Transformación de Datos**: Uso de Data Flows para aplicar transformaciones y limpieza de datos.
3. **Carga de Datos**: Mover datos transformados a las capas correspondientes del Data Lake.
4. **Monitoreo y Orquestación**: Implementación de monitoreo para asegurar el correcto flujo de datos y la resolución de problemas.

## Cómo Usar
1. **Configuración del Ambiente**: Asegúrate de tener las suscripciones de Azure y permisos necesarios.
2. **Clonación del Repositorio**: `git clone https://github.com/AngeloCastilloPerez/Proyecto---YAMAHA.git`

## Componentes de la Solución
Los componentes clave de Azure empleados en este proyecto incluyeron Azure Data Lake, Azure Data Factory y Azure SQL Database, cada uno cumpliendo roles específicos dentro de la metodología Medallion, que estructura los datos en capas de procesamiento, desde la ingestión hasta el análisis.

### Azure Data Lake
Fue utilizado como repositorio central para las cargas de trabajo de análisis de macrodatos, almacenando datos de cualquier tamaño y tipo en un solo lugar, facilitando así análisis operativos y exploratorios. La flexibilidad en el escalado permitió a Yamaha manejar las cargas de trabajo de manera eficiente y garantizar la alta disponibilidad de los datos.

### Azure Data Factory
Sirvió como la solución de integración de datos, proporcionando una plataforma completa para la implementación de proyectos híbridos de ETL y ELT. ADF se utilizó para mover datos desde las fuentes hacia el data warehouse y para construir lógicas de transformación de datos necesarias para promover los datos almacenados a los contenedores de datos WORK y MODEL.

### Azure SQL Database
Ofreció una opción PaaS para consumir una base de datos como un servicio de datos en la nube, manejado por Azure. Esta base de datos almacena las tablas que representan el modelo de datos optimizado para el análisis, proporcionando a Yamaha un almacenamiento de datos altamente disponible y escalable.

## Beneficios y Retorno de Inversión
El proyecto proporcionó múltiples beneficios tangibles e intangibles, incluyendo:

1. **Automatización de Procesos**: Eliminación de los procesos manuales y mejora de la eficiencia operativa.
2. **Integridad y Calidad de Datos**: Mejora en la calidad de los datos utilizados para la toma de decisiones a través de validaciones y transformaciones.
3. **Análisis Avanzado**: Capacidades mejoradas de análisis de datos para obtener insights profundos y mejorar estrategias y operaciones comerciales.
4. **Reducción de Costos**: Mantenimiento de costos operativos bajos mediante la activación de servicios según la demanda.
5. **Escalabilidad y Disponibilidad**: Capacidad para escalar recursos y garantizar la disponibilidad sin grandes inversiones en infraestructura.
6. **Seguridad de Datos**: Beneficios de la seguridad de nivel empresarial, protegiendo los datos contra amenazas y asegurando el cumplimiento de normativas.



## Contribuir
Para contribuir al proyecto, por favor haz un fork del repositorio, crea una rama con tu feature o corrección y realiza un pull request.



## Licencia
Este proyecto está bajo la Licencia de NASA - ver el archivo LICENSE-NASA.md para más detalles.
