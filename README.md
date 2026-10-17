# Sistema de Alerta Temprana de Sequía a 14 Días en el Embalse Mazar

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/elianyepez21/Sistema-de-Alerta-Mazar/blob/main/ProyectoFinal_ML.ipynb)

Este proyecto desarrolla un sistema predictivo para anticipar con **14 días de antelación** si la cota del embalse Mazar (Ecuador) caerá por debajo del umbral crítico de **2,120 msnm**, utilizando datos hidrológicos y energéticos de CELEC (2023–2025).

---

## 📌 Resumen de Hallazgos Principales

1. **Regresión Logística vs. Random Forest:** La Regresión Logística superó significativamente a Random Forest tanto en rendimiento global (PR-AUC de 0.942 vs 0.911, $p = 0.004$) como en la captura del inicio de las crisis (0.757 vs 0.606, $p < 0.0001$).
2. **Proyección Física:** Proyectar la tendencia lineal del nivel del agua demostró ser el predictor más fuerte al capturar el arranque de las sequías (PR-AUC de 0.858), confirmando que la inercia del embalse domina la señal predictiva.
3. **Confiabilidad Operativa:** La Regresión Logística capturó el 89% de los días de riesgo con un margen de anticipación de 14 a 18 días en crisis reales, manteniendo un récord de **0 falsas alarmas** durante el periodo de prueba de 2025.

---

## 🛠️ Estructura del Repositorio

* `ProyectoFinal_ML.ipynb`: Notebook autorcontenido con el pipeline de datos, gráficos (t-SNE, curvas ROC/PR, matrices de confusión), validación cruzada con purga temporal y pruebas de hipótesis (Wilcoxon).

---

## 🚀 Cómo ejecutar el proyecto

1. Haz clic en el botón superior **"Open in Colab"** para abrir directamente la notebook en Google Colab.
2. Sigue las instrucciones de cada celda para ejecutar secuencialmente el preprocesamiento, entrenamiento y evaluación estadística.
