# 📌 Proyecto: Detección de Fraude con Machine Learning

Este repositorio contiene un proyecto completo de detección de fraudes en transacciones financieras utilizando técnicas avanzadas de Machine Learning y un enfoque profesional orientado a la realidad del problema.

## 📊 Descripción del problema

Detectar fraudes en un conjunto de datos real de más de 6 millones de transacciones. El gran reto de este problema es el desbalance extremo entre clases (fraudes reales representan apenas el 0.1%).

## 🔧 Tecnologías y herramientas utilizadas

- Python
- pandas, numpy
- scikit-learn
- imbalanced-learn (SMOTE)
- matplotlib, seaborn
- xgboost

## 🧠 Flujo del proyecto

1. **Carga y exploración de datos**
2. **Preprocesamiento**: eliminación de columnas irrelevantes, codificación, escalamiento
3. **Balanceo de clases**: uso de SMOTE para combatir el desbalance
4. **Ingeniería de características**: medias móviles, retardos, diferencias, sectores
5. **Entrenamiento y evaluación de modelos**: Random Forest, XGBoost, Logistic Regression
6. **Optimización de hiperparámetros**: RandomizedSearchCV
7. **Evaluación avanzada**: análisis de umbral, matriz de confusión, curva ROC y métricas personalizadas

## ✅ Resultados del mejor modelo (Random Forest optimizado)

| Métrica     | Valor   |
|-------------|---------|
| Accuracy    | 0.9990  |
| Precision   | 0.5707  |
| Recall      | 0.9757  |
| F1-score    | 0.7201  |
| ROC AUC     | 0.9991  |

## 🧩 ¿Por qué no 99% de accuracy?

Porque **accuracy no es una métrica confiable** en problemas desbalanceados. Este proyecto se enfoca en **recall y F1-score**, métricas mucho más relevantes para detectar fraudes de forma efectiva.
