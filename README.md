# Project12_Spam-ES
> Este es un proyecto de detección de Spam en correos enteramente en español, se utilizó el set de datos "Gabrielaz/spamspa" y el modelo y tokenizador "distilbert-base-multilingual-cased", que es un modelo que puedes entrenar en varios lenguajes como Francés, Inglés o Español. 

## Descripción
> - Es un proyecto donde detectamos spam en correos, entrenando el modelo sobre el set de datos, y a su vez comparamos 2 formas distintas de entrenamiento, usando el atributo ".train" como entrenamiento automático y "accelerate " como entrenamiento manual.  
> 
> - Se utilizó "transformers" como herramienta principal y el set de datos "Gabrielaz/spamspa" que viene de `load_dataset from datasets`.
>
> - Se comparó las métricas "Accuracy" y "F1" por ser una tarea de clasificación.
> 
> - Se hizo "fine-tuning" y tokenizamos con el modelo "distilbert-base-multilingual-cased" que está pensado para ser entrenado en diferentes idiomas incluyendo el español.
>  
> - Se entrenó a 3 épocas de entrenamiento totales.
> 
> - BatchSize de 16 datos usando "dataloader" y 8 datos en el atributo ".train".
> 
> - Trabajamos con set de Entrenamiento, Validación y Prueba.
> -------------------

## Tecnologías usadas
- Python (main)
- PyTorch
- Google Colab / Jupyter NoteBook
- Datasets (from HuggingFace)
- Transformers (from HuggingFace)
- Accelerate
- Evaluate (from HuggingFace)
- Matplotlib.pyplot
- Train (from HuggingFace)
- tqdm

## Resultados Finales
En el set de evaluación:

        Resultados del Entrenamiento Manual:
                             Accuracy: 0.989
                             F1 score: 0.989
                                 Loss: 0.002
        Resultados del Entrenamiento Automático (trainer):
                              Accuracy: 0.989
                              F1 score: 0.989
                                  Loss: 0.063
