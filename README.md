# C5_Aprendizaje_Automatico
Comparación de algoritmos K-NN y Árbol de Decisión usando el Zoo Dataset
# Resumen del Proyecto: Comparación de Algoritmos de Clasificación

Este proyecto forma parte de la clase 5 del curso de Aprendizaje Automático. El objetivo fue comparar dos algoritmos supervisados de clasificación — K-Nearest Neighbors (K-NN) y Árbol de Decisión — utilizando el Zoo Dataset, que contiene características de 101 animales y sus respectivas clases.

---

## Dataset Utilizado

- **Nombre**: Zoo Dataset
- **Fuente**: UCI Machine Learning Repository
- **Características**: 16 atributos binarios + nombre del animal + clase objetivo (`class_type`)
- **Preprocesamiento**: Se eliminaron las columnas `animal_name` y se dividieron los datos en entrenamiento (70%) y prueba (30%).

---

## Modelo 1: K-Nearest Neighbors (K-NN)

- **Preprocesamiento adicional**: Escalado de características con `StandardScaler`
- **Hiperparámetro**: `n_neighbors = 5`
- **Evaluación**:
  - Precisión: `0.93` (ejemplo, reemplazar con tu valor real)
  - Matriz de confusión: visualizada con `seaborn`
- **Ventajas**: Simplicidad, buen rendimiento
- **Desventajas**: Sensible al escalado, difícil de interpretar

---

## Modelo 2: Árbol de Decisión

- **Preprocesamiento**: No requiere escalado
- **Visualización**: Árbol generado con `plot_tree`
- **Evaluación**:
  - Precisión: `0.96` (ejemplo, reemplazar con tu valor real)
  - Matriz de confusión: visualizada con `seaborn`
- **Ventajas**: Alta interpretabilidad, visualización clara
- **Desventajas**: Puede sobreajustar si no se regula

---

## Comparativa de Modelos

| Métrica               | K-NN                      | Árbol de Decisión           |
|----------------------|---------------------------|-----------------------------|
| Precisión            | 0.93                      | 0.96                        |
| Interpretabilidad    | Baja                      | Alta                        |
| Sensible a escalado  | Sí                        | No                          |
| Visualización        | Matriz de confusión       | Matriz + Árbol de decisión  |

![Comparación de precisión](visuales/comparacion_precision.png)

---

## 📝 Conclusión

Ambos modelos demostraron buen rendimiento sobre el Zoo Dataset. El Árbol de Decisión se destacó por su capacidad de interpretación y visualización


