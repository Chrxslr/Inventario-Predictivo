# 📦 Proyecto M3 – Inventario Predictivo con Power BI  

**Autor:** Christian Daniel Lara Larios  
**Email:** larad8704@gmail.com  
**Cohorte:** DAFT-16  
**Fecha de entrega:** 2025  
**Institución:** SoyHenry – Data Analytics Bootcamp  

---

## 📌 Introducción  
Este proyecto tuvo como objetivo el diseño de un **modelo de inventario predictivo** para una empresa ficticia de retail.  
Se buscó integrar información de ventas, tiendas y factores externos con el fin de **optimizar la gestión de stock**, identificar patrones de consumo y facilitar la **toma de decisiones estratégicas**.  

---

## 🛠️ Desarrollo del proyecto  

### 🔹 Modelado de datos  
- **Datasets empleados**:  
  - `stores.csv` → información de tiendas (tipo, tamaño, ubicación).  
  - `sales.csv` → ventas históricas por semana y departamento.  
  - `features.csv` → factores externos (clima, feriados, precios de combustible, CPI, desempleo, markdowns).  

- **Transformaciones aplicadas**:  
  - Limpieza de valores nulos y duplicados.  
  - Normalización de variables (ej: tamaño de tiendas).  
  - Conversión de columnas categóricas a numéricas.  
  - Creación de llaves primarias y foráneas para un modelo relacional robusto.  

- **Modelo relacional (DER)**:  
  - `Sales` ↔ `Stores`  
  - `Sales` ↔ `Features`  
  - Relaciones 1 a muchos con claves bien definidas.  

---

### 🔹 Dashboard en Power BI  
Se construyó un tablero interactivo dividido en dos niveles de análisis:  

**1. Vista Global**  
- KPIs principales: Ventas Totales, Ingresos, COGS, Utilidad Bruta, Utilidad Neta.  
- Gráficos:  
  - Tendencia de ingresos por mes.  
  - Ventas por tipo de tienda y tamaño.  
  - Análisis de la variación interanual de ingresos.  

**2. Vista Estados Unidos**  
- KPIs: Ventas, Utilidad, Rentabilidad.  
- Mapas geográficos: clientes por estado y distribución de ingresos.  
- Gráficos comparativos: variación de ventas por categoría y departamento.  
- Segmentadores para análisis dinámico (fecha, región, tipo de tienda).  

---

## 📈 Insights principales  

- **Variación de ingresos entre períodos** → crecimiento moderado con picos estacionales (diciembre = mes clave).  
- **Departamentos más rentables** → concentran más del 70 % de las ventas totales, útiles para planificación de stock.  
- **Tiendas líderes** → pocas sucursales concentran más del 25 % de las ventas → oportunidad de replicar estrategias en tiendas de bajo rendimiento.  
- **Impacto de factores externos** → los feriados impulsan ventas un **+8 %** en promedio.  
- **Estados Unidos** → mercado con mayor potencial, pero con diferencias significativas entre regiones.  

---

## 🧭 Conclusiones y recomendaciones  

- Mantener **stock prioritario** en departamentos clave y sucursales de alto rendimiento.  
- Diseñar **campañas especiales en fechas festivas** para maximizar ingresos.  
- Implementar **estrategias regionales** en EE. UU. para equilibrar ventas entre territorios.  
- Integrar modelos predictivos de demanda (Machine Learning) en fases futuras para mayor precisión.  

---

## 🚀 Tecnologías utilizadas  
- **Power BI** → limpieza, modelado, medidas DAX y dashboards interactivos.  
- **SQL / Excel** → apoyo en transformaciones y validaciones.  
- **DAX** → KPIs, cálculos de variación y rentabilidad.  

---
