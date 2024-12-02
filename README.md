# **Predicción de Abandono Laboral (Attrition)** 🏢🚪

Este proyecto analiza las posibles razones detrás del abandono laboral utilizando un enfoque de machine learning. Se emplearon varios modelos predictivos para generar insights clave que pueden ayudar a las empresas a mejorar la retención de talento y tomar decisiones basadas en datos.

---

## **🎯 Objetivo**
Identificar los factores que influyen en el abandono laboral y predecir la probabilidad de que un empleado deje la empresa mediante modelos de clasificación binaria.

---

## **📂 Estructura del Proyecto**
- **data/**: Datos ficticios empleados en el análisis.
- **notebooks/**: Notebooks para exploración de datos, modelado y evaluación.
- **src/**: Código fuente para preprocesamiento, modelado y generación de reportes.
- **models/**: Modelos entrenados.
- **outputs/**: Resultados generados, como gráficas e informes.

---

## **📊 Datos Utilizados**
### Fuente
Los datos son ficticios, diseñados para simular un entorno corporativo con información de empleados.

### Principales Variables:
- `Age`: Edad.
- `MaritalStatus`: Estado civil.
- `JobSatisfaction`: Satisfacción laboral.
- `EnvironmentSatisfaction`: Satisfacción con el entorno laboral.
- `MonthlyIncome`: Salario mensual.
- `YearsAtCompany`: Años en la empresa.
- `Attrition`: Variable objetivo (1: Abandono, 0: Permanencia).

---

## **🔍 Metodología**
1. **Análisis Exploratorio de Datos (EDA)**:
   - Identificación de patrones y visualización de correlaciones entre variables clave.
   - Ejemplo: Se observaron mayores tasas de abandono en empleados jóvenes y con roles técnicos.

2. **Preprocesamiento**:
   - Codificación de variables categóricas.
   - Estandarización de variables numéricas.
   - Manejo de valores nulos con técnicas de imputación.

3. **Modelos Utilizados**:
   - **Regresión Logística**: Modelo lineal para interpretar relaciones entre variables.
   - **Random Forests**: Modelo no lineal para manejar interacciones complejas.
   - **XGBoost**: Modelo avanzado para capturar patrones más profundos.

4. **Evaluación**:
   - Se compararon los modelos mediante métricas como precisión, recall, F1-score y AUC-ROC.
   - El modelo **XGBoost** presentó el mejor rendimiento global.

---

## **📈 Resultados**
### Conclusiones:
1. **Factores clave identificados**:
   - `MaritalStatus`: Los empleados divorciados tienen mayor probabilidad de abandonar.
   - `JobSatisfaction` y `EnvironmentSatisfaction`: La satisfacción laboral y con el entorno influyen significativamente en la retención.
   - `JobRole`: Los roles técnicos, como "Laboratory Technician" y "Healthcare Representative", están más asociados al abandono.
   - `YearsAtCompany`: Los empleados con menos años en la empresa tienen mayores tasas de abandono.

2. **Rendimiento de los modelos**:
   - **XGBoost**: Mejor precisión y recall, ideal para predecir correctamente los casos positivos (abandono).
   - **Random Forests**: Buen rendimiento, pero menos interpretable.
   - **Regresión Logística**: Útil para interpretar relaciones, aunque con menor rendimiento en comparación.

---

## **⚙️ Cómo Usar**
### Requisitos
- Python >= 3.8
- Librerías: pandas, scikit-learn, xgboost, matplotlib, seaborn

### Pasos
1. Clona este repositorio:
   ```bash
   git clone https://github.com/usuario/attrition-prediction.git
   cd attrition-prediction
