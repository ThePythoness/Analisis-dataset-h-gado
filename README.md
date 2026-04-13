# 🏥 Análisis Bioquímico para la Detección de Enfermedades Hepáticas

Este repositorio contiene un análisis exploratorio de datos (EDA) y un estudio estadístico de un dataset de pacientes con trastornos hepáticos. El objetivo es identificar qué marcadores bioquímicos (enzimas, proteínas y bilirrubinas) tienen mayor relevancia en el diagnóstico médico.

## 📋 Descripción del Proyecto
El proyecto aborda el análisis de un conjunto de datos médicos que incluye variables demográficas y resultados de pruebas de laboratorio. A través de este análisis, se busca entender la relación entre los diferentes biomarcadores y la presencia de patologías.

## 🛠️ Tecnologías Utilizadas
* **Lenguaje:** Python 3.x
* **Librerías:**
  * `Pandas`: Manipulación y limpieza de datos.
  * `Numpy`: Cálculos estadísticos.
  * `Matplotlib` & `Seaborn`: Visualización avanzada de datos (Histogramas, Boxplots, Heatmaps).

## 🔍 Análisis Realizado

### 1. Estadísticos Descriptivos
Se calcularon medidas de tendencia central y dispersión (media, desviación estándar, varianza, rango e IQR) para las variables principales como la Bilirrubina Total (TB) y Directa (DB).

### 2. Caracterización de Distribuciones
Análisis de la forma y simetría mediante histogramas para:
* **TB, DB, Alkphos y Sgpt.**
* **Hallazgo:** Se observó una asimetría positiva severa, indicando la presencia de casos críticos con valores muy elevados.

### 3. Detección de Valores Atípicos (Outliers)
Utilización de diagramas de caja (Boxplots) para identificar casos clínicos extremos en:
* **Sgot:** 66 atípicos identificados (indicador de daño agudo).
* **ALB:** 0 atípicos (indicador de estabilidad funcional).
* **TP y A/G Ratio:** Estabilidad moderada con pocos atípicos.

### 4. Matriz de Correlación
Estudio de las interrelaciones entre variables:
* **Alta Colinealidad:** Fuertes relaciones entre TB-DB (0.87) y Sgpt-Sgot (0.79).
* **Predictores Clave:** Las bilirrubinas mostraron la mayor correlación negativa con el estado de salud del paciente (Selector).
* **Independencia:** La edad y el género no mostraron una correlación significativa con la gravedad de los niveles bioquímicos.

## 🚀 Cómo usar este repositorio
1. Clona el repositorio:
   ```bash
   git clone [https://github.com/TU_USUARIO/NOMBRE_REPOSITORIO.git](https://github.com/TU_USUARIO/NOMBRE_REPOSITORIO.git)
