Este proyecto se centra en la toma de decisiones basada en datos para una tienda online de gran tamaño. El objetivo principal es aumentar los ingresos mediante la priorización estratégica de hipótesis de negocio y el análisis riguroso de los resultados de un test A/B.

📋 Estructura del Proyecto
El análisis se divide en tres etapas fundamentales:

Preprocesamiento de Datos: Limpieza, estandarización de columnas y ajuste de tipos de datos.

Priorización de Hipótesis: Aplicación de los frameworks ICE y RICE.

Análisis de Test A/B: Evaluación de métricas acumuladas, tasas de conversión y detección de anomalías.

🛠️ Tecnologías Utilizadas
Python 3.x

Pandas: Manipulación y limpieza de datos.

Matplotlib & Seaborn: Visualización de datos estática.

Plotly: Gráficos interactivos.

Scipy: Pruebas estadísticas.

🔍 Análisis Realizado
1. Priorización de Hipótesis
Se evaluaron 9 hipótesis utilizando dos métodos para determinar el enfoque óptimo:

ICE (Impact, Confidence, Ease): Para medir el valor rápido.

RICE (Reach, Impact, Confidence, Effort): Para incluir el alcance de usuarios en la ecuación.

Resultado: Se observó que al usar RICE, el orden de las hipótesis cambia significativamente, destacando aquellas que afectan a una base de usuarios mayor.

2. Análisis del Test A/B
Se analizaron los grupos A y B durante el mes de agosto de 2019:

Ingresos Acumulados: El Grupo B mostró un crecimiento superior, especialmente tras un pico detectado alrededor del 17 de agosto.

Tamaño Promedio de Pedido: Identificación de fluctuaciones drásticas debidas a pedidos inusualmente grandes (outliers).

Tasa de Conversión: Comparativa diaria de la capacidad de cada grupo para convertir visitas en ventas.

3. Tratamiento de Anomalías
Se utilizaron percentiles (95 y 99) para identificar valores atípicos:

Se determinó que usuarios con más de 2 pedidos o pedidos con un valor superior a un umbral específico (basado en el percentil 95) se consideran anomalías que pueden sesgar los resultados.

📈 Conclusiones Clave
Hipótesis Ganadora: Se realizaron pruebas de significancia para validar si las diferencias observadas entre el Grupo A y el Grupo B eran estadísticamente representativas o producto del azar.de

Conversión: Existe una diferencia estadísticamente significativa (p-value: 0.007). El Grupo B es superior y la mejora es real, no un artefacto de los datos.

Tamaño de Pedido: No hay una diferencia estadísticamente significativa en el tamaño promedio de los pedidos entre los grupos.

Decisión Final: Aunque el Grupo B muestra un liderazgo claro en conversión, se recomienda continuar la prueba un tiempo adicional para observar si la estabilidad del Grupo A o la volatilidad del Grupo B se mantienen, asegurando una decisión de negocio robusta a largo plazo.
