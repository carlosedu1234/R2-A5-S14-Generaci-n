# R2-A5-S14: Generación de Imágenes con DCGAN y Stable Diffusion

Repositorio de la actividad práctica sobre modelos generativos en Deep Learning, implementando una Red Generativa Adversaria (DCGAN) y fine-tuning de Stable Diffusion con LoRA.

## 📂 Contenido
*   **`DCGAN_LFW.ipynb`**: Entrenamiento de una DCGAN para generar rostros (dataset LFW).
*   **`StableDiffusion_LoRA.ipynb`**: Fine-tuning de Stable Diffusion v1.5 usando LoRA.
*   **`R2-A5-S14 Generación.pdf`**: Informe con análisis, resultados y conclusiones.

## 🛠️ Tecnologías
*   Python / PyTorch
*   Hugging Face (`diffusers`, `transformers`, `peft`)
*   Google Colab (GPU T4)

## 📊 Resultados Principales

**1. DCGAN (Rostros)**
El Discriminador dominó el entrenamiento (pérdida estable), mientras que el Generador mostró alta volatilidad. Se lograron rostros sintéticos con estructuras básicas pero borrosos debido a la resolución (64x64) y las limitaciones de cómputo.

**2. Stable Diffusion + LoRA**
Se entrenó solo el **0.0927%** de los parámetros del modelo. La pérdida MSE descendió correctamente, generando una abstracción geométrica. Esto demuestra que LoRA permite adaptar modelos masivos en hardware de consumo.

*Universidad de Cundinamarca - Especialización en Inteligencia Artificial*
