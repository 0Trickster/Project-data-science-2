# Project-data-science-2
Este repositorio contiene el desarrollo completo de un sistema de análisis predictivo y segmentación basado en Machine Learning para el estudio de la depresión estudiantil. El proyecto abarca desde la optimización de hiperparámetros hasta el despliegue de modelos supervisados y no supervisados.

## 📁 Estructura del Proyecto
```bash
Project-data-science-2/
│
├── data/
│   ├── processed/          # Datos limpios y transformados
│   └── raw/                # Datos originales sin procesar
│
├── notebooks/              # Ciclo de vida del modelado
│   ├── 0.0.Previous_data_analysis.ipynb
│   ├── 1.1.Hiperparams_logistic_regression.ipynb
│   ├── 1.2.Hiperparams_Random_Forest.ipynb
│   ├── 2.0.Supervised_Models_Pipeline.ipynb
│   ├── 3.0.Model_Evaluation.ipynb
│   └── 4.0.Unsupervised_Modeling.ipynb
│
├── outputs/
│   ├── models/             # Modelos entrenados (.pkl)
│   ├── params/             # Configuración de hiperparámetros óptimos (JSON)
│   ├── plots/              # Visualizaciones generadas
│   │   ├── analysis/       # Gráficos de exploración y factores de influencia
│   │   └── metrics/        # Curvas de aprendizaje, confusión y evaluación
│   └── reports/            # Resúmenes estadísticos en CSV
│
├── src/                    # Scripts de soporte (carga.py, eda_utils.py)
├── environment.yml
└── README.md

## Tecnologías utilizadas
* Python
* Pandas
* NumPy
* Matplotlib / Seaborn
* Jupyter Notebook
* SciPy
* Scikit-learn
* Conda
* Joblib (para guardar modelos)

## Flujo del proyecto
1. Carga de datos → `src/carga.py`
2. Análisis previo → `notebooks/0.0.Previous_data_analysis.ipynb`
3. Optimización de hiperparámetros:
   - Regresión Logística → `notebooks/1.1.Hiperparams_logistic_regression.ipynb`
   - Random Forest → `notebooks/1.2.Hiperparams_Random_Forest.ipynb`
4. Modelos supervisados → `notebooks/2.0.Supervised_Models_Pipeline.ipynb`
5. Evaluación de modelos → `notebooks/3.0.Model_Evaluation.ipynb`
6. Modelos no supervisados → `notebooks/4.0.Unsupervised_Modeling.ipynb`
7. Hiperparámetros → `outputs/params/`
8. Modelos entrenados → `outputs/models/`
9. Visualizaciones → `outputs/plots/`
10. Reportes finales → `outputs/reports/`

## Cómo usar el proyecto
1. Clonar el repositorio:
```bash
git clone https://github.com/0Trickster/Project-data-science-2
cd Project-data-science-2
```
2. Crear entorno
```bash
conda env create -f environment.yml
conda activate <env-name>
```
3. Ejecutar notebooks:
```bash
jupyter notebook
```

