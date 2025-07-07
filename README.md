# Clasificación de Células Cancerígenas IDC en Imágenes Histológicas

## Objetivo del trabajo

Este proyecto tiene como finalidad aplicar técnicas de procesamiento de imágenes clásicas y modernas para la **detección automática de células cancerígenas** en imágenes histológicas de tejido mamario. Se comparan dos enfoques:

- Un modelo basado en **técnicas clásicas** de visión por computador (histogramas + SVM).
- Un modelo basado en **redes neuronales convolucionales (CNN)** con interpretabilidad mediante **Class Activation Maps (CAMs)**.

El objetivo es evaluar el rendimiento de ambos métodos y visualizar las regiones de las imágenes que más influyen en la predicción, facilitando así una interpretación médica de los resultados.

---

##Nombre de los alumnos participantes

- Jorge Chipoco  
- [Agrega aquí otros nombres si hay más integrantes]

---

## Breve descripción del dataset

Se utilizó el conjunto de datos **Breast Histopathology Images (IDC)**, disponible en [Kaggle](https://www.kaggle.com/datasets/paultimothymooney/breast-histopathology-images), que contiene más de 270,000 imágenes microscópicas de tejido mamario, cada una con resolución 50×50 píxeles y etiquetadas como:

- `0`: No cancerígena
- `1`: Cancerígena (Invasive Ductal Carcinoma - IDC)

> 📎 Puedes encontrar más detalles técnicos en el archivo `IDC_dataset_description.pdf` incluido en este repositorio.

---

## Conclusiones

- El modelo **clásico (SVM)** logró un rendimiento aceptable (~80% accuracy), pero mostró limitaciones en la detección de imágenes cancerígenas (recall ~65%).
- La **CNN** alcanzó un desempeño significativamente superior (~88–90% accuracy), con mejor precisión y recall para la clase cancerígena.
- El uso de **Class Activation Maps (CAM)** permitió interpretar visualmente las decisiones del modelo profundo, destacando las zonas más relevantes de cada imagen.
- La automatización de este tipo de clasificación puede servir como herramienta de apoyo para patólogos en diagnósticos médicos, especialmente en regiones con pocos recursos.

---

## Licencia

Este proyecto es de carácter educativo y se encuentra bajo la licencia **MIT**. Puedes modificar, distribuir y reutilizar el código con fines académicos citando a los autores.

---

