# omics-like-ml-demo
Mini-proyecto: clasifica **Tumor vs Normal** con un dataset **sintético de alta dimensión** (miles de “genes”). Entreno **Regresión Logística** y **Random Forest**, reporto **AUROC/AUPR**, dibujo **ROC/PR** y muestro **importancias**.

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/davidagracastroIA/omics-like-ml-demo/blob/main/omics_like_demo.ipynb)

## Cómo ejecutar
1. Abre el notebook en Colab (botón de arriba).  
2. Conecta el runtime y pulsa **Runtime → Run all**.  
3. Al final verás las métricas y se guardará `omics_sintetico_rf.joblib`.

## Resultados (mi ejecución)
- Logistic Regression — **AUROC: 0.966**, **AUPR: 0.967**  
- Random Forest      — **AUROC: 0.987**, **AUPR: 0.986**  
Figuras: ROC/PR para ambos modelos + Importancias (Gini).

## Contenido
├─ omics_like_demo.ipynb
├─ README.md
├─ figs/
│ ├─ pr_logistic.png
│ ├─ pr_rf.png
│ ├─ roc_logistic.png
│ └─ roc_rf.png
└─ omics_sintetico_rf.joblib

## Requisitos (para ejecutar en local)
pandas
numpy
scikit-learn
matplotlib
joblib

## Nota ética
Dataset **sintético** que emula expresión génica de alta dimensión → **solo educativo; no uso clínico**. El flujo es el mismo que para ómics reales (TCGA/GEO) cambiando la carga de datos.
