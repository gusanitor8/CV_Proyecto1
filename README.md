# Segmentación de Imágenes de Arterias

Este repositorio contiene el código y los resultados del proyecto de segmentación de arterias en imágenes biomédicas. El enfoque principal es la binarización de las imágenes para resaltar la estructura arterial y evaluar la precisión del método utilizado; posteriormente, se discretizan para representarlas como un grafo. Este grafo permite modelar la estructura de las arterias y facilita el análisis de su conectividad y ramificaciones.

## Instalación y Requisitos

Para ejecutar el proyecto, se recomienda usar un entorno virtual y asegurarse de tener instaladas las dependencias necesarias:

```bash
python -m venv venv
source venv/bin/activate  # En Windows: venv\Scripts\activate
pip install -r requirements.txt
```


## Evaluación

Las métricas principales utilizadas son:
- **Accuracy**
- **Sensitivity (Recall)**
- **Specificity**
- **Precision**
- **F1 Score**

Los resultados obtenidos sugieren que, aunque la estructura de las arterias se detecta en la mayoría de los casos, existe una cantidad significativa de ruido. Se recomienda aplicar operaciones morfológicas adicionales como *white top-hat* y *erosion* para mejorar la calidad de la segmentación.

## Autores
Diego Leiva  
Maria Marta Ramirez  
Jose Pablo Orellana  
Gustavo González


