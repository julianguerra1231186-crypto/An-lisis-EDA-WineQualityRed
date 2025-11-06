<!-- 🎨 PORTADA -->
<h1 align="center">🍷 Análisis Exploratorio de Datos – Wine Quality Red</h1>

<p align="center">
  <b>Proyecto Final | Universidad Corhuila</b><br>
  <i>Materia: Minería de Datos</i> · <i>Docente: Julian Quimbayo </i>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.11+-blue?logo=python&logoColor=white"/>
  <img src="https://img.shields.io/badge/Pandas-Data%20Analysis-purple?logo=pandas"/>
  <img src="https://img.shields.io/badge/Scikit--Learn-Modelado%20Predictivo-orange?logo=scikit-learn"/>
  <img src="https://img.shields.io/badge/Matplotlib%20%7C%20Seaborn-Visualización-green?logo=plotly"/>
  <img src="https://img.shields.io/badge/Status-Completo-success"/>
</p>

---

## 🧠 Descripción General
Este proyecto desarrolla un **Análisis Exploratorio de Datos (EDA)** sobre el dataset **Wine Quality Red**, con el objetivo de **identificar los factores químicos que más influyen en la calidad del vino tinto** y construir un modelo predictivo basado en regresión lineal.

> 🍇 *El vino es ciencia, arte y datos. Este análisis descubre qué lo hace realmente bueno.*

---

## 📦 Dataset
- **Fuente:** [UCI Machine Learning Repository – Wine Quality Data Set](https://archive.ics.uci.edu/ml/machine-learning-databases/wine-quality/winequality-red.csv)  
- **Registros:** 1.599  
- **Variables:** 12 (11 predictoras + 1 objetivo `quality`)  
- **Tipo de problema:** Regresión  
- **Contexto:** Análisis químico de vinos tintos de Portugal para evaluar su calidad sensorial.

---

## ⚙️ Flujo del Proyecto
El proyecto sigue los **11 pasos definidos por la Guía EDA del curso**, garantizando una estructura completa y replicable:

| Paso | Descripción | Estado |
|------|--------------|--------|
| 1️⃣ | Importación y descripción del dataset | ✅ |
| 2️⃣ | Análisis inicial y revisión de valores faltantes | ✅ |
| 3️⃣ | Limpieza de datos y eliminación de duplicados | ✅ |
| 4️⃣ | Conversión de variables categóricas (LabelEncoder) | ✅ |
| 5️⃣ | Normalización (MinMaxScaler) | ✅ |
| 6️⃣ | Visualizaciones: Histogramas, Boxplots, Dispersión, Pastel | ✅ |
| 7️⃣ | Correlación (Spearman) | ✅ |
| 8️⃣ | Test de Normalidad (Shapiro-Wilk) | ✅ |
| 9️⃣ | Pregunta de investigación | ✅ |
| 🔟 | Modelo predictivo (Regresión Lineal) | ✅ |
| 1️⃣1️⃣ | Conclusiones finales y recomendaciones | ✅ |

---

## 📊 Principales Hallazgos

### 🔬 Variables más influyentes en la calidad
| Variable | Influencia | Tipo de relación |
|-----------|-------------|------------------|
| **Alcohol** | 🍷 Muy alta | Positiva |
| **Sulphates** | ⚗️ Alta | Positiva |
| **Citric acid** | 🍋 Media | Positiva |
| **Volatile acidity** | 💨 Alta | Negativa |
| **Density** | 🌡️ Moderada | Negativa |

> 🧩 *A mayor contenido de alcohol y sulfatos, mayor suele ser la puntuación de calidad; una alta acidez volátil reduce el puntaje.*

---

## 📈 Resultados del Modelo
- **Modelo aplicado:** Regresión Lineal  
- **Métricas de rendimiento:**
  - 🔹 **R²:** ≈ 0.40  
  - 🔹 **MSE / RMSE:** valores moderados, dentro de rango aceptable  
  - 🔹 El modelo explica el **40% de la variabilidad** en la calidad del vino.  
- **Interpretación:**  
  Aunque la regresión lineal es simple, logró identificar de forma clara las variables químicas determinantes en la calidad del vino.

---

## 🧩 Conclusiones
- El dataset no contiene valores faltantes y fue depurado de 240 duplicados.  
- La **correlación de Spearman** evidenció relaciones químicas importantes, como *alcohol–density* (-0.78).  
- El modelo mostró un desempeño **estable y coherente con la realidad química**.  
- Se comprobó que las propiedades químicas explican una parte sustancial de la calidad del vino tinto.  
- Este análisis sienta las bases para modelos más complejos con mejor capacidad predictiva.

---

## 🚀 Recomendaciones Futuras
1. Aplicar modelos no lineales como **Random Forest, XGBoost o Redes Neuronales**.  
2. Agregar variables sensoriales y de proceso (color, aroma, fermentación).  
3. Comparar resultados entre **vinos tintos y blancos**.  
4. Usar técnicas de **balanceo de clases** para mejorar el aprendizaje del modelo.

---

## 🛠️ Tecnologías Utilizadas
| Herramienta | Uso Principal |
|--------------|----------------|
| 🐍 **Python 3.11+** | Lenguaje principal |
| 📊 **Pandas / NumPy** | Limpieza y manipulación de datos |
| 📈 **Matplotlib / Seaborn** | Visualización de datos |
| 🧮 **Scikit-learn** | Normalización, modelado y evaluación |
| 🧰 **Google Colab / Jupyter** | Entorno de desarrollo |
| 🤖 **Asistencia de GPT-5 (ChatGPT)** | Apoyo en redacción técnica, estructuración del análisis y revisión del código |



---

## 💡 Pregunta de Investigación
> **¿Qué variables químicas influyen con mayor fuerza en la calidad del vino tinto y hasta qué punto pueden predecir su puntuación final?**

✅ **Específica:** se centra solo en la variable `quality`.  
📊 **Medible:** se evalúa mediante métricas (R², MSE).  
🍇 **Relevante:** conecta directamente con la composición química y la percepción sensorial del vino.

---

## 🧾 Conclusión Final
> El análisis realizado demuestra que la **calidad del vino tinto** puede predecirse parcialmente a partir de sus características químicas.  
> Variables como el **alcohol, los sulfatos y el ácido cítrico** son determinantes en la calificación final del vino, mientras que la **acidez volátil y la densidad** afectan negativamente su puntuación.  
>  
> Aunque el modelo de regresión lineal explica un 40% de la variabilidad, constituye una base sólida para avanzar hacia modelos predictivos más sofisticados que integren factores sensoriales y no lineales.

---

## 💬 Autor y Contacto
👤 **Julián Guerra**  
📍 Neiva – Huila, Colombia  
🏢 Universidad-Corhuila
📧 [(correo:Jaguerra20201@corhuila.edu.co)  

---

<p align="center">
  <i>“La ciencia de los datos es el vino del conocimiento: entre más se analiza, más sabor deja.” 🍇</i>
</p>
