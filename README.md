# 🤖 Machine Learning

Repositorio de aprendizaje progresivo de Machine Learning con notebooks prácticos en Python.

---

## 📁 Estructura del proyecto

```
MACHINE_LEARNING/
│
├── README.md
├── requirements.txt
├── main.py
│
├── data/                        ← datasets de laboratorios
│   └── concrete.csv
│
└── notebooks/                   ← laboratorios y proyecto final
    ├── 01-regresion-lineal/
    ├── 02-regresion-logistica/
    ├── 03-regresion-logistica-gd/
    ├── 04-mlp-capas-fijas/
    ├── 05-mlp-matricial/
    └── 06-proyecto-final/
        └── data/                ← datasets específicos del proyecto
            ├── adult.csv
            └── housing.csv
```

---

## 📓 Laboratorios

| # | Laboratorio | Temas | Dataset |
|---|---|---|---|
| 01 | [Regresión Lineal](notebooks/01-regresion-lineal/lab_01_regresion_lineal.ipynb) | OLS, estandarización, polinomial, sesgo-varianza | `data/concrete.csv` |
| 02 | [Regresión Logística](notebooks/02-regresion-logistica/lab_02_regresion_logistica.ipynb) | OLS vs logística, sigmoide, outliers, métricas de clasificación | Sintético (`make_classification`) |
| 03 | [Logística con Gradient Descent](notebooks/03-regresion-logistica-gd/lab_03_regresion_logistica.ipynb) | BCE, gradiente vectorizado, GD manual, clase con API sklearn | Sintético (NumPy) |
| 04 | [MLP desde Cero](notebooks/04-mlp-capas-fijas/lab_04_mlp_capas_fijas.ipynb) | Forward pass, backpropagation escalar, SGD, Early Stopping, feature scaling | Breast Cancer (sklearn) |
| 05A | [MLP Matricial — CCE](notebooks/05-mlp-matricial/lab_05a_mlp_cce.ipynb) | MLP vectorizado, ReLU, Softmax, CCE, inicializaciones (Normal/Xavier/He) | Sintético (`make_moons`) |
| 05B | [MLP Matricial — MSE](notebooks/05-mlp-matricial/lab_05b_mlp_mse.ipynb) | MLP vectorizado, regresión, identidad, MSE, superficie 3D | Sintético (NumPy) |

---

## 🎓 Proyecto Final

| Entrega | Notebook | Temas | Datasets |
|---|---|---|---|
| Parcial | [Entrega Parcial](notebooks/06-proyecto-final/proyecto_final_entrega_parcial.ipynb) | EDA, preprocesamiento, regresión lineal y logística con GD desde cero | `adult.csv`, `housing.csv` |
| Final | — | MLP configurable, comparación con modelos lineales | `adult.csv`, `housing.csv` |

---

## 🚀 Cómo ejecutar

### Opción 1 Local

```bash
git clone https://github.com/tu-usuario/MACHINE_LEARNING.git
cd MACHINE_LEARNING
pip install -r requirements.txt
jupyter notebook
```

### Opción 2 Google Colab

Reemplaza `github.com` por `githubtocolab.com` en la URL de cualquier notebook,
o haz clic en el enlace y luego en **"Open in Colab"**.

> Para ell proyecto final, sube la carpeta `06-proyecto-final/data/` a tu entorno de Colab
> o monta tu Google Drive antes de ejecutar.

---

## 🛠️ Requisitos

```txt
numpy>=1.24.0
pandas>=2.0.0
matplotlib>=3.7.0
scikit-learn>=1.3.0
plotly>=5.0.0
jupyter>=1.0.0
notebook>=7.0.0
```

Ver [`requirements.txt`](requirements.txt) para la lista completa.

---

## 📌 Notas

- Los laboratorios 01–05 son ejercicios guiados con celdas `# TODO` y análisis de resultados.
- El lab 05 usa el **patrón Strategy** para intercambiar inicializaciones sin duplicar código.
- El proyecto final (06) implementa pipelines completos sobre datos reales con clases en NumPy.
- Los datasets de laboratorio están en `data/`; los del proyecto en `notebooks/06-proyecto-final/data/`.