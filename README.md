# ChallengeTelecom-evasionClientes
Segundo desafío- Primera parte del desafío de Telecom

# 📊 Proyecto: Análisis de Evasión de Clientes en TelecomX

## 📅 Fechas de trabajo
- **Inicio:** 26 de junio  
- **Cierre:** 22 de julio  

Durante este periodo se desarrolló un análisis completo de los datos de clientes de **TelecomX** con el objetivo de comprender los factores que influyen en la evasión (*Churn*).

---

## 🔹 Objetivo
El propósito del proyecto es **identificar patrones de cancelación de clientes** y proponer **estrategias de retención** basadas en datos.

---

## 🔹 Flujo de trabajo
1. **Carga de datos**
   - Se extrajeron datos desde la API proporcionada en formato JSON.
   - Se normalizó la estructura anidada utilizando `pandas.json_normalize`.

2. **Exploración inicial**
   - Revisión de estructura y tipos de datos.
   - Análisis de valores únicos, duplicados y nulos.
   - Consulta del diccionario de datos (`TelecomX_diccionario.md`) para comprender el significado de cada columna.

3. **Limpieza de datos**
   - Conversión de columnas numéricas (`Charges.Monthly`, `Charges.Total`).
   - Eliminación de filas sin valor en `Churn`.
   - Unificación de categorías inconsistentes (ejemplo: `"No internet service"` → `"No"`).
   - Creación de la columna **`Cuentas_Diarias`** a partir de los cargos mensuales.

4. **Análisis descriptivo**
   - Cálculo de métricas: media, mediana, desviación estándar.
   - Distribución de la evasión general (Churn).
   - Análisis de churn por variables categóricas (género, contrato, método de pago, servicios).
   - Análisis de churn por variables numéricas (tenure, gasto mensual y total).

5. **Visualizaciones**
   - Gráficos de barras y pastel para churn.
   - Histogramas y boxplots para comparar categorías y valores numéricos.
   - Diagramas de dispersión (tenure vs cargos mensuales).

6. **Informe final**
   - **Introducción**: importancia del churn en telecomunicaciones.
   - **Limpieza y tratamiento de datos**: pasos realizados.
   - **EDA**: hallazgos clave respaldados con visualizaciones.
   - **Conclusiones**: perfiles de clientes con mayor churn.
   - **Recomendaciones**: estrategias para reducir la evasión (incentivar contratos largos, mejorar experiencia de pago electrónico, fidelización temprana).

---

## 🔹 Librerías utilizadas
- `pandas`
- `numpy`
- `requests`
- `matplotlib`
- `seaborn`
- `plotly.express`

---

## 🔹 Resultados principales
- La evasión es mayor en clientes con **contratos mensuales**.  
- Los clientes con **alto gasto mensual** y **bajo tiempo de permanencia (tenure)** tienen mayor probabilidad de cancelar.  
- Ciertos **métodos de pago electrónicos** están asociados a mayor churn.  
- Los servicios de **Internet y Streaming** son determinantes en la decisión de cancelación.  

---

## 🔹 Equipo
Proyecto realizado entre el **26 de junio y el 22 de julio de 2025** como parte del análisis de datos de clientes de **TelecomX LATAM**.
