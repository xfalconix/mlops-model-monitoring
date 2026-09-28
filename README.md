# MLOps: Model Drift & Bias Monitoring

![Python](https://img.shields.io/badge/Python-3.8+-3776AB?style=flat-square&logo=python&logoColor=white)
![pandas](https://img.shields.io/badge/pandas-150458?style=flat-square&logo=pandas&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=flat-square&logo=scikit-learn&logoColor=white)
![alibi-detect](https://img.shields.io/badge/alibi--detect-1A73E8?style=flat-square)
![sklego](https://img.shields.io/badge/sklego-E8A000?style=flat-square)
![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=flat-square&logo=jupyter&logoColor=white)
![LinkedIn](https://img.shields.io/badge/LinkedIn%20Learning-0A66C2?style=flat-square&logo=linkedin&logoColor=white)

Repositorio con el rework personal de los notebooks del curso de LinkedIn Learning **[MLOps Essentials: Monitoring Model Drift and Bias](https://www.linkedin.com/learning/mlops-essentials-monitoring-model-drift-and-bias)** (2023) de **Kumaran Ponnambalam**.

Ejercicios de deteccion de cambios en los datos y evaluacion de equidad, con comentarios en espanol.

**Certificado del curso:** [Ver en LinkedIn](https://www.linkedin.com/learning/certificates/a258462ee55bbd8fc518baf4c6d94597609537448bb3472bf29f4c17d01d72cf?trk=share_certificate)

---

## Notebooks del repositorio

| Archivo | Tema |
|---------|------|
| `code_03_XX Drift Detection Example.ipynb` | Comparacion de rendimiento y distribuciones; feature drift con **alibi-detect** |
| `code_06_03 Equal Opportunity Score with sklego.ipynb` | Medicion de sesgo: Equal Opportunity Score con la libreria **sklego** |

Ambos notebooks usan un dataset de aprobacion de creditos (`credit-approval-training-data.csv`, `credit-approval-prod-data.csv`, `credit-approval-fair-data.csv`) como conjuntos de ejemplo para estudiar drift y sesgo. No implementan monitorizacion continua de un servicio desplegado.

---

## Stack tecnologico

| Libreria | Uso en el repo |
|-----------|---------------|
| `pandas` | Manipulacion y analisis de datos |
| `numpy` | Operaciones numericas |
| `matplotlib` | Visualizacion de resultados |
| `scikit-learn` | Modelo base (GaussianNB), train_test_split, metricas |
| `alibi-detect` | ChiSquareDrift para deteccion de feature drift |
| `sklego` | equal_opportunity_score para medicion de sesgo |

---

## Aplicacion posible: inspeccion de cascos de buques

En un sistema de reconocimiento de biofouling, cambios en la iluminacion, la turbidez o los tipos de embarcacion podrian modificar la distribucion de las imagenes. Seria necesario comparar los datos nuevos con los de entrenamiento y evaluar el rendimiento con etiquetas verificadas.

Es un ejemplo de aplicacion de los conceptos del curso al sector maritimo; el repositorio no implementa ni despliega ese sistema de imagenes.
