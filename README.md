# Tarea 3 — Redes Neuronales Multicapa (MLP)

## Requisitos

- Python 3.12
- Jupyter Notebook

## Estructura
````
.
├── datasets/                      # CSV de entrada
│   ├── postures_balanced_50000.csv
│   └── postures_imbalanced_50000.csv
├── IA_Tarea_3.ipynb                # Notebook principal
├── requirements.txt                # Dependencias de Python
├── Rúbrica_T3_IA_2026.pdf          # Rúbrica de evaluación
├── T3_IA2026-1.pdf                 # Enunciado de la tarea
├── .venv/                          # Entorno virtual
└── README
````

## Instalación

Desde la raíz del proyecto:

```bash
python -m venv .venv
source .venv/bin/activate
pip install jupyter notebook
```

Librerías principales: `pandas`, `numpy`, `matplotlib`, `scikit-learn`, `torch`, `torchvision`.

## Uso

Activar el entorno virtual e iniciar Jupyter:

```bash
source .venv/bin/activate
jupyter notebook
```

Luego:
1. Colocar `postures_balanced_50000.csv` y `postures_imbalanced_50000.csv` dentro de `datasets/`.
2. Abrir `IA_Tarea_3.ipynb` desde la interfaz de Jupyter y ejecutarlo de principio a fin.

El notebook detecta automáticamente el hardware disponible (CPU/GPU) y entrena 8 arquitecturas MLP por dataset.

## Contenido del notebook

1. **Preparación de entorno** — instalación de librerías y detección de hardware.
2. **Dataset 1 (balanceado)** — exploración, preprocesamiento (imputación por mediana + escalado estándar), definición y entrenamiento de las 8 arquitecturas (A1–A8), selección de mejores modelos, evaluación con métricas macro y matrices de confusión.
3. **Dataset 2 (desbalanceado)** — mismo flujo que el punto anterior, reutilizando las arquitecturas ya definidas.
4. **Comparación entre datasets** — contraste de los modelos finales de ambos datasets.
5. **Análisis y mejora del modelo con menor desempeño** — propuesta de ajuste de hiperparámetros y discusión de resultados.
6. **Conclusiones**.

## Declaración de uso de herramientas de IA

Se utilizaron herramientas de IA generativa para generación de plantillas de código repetitivo y revisión de errores de sintaxis. Los análisis, interpretaciones y conclusiones en celdas de texto son de autoría propia.
