# Réplica de Kesgin et al. (2025) con CatBoost

Réplica del flujo del artículo "Beyond performance: Explaining and ensuring
fairness in student academic performance prediction with machine learning"
(Applied Sciences, 2025, DOI 10.3390/app15158409). Proyecto del curso
Propuesta de Investigación 2026-2, Universidad de Lima.

## Qué hace
- Une los datos de matemática y portugués de UCI Student Performance (1,044 alumnos).
- One-hot, estandarización, partición 80/20 estratificada y SMOTE-NC (solo entrenamiento).
- Modelos: regresión logística, Random Forest, XGBoost y CatBoost (agregado).
- Métricas: exactitud, F1 y AUC. Explicabilidad con SHAP y LIME.
- Equidad por sexo: diferencia de paridad demográfica y de probabilidades igualadas.

## Cómo ejecutar
1. Abrir Replica_Kesgin_CatBoost.ipynb en Google Colab.
2. Subir student-mat.csv y student-por.csv a la carpeta de trabajo.
3. Ejecutar todo.

## Diferencias con el artículo
- No se aplica debiasing adversarial; la equidad se calcula a mano.
- Hiperparámetros tomados del artículo, sin nueva búsqueda.
- Algunos alumnos aparecen en ambos archivos, lo que puede inflar un poco los resultados.

## Fuentes
- Datos: https://archive.ics.uci.edu/dataset/320/student+performance
- Código original de los autores: https://github.com/kdrksgn/fairsynedu
