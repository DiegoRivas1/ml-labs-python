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
├── data/               ← datasets utilizados
└── notebooks/          ← laboratorios prácticos
    ├── 01-regresion-lineal/
    ├── 02-regresion-logistica/
    ├── 03-regresion-logistica-gd/
    └── 04-mlp-capas-fijas/
```

---

## 📓 Notebooks

| # | Laboratorio | Temas | Dataset |
|---|---|---|---|
| 01 | [Regresión Lineal](notebooks/01-regresion-lineal/lab_01_regresion_lineal.ipynb) | OLS, estandarización, polinomial, sesgo-varianza | `data/concrete.csv` |
| 02 | [Regresión Logística](notebooks/02-regresion-logistica/lab_02_regresion_logistica.ipynb) | OLS vs logística, sigmoide, outliers, métricas de clasificación | Sintético (`make_classification`) |
| 03 | [Logística con Gradient Descent](notebooks/03-regresion-logistica/lab_03_regresion_logistica.ipynb) | BCE, gradiente vectorizado, GD manual, clase con API sklearn | Sintético (NumPy) |
| 04 | [MLP desde Cero](notebooks/04-mlp-capas-fijas/lab_04_mlp_capas_fijas.ipynb) | Forward pass, backpropagation escalar, SGD, Early Stopping, feature scaling | Breast Cancer (sklearn) |

> 🔄 Se irán agregando nuevos notebooks progresivamente.

---

## 🚀 Cómo ejecutar

### Opción 1: Local

```bash
# Clonar el repositorio
git clone https://github.com/tu-usuario/MACHINE_LEARNING.git
cd MACHINE_LEARNING

# Instalar dependencias
pip install -r requirements.txt

# Abrir Jupyter
jupyter notebook
```

### Opción 2: En la nube (sin instalar nada)

Abre cualquier notebook directamente en Google Colab haciendo clic en el enlace
del laboratorio y luego en el botón **"Open in Colab"**, o reemplazando
`github.com` por `githubtocolab.com` en la URL.

---

## 🛠️ Requisitos

Ver [`requirements.txt`](requirements.txt) para la lista completa de dependencias.

---

## 📌 Notas

- Cada notebook es independiente y contiene explicaciones en celdas Markdown.
- Los datasets usados se encuentran en la carpeta `data/`.