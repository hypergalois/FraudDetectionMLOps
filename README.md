# Demostración de Detección de Fraude con MLOps

Esta demostración presenta una solución para la prevención de fraudes financieros utilizando el feature store de MLRun para definir características complejas que ayudan a identificar actividades fraudulentas. La prevención de fraudes es un desafío particular, ya que requiere procesar transacciones y eventos en tiempo real, respondiendo rápidamente para bloquear transacciones antes de que se completen.

## Enfoque de la solución

Para abordar este problema, se implementan dos pipelines:

-   Pipeline de desarrollo: Permite probar y ajustar la lógica de ingeniería de características y modelos.

-   Pipeline de producción: Utiliza las mismas características y modelos, pero se adapta para manejar datos en tiempo real.

Además, se automatiza el monitoreo de datos y modelos, permitiendo detectar desviaciones (drift) y activar el reentrenamiento de modelos dentro de un pipeline CI/CD. El proceso completo se describe en el siguiente diagrama:

![Feature store demo diagram - fraud prevention](./diagram.png)

## Pasos de implementación del proyecto

### Exploración y análisis de datos (EDA):

Comprender las características de los datos y su estructura.

### Construcción del pipeline de ingesta y preparación de datos:

Preprocesar y transformar datos para su uso en modelos.

### Desarrollo del pipeline de entrenamiento y validación de modelos:

Entrenar modelos con diferentes características y algoritmos.

### Desarrollo del pipeline de servicio de la aplicación:

Interceptar solicitudes, procesar datos en tiempo real y realizar inferencias.

### Monitoreo de datos y modelos:

Detectar desviaciones (drift) y evaluar el rendimiento de los modelos en producción.

### Gestión de operaciones continuas y CI/CD:

Automatizar la integración y el despliegue continuo para mantener los modelos actualizados.
Preparación de los datos
