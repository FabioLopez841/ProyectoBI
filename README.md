# 📈 Optimización de Gastos de Marketing en Showz

## 🧩 Descripción del Proyecto

Como parte de mis prácticas en el departamento de analítica de **Showz**, una plataforma de venta de entradas para eventos, recibí el desafío de analizar datos históricos para **optimizar el gasto en marketing**.

---

## 🎯 Objetivo

Analizar el comportamiento de los usuarios, los patrones de compra y el impacto de las campañas de marketing para:

- Entender **cómo y cuándo los clientes utilizan la plataforma**.
- Calcular cuánto dinero aporta cada cliente (**LTV**).
- Determinar **el retorno de la inversión en marketing** (**ROMI**).
- Identificar **las fuentes publicitarias más efectivas y rentables**.

---

## 🗃️ Conjunto de Datos

Los datos abarcan el periodo de **enero de 2017 a diciembre de 2018** e incluyen:

- **Visitas:** registros del servidor con información de sesiones de usuario.
- **Pedidos:** historial de compras realizadas en la plataforma.
- **Costos:** estadísticas diarias de gastos publicitarios por fuente.

Tamaño del dataset:  
- Visitas:  [uid, dispositivo, fecha/hora, fuente]  
- Pedidos:  [uid, fecha/hora de compra, ingreso generado]  
- Costos:   [fuente de adquisición, fecha, monto gastado]

---

## 📊 KPIs y Métricas Analizadas

- **Visitas**
  - Usuarios únicos por día, semana y mes
  - Número de sesiones diarias
  - Duración promedio de sesión
  - Frecuencia de retorno de los usuarios

- **Ventas**
  - Tiempo desde la primera visita hasta la primera compra (conversiones 0d, 1d, etc.)
  - Número total de pedidos
  - Tamaño promedio de compra
  - Valor de vida del cliente (**LTV**)

- **Marketing**
  - Gasto total y por fuente de adquisición
  - **CAC** (Costo de Adquisición de Clientes)
  - **ROMI** (Retorno sobre la Inversión en Marketing)

---

## 📈 Herramientas y Tecnologías

- Python (Pandas, NumPy, Matplotlib, Seaborn)
- Jupyter Notebook
- Exploración de Datos (EDA)
- Análisis de cohortes y rendimiento por canal

---

## 🧠 Principales Insights

- Algunas fuentes publicitarias generan **mayor LTV con menor CAC**, siendo candidatas ideales para reinversión.
- La mayoría de las conversiones suceden **el mismo día o al día siguiente** de la primera visita.
- Las campañas que atraen desde **dispositivos móviles** generan más tráfico, pero no siempre más ingresos.
- **Menos del 20% de las fuentes de marketing generan más del 80% del retorno** (principio de Pareto).

---

## 🧾 Recomendaciones

- **Invertir en las fuentes con ROMI positivo y alto**.
- Reasignar presupuesto desde campañas de bajo rendimiento hacia canales con mejor conversión y rentabilidad.
- Implementar una estrategia de **retención de usuarios recurrentes**, quienes tienden a generar mayor ingreso a largo plazo.

---

## 📂 Estructura del Proyecto

```bash
├── data/
│   ├── visits_log_us.csv
│   ├── orders_log_us.csv
│   └── costs_us.csv
├── notebooks/
│   └── marketing_analytics_showz.ipynb
├── README.md
