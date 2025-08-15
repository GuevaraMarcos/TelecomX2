````markdown
# Challenge Telecom X: Análisis de Evasión de Clientes - Parte 2

## 📌 Descripción del Proyecto
Este proyecto corresponde a la segunda parte del **"Challenge Telecom X"**, cuyo objetivo es desarrollar modelos predictivos para identificar clientes con alta probabilidad de cancelar sus servicios (**Churn**) en una empresa de telecomunicaciones.

El flujo de trabajo implementado incluye:
- **Preparación y transformación de datos** (One-Hot Encoding, escalado, manejo de desbalance con SMOTE).
- **Análisis exploratorio** para conocer la distribución y correlaciones de variables.
- **Entrenamiento y evaluación** de modelos de clasificación.
- **Interpretación de resultados** con análisis de importancia de variables.
- **Generación de conclusiones** estratégicas para mitigar la pérdida de clientes.

---

## 🎯 Objetivos
1. Preparar los datos para el modelado, codificando variables categóricas y normalizando datos.
2. Manejar el desbalance de clases mediante técnicas de sobremuestreo (SMOTE).
3. Entrenar modelos de clasificación (Random Forest, XGBoost, KNN).
4. Evaluar el rendimiento de los modelos con métricas como Accuracy, Precision, Recall, F1-score y AUC.
5. Analizar la importancia de las variables más influyentes en la predicción del churn.

---

## 📂 Datos Utilizados
- **Archivo:** `data_preprocesada.csv`  
- **Contenido:** Información de clientes de Telecom X:
  - Datos demográficos.
  - Servicios contratados.
  - Estado de evasión (**Churn**: Sí/No).

---

## ⚙️ Librerías Utilizadas
El notebook utiliza las siguientes librerías principales:

```bash
pandas==1.5.3
numpy==1.24.0
matplotlib==3.6.3
seaborn==0.11.2
scikit-learn
imbalanced-learn==0.0
xgboost==1.4.2
````

---

## 🔄 Flujo del Proceso

1. **Importación de librerías**
   Configuración inicial y carga de dependencias.

2. **Carga de datos**
   Lectura del archivo `data_preprocesada.csv` y exploración inicial.

3. **Codificación de variables categóricas**
   Uso de **One-Hot Encoding** con `OneHotEncoder` para transformar variables categóricas a formato numérico.

4. **Separación de variables**
   Definición de `X` (predictores) e `y` (variable objetivo `Churn`).

5. **División de datos**
   Uso de `train_test_split` con estratificación para mantener la proporción de clases.

6. **Manejo del desbalance**
   Aplicación de **SMOTE** para equilibrar la cantidad de ejemplos entre las clases.

7. **Entrenamiento de modelos**

   * **Random Forest**
   * **XGBoost**
   * **K-Nearest Neighbors (KNN)**

8. **Evaluación de modelos**
   Cálculo de métricas (Accuracy, Precision, Recall, F1-score) y generación de **matrices de confusión**.

9. **Interpretación de resultados**

   * Importancia de variables en modelos de árboles.
   * Comparativa de desempeño entre modelos.

---

## 📊 Resultados Esperados

* Lista de variables más influyentes en el churn.
* Comparativa clara entre modelos.
* Métricas clave para la toma de decisiones.
* Recomendaciones estratégicas basadas en los hallazgos.

---

## ▶️ Ejecución

### 1️⃣ Clonar repositorio

```bash
git clone https://github.com/usuario/Challenge-TelecomX-Parte2.git
cd Challenge-TelecomX-Parte2
```

### 2️⃣ Crear entorno virtual e instalar dependencias

```bash
python -m venv env
source env/bin/activate  # Linux/Mac
env\Scripts\activate     # Windows

pip install -r requirements.txt
```

**Archivo `requirements.txt`:**

```
pandas==1.5.3
numpy==1.24.0
matplotlib==3.6.3
seaborn==0.11.2
scikit-learn
imbalanced-learn==0.0
xgboost==1.4.2
```

### 3️⃣ Ejecutar análisis

1. Colocar `data_preprocesada.csv` en la carpeta `data/`.
2. Abrir `Untitled1.ipynb` en **Jupyter Notebook** o **VS Code**.
3. Ejecutar todas las celdas en orden.

---

## 📜 Licencia

Este proyecto se distribuye bajo licencia **MIT**. Puedes utilizarlo y modificarlo libremente citando la fuente original.
