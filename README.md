# Programación Genética desde Cero para Regresión Simbólica

## Descripción
Implementación completa de un motor de Programación Genética (GP) desde cero, siguiendo los lineamientos de "A Field Guide to Genetic Programming". Permite realizar regresión simbólica en 6 datasets clásicos.

## Ejecución Rápida

### 1. Instalación
```bash
pip install -r requirements.txt
```

### 2. Ejecutar un dataset específico
```bash
python experimento_completo.py --dataset concrete --runs 3
```

### 3. Ejecutar todos los datasets
```bash
python ejecutar_todos_datasets.py
````

### 4. Comparar con gplearn
```bash
python gplearn_comparison.py
````
## Estructura del proyecto
```bash
gp_from_scratch/
├── config.py                 # Hiperparámetros
├── nodo.py                   # Estructura de árbol
├── generador_arboles.py      # Ramped Half-and-Half
├── evaluador.py              # Evaluación y fitness
├── operadores_gp.py          # Selección, cruce, mutación
├── poblacion.py              # Evolución de población
├── analisis_bloat.py         # Análisis de crecimiento
├── visualizacion.py          # Gráficas y visualización
├── gplearn_comparison.py     # Comparativa con gplearn
├── experimento_completo.py   # Pipeline completo
├── ejecutar_todos_datasets.py # Experimentos en 6 datasets
├── main.py                   # Punto de entrada simple
└── datos/                    # Carpeta para datasets
    ├── concrete.csv
    ├── tower.csv
    ├── yacht.csv
    ├── housing.csv
    ├── energy_cooling.csv
    └── energy_heating.csv
```


## Cómo Ejecutar TODO el Proyecto PASO a PASO:

```bash
# 1. Crear estructura de carpetas
mkdir gp_from_scratch
cd gp_from_scratch
mkdir datos

# 2. Crear todos los archivos Python listados arriba

# 3. Instalar dependencias
pip install numpy pandas scikit-learn matplotlib seaborn gplearn networkx

# 4. ¡Ejecutar el experimento completo!
python experimento_completo.py --dataset concrete --runs 3

# 5. Ejecutar en todos los datasets
python ejecutar_todos_datasets.py
