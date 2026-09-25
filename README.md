**GRUPO 10**

# 🎲 Detección de Perfiles de Riesgo en Apuestas Deportivas (Ludopatía)

## 📌 Resumen del Proyecto y Problemática Social
En los últimos años, el acceso masivo a plataformas de casino virtual y apuestas deportivas ha desatado una crisis silenciosa de ludopatía, afectando fuertemente a jóvenes y adolescentes. Mientras que muchas problemáticas sociales se centran en factores ambientales o de infraestructura, la adicción al juego online representa una amenaza directa a la salud mental y la estabilidad económica de miles de familias.

Este proyecto tiene como objetivo utilizar técnicas de Data Science y Machine Learning para analizar el comportamiento transaccional de usuarios en plataformas de apuestas. El fin último es lograr perfilar matemáticamente a los "jugadores de riesgo" (comportamientos compulsivos, aumento drástico de montos apostados, alta frecuencia) para el potencial desarrollo de sistemas de alerta temprana o prevención.

## 📊 Sobre el Dataset
Para este análisis se utiliza el **Sports Betting Profiling Dataset** (obtenido de Kaggle), el cual simula con precisión el ecosistema real de una casa de apuestas. 

* **Volumen:** 100.000 registros (apuestas) distribuidos en 5.000 usuarios únicos.
* **Variables principales:** 
  * `stake`: Monto de la apuesta.
  * `odds`: Cuota o probabilidad de la apuesta.
  * `sport` y `bet_type`: Deporte elegido y tipo de apuesta (Simple/Combinada).
  * `is_win`, `gain` y `GGR`: Resultados financieros tanto para el jugador como para la casa de apuestas.

## 🚀 Avances del proyecto hasta ahora

1. **Análisis Exploratorio de Datos (EDA):** Generación de estadísticas descriptivas y visualizaciones clave para entender la distribución de las apuestas y el comportamiento general de los usuarios.
2. **Limpieza y Valores Faltantes:** Identificación y tratamiento de datos nulos para asegurar la calidad de la información.
3. **Detección de Outliers:** Aplicación de métodos estadísticos (como el Rango Intercuartílico - IQR) para aislar apuestas de montos extremos que podrían sesgar los modelos predictivos posteriores.
4. **Transformación de Datos (Feature Engineering):** Codificación de variables categóricas (como el deporte o el tipo de apuesta) para su uso en algoritmos matemáticos.
5. **Estandarización:** Escalado de variables numéricas con diferentes rangos (ej. `stake` vs `odds`) preparándolas para la futura ingesta en modelos de Machine Learning.

## 📁 Archivos del Repositorio
* `bets_final.csv`: Dataset original utilizado para el análisis.
* `ludopatiaEDA.ipynb`: Jupyter Notebook con el código detallado del Análisis Exploratorio de Datos, gráficos y transformaciones.

## 🛠️ Tecnologías Utilizadas
* Python (Pandas, NumPy)
* Matplotlib / Seaborn (Visualización)
* Scikit-Learn (Preprocesamiento y Estandarización)
