# 📦 Análisis de Negocio — Shipping & Sales Data 2013–2017 (Power BI + Python)

## 📌 Problema de negocio

Una empresa distribuidora con actividad en tres categorías de producto necesita entender qué impulsa sus ventas, qué clientes generan más valor, por qué las ventas cayeron un 28,6% en 2016 y cómo optimizar su estrategia comercial para recuperar el crecimiento.

## 🎯 Objetivo

Realizar un análisis de negocio completo sobre 4 años de transacciones comerciales reales, combinando exploración de datos, técnicas estadísticas y visualización en Power BI, para extraer conclusiones accionables que apoyen la toma de decisiones estratégicas.

## 📊 Dataset

- **Fuente:** Shipping Data — Kaggle
- **Período:** Febrero 2013 – Febrero 2017
- **Volumen:** 1.039 registros, 19 variables
- **Categorías:** Furniture, Office Supplies, Technology
- **Variables clave:** Order Date, Customer Type, Account Manager, Product Category, Cost Price, Retail Price, Order Quantity, Profit

## 🔧 Proceso técnico completo

| Fase | Descripción |
|------|-------------|
| Exploración | Análisis descriptivo de 19 variables. Detección de outliers con método IQR (112 pedidos atípicos identificados y tratados) |
| Limpieza | 0 valores nulos, 0 duplicados. Conversión de tipos, normalización de cabeceras |
| Feature Engineering | Variables derivadas: Profit, Profit_Margin_Pct, Lead_Time_Days, Year/Month/Quarter, Is_Outlier, Segmento_Cliente |
| EDA | Análisis por categoría, agente comercial, tipología de cliente y evolución temporal |
| Correlación | Matriz de correlación entre variables numéricas clave |
| Regresión Lineal | Modelo predictivo del importe del pedido con 4 predictores (R² = 0,76) |
| Segmentación | K-Means con k=3 clusters: clientes Premium, Ocasionales e Inactivos |
| Series Temporales | Análisis de crecimiento YoY y variación trimestral 2013–2017 |
| Visualización | Dashboard de 6 páginas en Power BI con insights y recomendaciones |

## ✅ Hallazgos y métricas clave

| Métrica | Valor |
|---------|-------|
| Ventas totales | 1.206.000 € |
| Beneficio total | 568.000 € |
| Margen medio | 47,13% |
| Pedidos totales | 993 |
| Crecimiento 2013 a 2015 | +83,2% |
| Caída 2015 a 2016 | -28,6% |
| Technology sobre ventas | 68,9% |
| Correlación Ventas–Beneficio | r = 0,971 |
| R² modelo regresión | 0,76 |
| Ticket medio cliente Premium | 8.186 € |

## 💼 Recomendaciones estratégicas generadas

A partir del análisis se formularon 5 recomendaciones con respaldo estadístico: reforzar la estrategia comercial en Technology, desarrollar el segmento Small Business (mayor ticket medio: 1.362 €/pedido), revisar la política de descuentos (correlación prácticamente nula con el importe del pedido), investigar y revertir la caída de 2016, y evaluar el potencial desaprovechado de la categoría Furniture.

## 🛠️ Stack tecnológico

`Power BI Desktop` `DAX` `Power Query` `Python` `pandas` `numpy` `scikit-learn` `K-Means` `Regresión Lineal` `Matplotlib`

## 📁 Estructura del repositorio

- README.md
- data/ → DataSet.xlsx
- report/ → Reto3_Dashboard.pbix
- docs/ → Informe_Analisis_Profesional.pdf, Dashboard_Preview.pdf, Presentacion_Reto3.pptx
