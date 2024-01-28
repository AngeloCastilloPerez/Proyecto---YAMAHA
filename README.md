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

## Contribuir
Para contribuir al proyecto, por favor haz un fork del repositorio, crea una rama con tu feature o corrección y realiza un pull request.



## Licencia
Este proyecto está bajo la Licencia MIT - ver el archivo LICENSE.md para más detalles.
