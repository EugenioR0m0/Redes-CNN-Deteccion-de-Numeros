# Redes-CNN-Deteccion-de-Numeros

Este repositorio contiene un sistema completo de clasificación de dígitos manuscritos utilizando Redes Neuronales Convolucionales (CNN). Incluye el entrenamiento de múltiples arquitecturas, la selección del mejor modelo y un sistema de OCR en tiempo real basado en cámara.

---

## Contenido del Repositorio

### 1. Modelo Final (`vgg_final_model_2.keras`)
Modelo VGG mejorado entrenado con imágenes preprocesadas (grayscale, resize 280×280, Otsu, invertir y normalizar).  
Este modelo obtuvo el mejor rendimiento entre todas las arquitecturas evaluadas.

### 2. Script de OCR en Tiempo Real (`ocr_realtime.py`)
Programa que:
- Abre la cámara
- Detecta posibles dígitos mediante contornos
- Preprocesa cada región exactamente igual que en el entrenamiento
- Clasifica en tiempo real usando el modelo final
- Muestra la imagen original y la imagen preprocesada

### 3. Comparación de Modelos (`Modelos_Comparados.html`)
Archivo HTML con:
- Implementación de todas las arquitecturas evaluadas  
- Baseline CNN  
- VGG Mejorado  
- ResNet simplificado  
- Inception simplificado  
- MobileNet lite  
- CNN con Data Augmentation  
- Gráficas de accuracy/loss  
- Evaluación final y conclusiones

---

## Instalación

Clonar el repositorio:
```bash
git clone https://github.com/tu-usuario/tu-repo.git
cd tu-repo
