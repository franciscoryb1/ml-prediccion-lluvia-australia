# ClimaMañana: Predicción de Lluvia en Australia

Proyecto académico orientado al diseño, entrenamiento y evaluación de modelos de *machine learning* para predecir la ocurrencia de lluvia (**RainTomorrow**) y el volumen estimado (**RainfallTomorrow**) a partir de variables meteorológicas históricas.

El proyecto incluye una aplicación interactiva desarrollada con **Streamlit**, que permite realizar inferencias de forma sencilla mediante una interfaz web.

---

## Objetivos

* Entrenar y evaluar modelos predictivos utilizando datos meteorológicos reales.
* Construir un flujo reproducible de preparación de datos, entrenamiento y validación.
* Desplegar un prototipo interactivo para inferencia en tiempo casi real.
* Documentar el proceso completo de análisis, modelado y uso del sistema.

---

## Funcionalidades

* Predicción **binaria** de lluvia para el día siguiente (`RainTomorrow`).
* Predicción del **volumen estimado** de lluvia (`RainfallTomorrow`).
* Interfaz web para ingresar variables climáticas y visualizar resultados.

---

## Tecnologías

* **Python**
* **Pandas / NumPy**
* **Scikit-learn**
* **TensorFlow** (modelos utilizados en `app.py`)
* **Streamlit**

---

## Requisitos

* Python 3.9 o superior
* Entorno virtual (recomendado)
* Dependencias listadas en `requirements.txt`

---

## Instalación y configuración

1. Crear y activar un entorno virtual (opcional):

```bash
python -m venv .venv
source .venv/bin/activate  # Linux / Mac
.venv\\Scripts\\activate     # Windows
```

2. Instalar dependencias:

```bash
pip install -r requirements.txt
```

---

## Ejecución de la aplicación

Desde la raíz del proyecto ejecutar:

```bash
streamlit run main.py
```

La aplicación abrirá automáticamente un navegador local con la interfaz interactiva.

---

## Estructura del proyecto

```
.
├── main.py            # Aplicación Streamlit
├── app.py             # Clases y utilidades de modelos
├── pipelines/         # Pipelines entrenados (.joblib)
├── assets/            # Recursos estáticos
├── *.ipynb            # Notebooks de exploración y entrenamiento
├── *.csv              # Datasets de trabajo
└── README.md
```

---

## Datos

El proyecto utiliza el dataset **WeatherAUS**, que contiene variables meteorológicas históricas de distintas regiones de Australia.

En los notebooks se documenta detalladamente el proceso de limpieza, transformación de variables y entrenamiento de los modelos.

---

## Notas académicas

Trabajo práctico integrador correspondiente al curso **AA1 – TUIA**.

El foco principal está en demostrar el proceso completo de análisis de datos, modelado predictivo y despliegue a pequeña escala de un sistema de inferencia.
