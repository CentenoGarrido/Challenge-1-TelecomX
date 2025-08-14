# Challenge-1-Telecomx
Challenge de Alura ONE Ciencia de datos.

# Análisis de Evasión de Clientes en TelecomX

Este proyecto documenta el proceso de análisis de datos para identificar los factores que contribuyen a la evasión de clientes de la empresa de telecomunicaciones ficticia *TelecomX*. El análisis incluye la carga, limpieza, transformación y visualización de datos para extraer insights.

## Fases de trabajo:

*  **Extracción de Datos:** Descarga y carga de los datos de clientes desde un archivo JSON remoto.
*  **Transformación de Datos:**
    *   Normalización de la estructura JSON anidada en un DataFrame plano.
    *   Manejo de valores faltantes, duplicados y en blanco.
    *   Conversión de tipos de datos.
    *   Codificación numérica de variables categóricas y binarias.
    *   Preparación de datos con etiquetas traducidas para visualización.
*  **Análisis y Visualización:**
    *   Definición de funciones de graficación reutilizables para distribuciones y conteos por categoría.
    *   Generación de gráficos para explorar la relación entre diversas características del cliente (demografía, servicios, contrato, cargos, antigüedad) y la tasa de evasión.
    *   Análisis de la matriz de correlación entre variables numéricas y binarias.
*  **Informe Final:** Resumen de las principales conclusiones del análisis y recomendaciones estratégicas basadas en los hallazgos.

## Hallazgos del análisis:
El análisis reveló varios factores significativos asociados con la evasión de clientes:

*   **Tipo de Contrato:** Los clientes con contratos **mes a mes** tienen una probabilidad de evasión considerablemente mayor en comparación con aquellos con contratos a largo plazo (uno o dos años).
*   **Antigüedad del Cliente (Tenure):** La tasa de evasión es inversamente proporcional a la antigüedad; los clientes con **menos meses** en la compañía son los más propensos a cancelar.
*   **Servicios de Internet:** Los clientes con servicio de **Fibra Óptica** presentan una tasa de evasión más alta que los que tienen DSL o no tienen servicio de internet.
*   **Método de Pago:** El uso de **Cheque Electrónico** como método de pago está fuertemente asociado con una mayor tasa de evasión.
*   **Servicios Adicionales:** Los clientes que **no** tienen servicios como Seguridad en Línea, Respaldo en Línea, Protección de Dispositivos y Soporte Técnico tienden a evadir más. Estos servicios parecen ser importantes para la retención.
*   **Cargos:** Existe una correlación positiva entre los **cargos mensuales y totales** y la evasión, sugiriendo que los clientes con facturas más altas podrían ser más propensos a irse.

## Recomendaciones:
Basado en estos hallazgos, se sugieren las siguientes acciones para reducir la evasión:

*   Ofrecer incentivos para que los clientes de contrato mes a mes migren a planes de mayor duración.
*   Implementar un programa de incorporación y seguimiento intensivo para clientes nuevos durante sus primeros meses.
*   Investigar las razones detrás de la alta tasa de evasión de clientes de Fibra Óptica y tomar medidas correctivas (ej. mejorar calidad, ajustar precios).
*   Promover activamente métodos de pago automáticos y desalentar el uso de cheque electrónico.
*   Destacar el valor y fomentar la adopción de servicios adicionales, especialmente entre los clientes de fibra óptica.
