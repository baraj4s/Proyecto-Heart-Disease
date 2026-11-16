
<div align="center">

# ❤️ HEART DISEASE
### Análisis y predicción de enfermedades cardíacas utilizando Machine Learning

**Proyecto de Aprendizaje de Máquina — Grupo C1**

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![Scikit Learn](https://img.shields.io/badge/Scikit--learn-F7931E?style=for-the-badge&logo=scikitlearn&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=for-the-badge&logo=jupyter&logoColor=white)

[📂 REPOSITORIO](https://github.com/baraj4s/Proyecto-Heart-Disease)
[📊 DATASET](https://www.kaggle.com/datasets/johnsmith88/heart-disease-dataset)

</div>

---

<div align="center">

![Heart Disease](images/heart-disease-banner.jpg)

</div>

---

## 👥 Integrantes

| Integrante | Código | Correo |
|:---|:---:|:---|
| Angel Santiago Barjas | 2251511 | angelsantybarajas@gmail.com |
| Miguel Angel Plata | 2211245 | mikevideos45@gmail.com |

**Grupo:** C1  
**Periodo:** 2026-2  
**Profesora:** Alejandra Moreno  
**Asignatura:** Aprendizaje de Máquina

---

## 📌 Descripción del proyecto

Heart Disease es un proyecto académico enfocado en el análisis de datos clínicos y la aplicación de algoritmos de Machine Learning para estudiar y predecir enfermedades cardíacas.

A partir de un conjunto de datos que contiene información de pacientes, se desarrollan diferentes técnicas de análisis exploratorio, clasificación y regresión con el propósito de identificar patrones relevantes en las variables clínicas.

El proyecto contempla la construcción y evaluación de modelos de clasificación para determinar la presencia o ausencia de enfermedad cardíaca, modelos de regresión para estimar los niveles de colesterol y una extensión de clasificación multiclase para identificar diferentes tipos de dolor torácico.

---

## 🎯 Objetivos

### Objetivo general

Desarrollar un proyecto de análisis de datos y Machine Learning que permita estudiar las características clínicas de los pacientes y construir modelos predictivos relacionados con las enfermedades cardíacas.

### Objetivos específicos

- Explorar y analizar el conjunto de datos Heart Disease.
- Identificar patrones, distribuciones y correlaciones entre variables clínicas.
- Preparar los datos para el entrenamiento de algoritmos de Machine Learning.
- Implementar modelos de clasificación binaria para predecir la presencia de enfermedades cardíacas.
- Comparar diferentes algoritmos mediante métricas de evaluación.
- Desarrollar modelos de regresión para estimar los niveles de colesterol.
- Implementar una clasificación multiclase utilizando la variable de dolor torácico.
- Analizar los resultados y seleccionar las configuraciones de modelos más adecuadas para cada problema.

---

## 📊 Dataset

Para el desarrollo del proyecto se utilizó el **Heart Disease Dataset**, obtenido de Kaggle.

**Fuente:** [Heart Disease Dataset - Kaggle](https://www.kaggle.com/datasets/johnsmith88/heart-disease-dataset)

### Características del dataset

| Característica | Descripción |
|:---|:---|
| Registros | 1.025 |
| Columnas | 14 |
| Variables predictoras | 13 |
| Variable objetivo | target |
| Valores nulos | 0 |

### Variables utilizadas

- `age`: edad del paciente.
- `sex`: sexo.
- `cp`: tipo de dolor torácico.
- `trestbps`: presión arterial en reposo.
- `chol`: nivel de colesterol.
- `fbs`: glucemia en ayunas.
- `restecg`: resultados electrocardiográficos.
- `thalach`: frecuencia cardíaca máxima.
- `exang`: angina inducida por ejercicio.
- `oldpeak`: depresión del segmento ST.
- `slope`: pendiente del segmento ST.
- `ca`: número de vasos principales.
- `thal`: resultado de la variable talasemia.
- `target`: presencia o ausencia de enfermedad cardíaca.

La variable `target` representa la clasificación binaria:
- 0: ausencia de enfermedad cardíaca.
- 1: presencia de enfermedad cardíaca.

---

## 🔬 Desarrollo del proyecto

### 1. Análisis exploratorio de datos (EDA)

En la primera etapa se realizó un análisis general del dataset para comprender su estructura y las características de las variables.

Se desarrollaron las siguientes actividades:

- Inspección de dimensiones y tipos de datos.
- Análisis estadístico descriptivo.
- Distribución de variables categóricas.
- Histogramas de variables numéricas.
- Identificación de valores atípicos mediante boxplots.
- Verificación de valores nulos.
- Análisis de correlaciones mediante mapas de calor.

### 2. Clasificación binaria

En esta etapa se entrenaron y compararon cuatro algoritmos de clasificación para identificar la presencia o ausencia de enfermedades cardíacas.

**Modelos implementados:**

- Support Vector Machine (SVM).
- Decision Tree Classifier.
- Random Forest Classifier.
- Gaussian Naive Bayes.

Se utilizaron las siguientes métricas:

- Accuracy.
- Precision.
- Recall.
- F1-score.

Se seleccionó como configuración final Random Forest con 100 estimadores y profundidad máxima de 8.

### 3. Regresión para la predicción del colesterol

Se amplió el proyecto mediante modelos de regresión, utilizando `chol` como variable objetivo.

**Modelos implementados:**

- Decision Tree Regressor.
- Random Forest Regressor.
- Support Vector Regressor (SVR).

La evaluación se realizó utilizando:

- Mean Squared Error (MSE).
- Root Mean Squared Error (RMSE).
- Mean Absolute Error (MAE).
- Coeficiente de determinación (R²).

El modelo Random Forest Regressor presentó el mejor desempeño entre los modelos evaluados.

### 4. Clasificación multiclase

Como extensión del proyecto se desarrolló una clasificación multiclase utilizando `cp` como variable objetivo.

Se implementó Random Forest Classifier para identificar las diferentes categorías de dolor torácico.

La evaluación incluyó:

- Accuracy.
- Precision.
- Recall.
- F1-score.
- Matriz de confusión.
- Reporte de clasificación.

---

## 📈 Resultados obtenidos

### Clasificación binaria

Comparación de los cuatro modelos implementados:

| Modelo | Accuracy | Precision | Recall | F1-score |
|:---|---:|---:|---:|---:|
| SVM | 98,54 % | 97,22 % | 100 % | 98,59 % |
| Decision Tree | 87,32 % | 86,24 % | 89,52 % | 87,85 % |
| Random Forest | **99,02 %** | **98,13 %** | **100 %** | **99,06 %** |
| Gaussian Naive Bayes | 82,93 % | 80,70 % | 87,62 % | 84,02 % |

Random Forest obtuvo el mejor resultado general en la comparación final, con un Accuracy de 99,02 % y un Recall de 100 %.

### Regresión del colesterol

| Modelo | RMSE | MAE | R² |
|:---|---:|---:|---:|
| Decision Tree | 46,90 | 34,02 | 0,357 |
| Random Forest | **27,37** | **20,37** | **0,781** |
| SVR | 53,80 | 35,37 | 0,154 |

Random Forest Regressor obtuvo el mejor resultado, con un R² de 0,781 y un error absoluto medio de 20,37.

### Clasificación multiclase

El modelo Random Forest alcanzó un Accuracy de 93,17 % en la clasificación de las categorías de dolor torácico.

| Métrica | Resultado |
|:---|---:|
| Accuracy | 93,17 % |
| Precision macro | 92 % |
| Recall macro | 96 % |
| F1-score macro | 93 % |

---

## 🛠️ Tecnologías utilizadas

| Tecnología | Aplicación |
|:---|:---|
| Python | Lenguaje de programación |
| Pandas | Manipulación de datos |
| NumPy | Operaciones numéricas |
| Matplotlib | Visualización de datos |
| Seaborn | Análisis gráfico |
| Scikit-learn | Entrenamiento y evaluación de modelos |
| SciPy | Análisis estadístico |
| KaggleHub | Descarga del dataset |
| Jupyter Notebook | Desarrollo del proyecto |

---

## 📁 Estructura del repositorio

```text
Proyecto-Heart-Disease/
│
├── Proyecto_AM.ipynb
│
├── README.md
│
├── Proyecto_AM.ipynb
│
├── images/
│   └── heart-disease-banner.png
│
└── requirements.txt
```

---

## ▶️ Instalación y ejecución

### 1. Clonar el repositorio

```bash
git clone https://github.com/baraj4s/Proyecto-Heart-Disease.git
```

### 2. Ingresar al directorio

```bash
cd Proyecto-Heart-Disease
```

### 3. Instalar las dependencias

```bash
pip install numpy pandas matplotlib seaborn scipy scikit-learn kagglehub jupyter
```

### 4. Ejecutar el notebook

Abrir el archivo `Proyecto_AM.ipynb` desde Jupyter Notebook o Google Colab.

Ejecutar las celdas en orden para reproducir el análisis, entrenamiento y evaluación de los modelos.

---

## 📝 Conclusiones generales

El desarrollo del proyecto permitió aplicar diferentes técnicas de Machine Learning al análisis de información clínica relacionada con enfermedades cardíacas.

En la clasificación binaria, Random Forest presentó el mejor desempeño general, alcanzando un Accuracy de 99,02 % y un Recall de 100 % en el conjunto de prueba.

En la tarea de regresión, Random Forest Regressor obtuvo el menor error y el mayor coeficiente de determinación para estimar los niveles de colesterol.

Finalmente, la extensión multiclase permitió explorar la capacidad de los algoritmos de clasificación para identificar diferentes categorías de dolor torácico, alcanzando un Accuracy de 93,17 %.

Estos resultados muestran la utilidad de las técnicas de aprendizaje automático para analizar patrones en conjuntos de datos clínicos y desarrollar modelos predictivos con fines académicos.

---

## ⚠️ Aviso

Este proyecto tiene fines académicos y educativos. Los modelos desarrollados no constituyen herramientas de diagnóstico médico ni sustituyen la evaluación de profesionales de la salud.

---

<div align="center">

**HEART DISEASE — MACHINE LEARNING PROJECT**

Desarrollado para la asignatura de Aprendizaje de Máquina.

**Grupo C1 · 2026-2**

❤️

</div>
