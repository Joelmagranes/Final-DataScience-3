# 🎥 Análisis de Sentimientos en Reseñas de Películas

## 🎯 Objetivo
Desarrollar un modelo capaz de clasificar reseñas de películas como positivas o negativas, utilizando técnicas de Procesamiento de Lenguaje Natural (NLP) y modelos de clasificación supervisada, tanto clásicos como de Deep Learning.

---

## 📂 Dataset
**movies_reviews**  
- 46.173 reseñas de películas en inglés.  
- Cada reseña incluye un **Rating** de 1 a 10 y el nombre de la película.  
- La variable objetivo (**Sentiment**) se derivó del rating:  
  - **1–4 → negativo**  
  - **7–10 → positivo**  
  - Se descartaron los valores neutros (5–6).

---

## ⚙️ Preprocesamiento
Se aplicaron técnicas básicas de NLP:

- Normalización del texto  
- Tokenización  
- Eliminación de stopwords  
- Lematización  
- Vectorización con:
  - **CountVectorizer**
  - **TF‑IDF**

---

## 🤖 Modelado
Se entrenaron y compararon modelos clásicos:

- Naive Bayes Multinomial  
- Regresión Logística  
- Random Forest  
- SVM (LinearSVC)

Además, se entrenó una **red neuronal densa (MLP)** sobre la representación TF‑IDF para comparar su desempeño con el mejor modelo clásico.

---

## 📁 Contenido del repositorio
- `EntregaFinal_DataScience3_JoelMagranes.ipynb` → desarrollo completo del proyecto  
- `movies_reviews/` → dataset utilizado  
- `README.md` → descripción del proyecto
