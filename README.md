# Detector de Manos en Tiempo Real

Aplicación en Python que usa la cámara web para detectar hasta dos manos
en tiempo real y mostrar sus puntos de referencia (landmarks) sobre el video.

> Proyecto guiado realizado con Daxus LATAM como parte de mi formación en Python.

## Tecnologías
- Python
- OpenCV
- cvzone (HandDetector, basado en MediaPipe)

## Instalación
pip install opencv-python mediapipe cvzone

## Uso
python proyecto4.py
Se abre una ventana con la cámara. Presiona cualquier tecla para cerrar.

## Qué hace el código
- Captura video con `cv2.VideoCapture(0)` y lo redimensiona a 920x600.
- Detecta hasta 2 manos con una confianza mínima de 0.8.
- Imprime las coordenadas detectadas y dibuja las manos sobre la imagen.

## Próximas mejoras
- Contar los dedos levantados con `fingersUp()`.
- Mostrar el número en pantalla.
