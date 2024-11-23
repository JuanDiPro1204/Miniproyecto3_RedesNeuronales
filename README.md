# 🌟 **MiniProyecto 3 - Generación de Imágenes Sintéticas a Partir de Mamografías Usando Pix2Pix** 🌟

## 📑 **Descripción**
Este proyecto utiliza Redes Generativas Antagónicas (GANs) para mejorar la calidad de las mamografías. Las GANs permiten generar imágenes de alta calidad a partir de imágenes de baja calidad, contribuyendo al diagnóstico temprano del cáncer de mama al reducir el ruido, mejorar la resolución y destacar las características clínicas esenciales.

🔗 **Notebook del proyecto:**  
El cuaderno de colab en el que se realizó todo el entrenamiento y validación del funcionamiento de la red de encuentra en el archivo llamado Miniproyecto3_Redes.ipynb
---

## 🧠 **Resumen**
El proyecto propone el uso de **Pix2Pix**, un modelo basado en GANs, para:
- Mejorar la calidad visual de imágenes mamográficas.
- Facilitar el diagnóstico clínico mediante imágenes más nítidas y libres de ruido.
- Proveer una alternativa de bajo costo frente a equipos de imágenes avanzados.

---

## 📚 **Marco Teórico**
1. **Redes Neuronales Artificiales (RNA):** Inspiradas en el cerebro humano, útiles en clasificación y generación de imágenes.
2. **GANs (Generative Adversarial Networks):**  
   - Dos redes en competencia: Generador y Discriminador.  
   - Aplicadas para mejorar imágenes médicas, como mamografías.
3. **Técnicas de preprocesamiento:**  
   - Normalización y aumento de datos para superar la limitación de conjuntos de datos médicos.

---

## 🔍 **Metodología**
1. **Preprocesamiento:**  
   - Normalización de imágenes.  
   - Aumento de datos (rotaciones, cambios de brillo, etc.).  

2. **Diseño del modelo GAN:**  
   - Generador: Se crea la red que produce imágenes mejoradas.  
   - Discriminador: Distingue entre imágenes reales y generadas u artificiales, esto con el fin de evaluar la calidad de la generación de las imágenes.

3. **Entrenamiento:**  
   - Métricas utilizadas:  
     - **MSE** (Error Cuadrático Medio).  
     - **PSNR** (Relación Señal-Ruido de Pico).  
     - **SSIM** (Índice de Similitud Estructural).  

4. **Evaluación:**  
   - Comparación cualitativa y cuantitativa de las imágenes generadas frente a las originales.

---

## 🌟 **Resultados**
📈 **Curvas de entrenamiento:**  
El modelo mostró un entrenamiento balanceado entre el generador y el discriminador, logrando una generación estable de imágenes.

📷 **Imágenes generadas:**  
- Las imágenes generadas presentan una notable mejora en resolución y reducción de ruido.  
- Similitud visual elevada con las imágenes originales de alta calidad (Ground Truth).

**Ejemplos visuales:**
| **Input**  | **Ground Truth**  | **Predicted**  |
|------------|-------------------|----------------|
| ![Input](input_example.jpg) | ![GT](ground_truth.jpg) | ![Predicted](predicted_example.jpg) |

---

🎉 **Gracias por explorar este proyecto!**  

