#  Supply Chain Resilience & Customer Lifetime Value (CLV) Optimization

1. El Dataset: Olist E-Commerce (Kaggle) es un conjunto de datos real de e-commerce en Brasil con mas de 100k pedidos. 

2. El objetivo es atacar tres frentes:
* Optimización Logística: Análisis de la brecha entre el tiempo estimado de entrega y el real, utilizando distribuciones de probabilidad para identificar cuellos de botella geográficos.
* Modelado de Retención (Cohortes): No solo ver quién compró, sino cuándo regresan, calculando el Churn Rate y el Customer Lifetime Value.
* Análisis de Sensibilidad: Un simulador de escenarios dentro de Power BI.

3. Arquitectura del ProyectoFaseTecnologíaAcción de Nivel ExpertoETL & CleaningPython (Pandas/Polars) o SQLImplementar una arquitectura Medallion (Bronze, Silver, Gold). Manejar valores nulos mediante imputación estadística, no solo borrando filas.Análisis EstadísticoSciPy / StatsmodelsRealizar un análisis de correlación de Pearson y pruebas de hipótesis para validar si el precio del flete realmente afecta la satisfacción del cliente ($p-value < 0.05$).VisualizaciónPower BIUso exhaustivo de DAX avanzado, Row-Level Security (simulado) y Calculation Groups.

4. Estructura del Dashboard en Power BI
* A. Strategic Executive SummaryKPIs Dinámicos: Utiliza Field Parameters para que el usuario elija si quiere ver el KPI por "Ingresos", "Volumen de Pedidos" o "Margen de Beneficio".Gráfico de Descomposición (Decomposition Tree): Para analizar qué categorías de productos están arrastrando el margen hacia abajo.
* B. Supply Chain & Logistics (Deep Dive)Análisis de Errores de Estimación: Un histograma que muestre la diferencia en días entre la fecha prometida y la real.Mapa de Calor Geo-espacial: Integración con Azure Maps o Mapbox para visualizar densidades de entrega y tiempos de tránsito por estado brasileño.
* C. Customer Intelligence (Matemática Aplicada)Matriz de Análisis de Cohortes: Una tabla de calor que muestre la retención mensual.Segmentación RFM (Recency, Frequency, Monetary): Clasifica a los clientes automáticamente en "Campeones", "En Riesgo" o "Perdidos" usando DAX.D. "What-If" Analysis (El diferenciador)Crea parámetros numéricos donde el usuario pueda deslizar una barra para decir: "Si reducimos el costo del flete en un 10%, ¿cuántas órdenes más necesitamos para mantener el mismo margen?". Esto demuestra que entiendes el negocio.

5. Técnicas de Power BI que debes incluir para impresionar:DAX Avanzado: Uso de CALCULATE, KEEPFILTERS, y funciones de iteración como SUMX o AVERAGEX sobre tablas virtuales.Tooltips Personalizados: Gráficos de tendencias pequeños que aparecen al pasar el cursor sobre un punto de datos.Navegación Intuitiva: Menús laterales colapsables mediante marcadores (bookmarks) y botones.Diseño UI/UX: Usa una paleta de colores profesional (ej. Dark Mode o Corporate Blue) y asegúrate de que haya suficiente espacio negativo.