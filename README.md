# Monitoreo_Satelital_Malinche


##  Descripción del Proyecto
Este proyecto aplica técnicas de **Teledetección** y **Ciencia de Datos** para analizar la salud de la vegetación en el Parque Nacional La Malinche y sus alrededores (Valle de Puebla-Tlaxcala). Utilizando imágenes multiespectrales del satélite **Sentinel-2** (Agencia Espacial Europea), se calculó el Índice de Vegetación de Diferencia Normalizada (NDVI) para diagnosticar el estrés hídrico durante la temporada seca (Enero 2026).

## Metodología Matemática
El núcleo del análisis se basa en la respuesta espectral de la clorofila. Se procesaron las bandas **B04 (Rojo visible)** y **B08 (Infrarrojo Cercano - NIR)** utilizando álgebra de matrices en Python para aplicar la fórmula del NDVI:

$$NDVI = \frac{NIR - RED}{NIR + RED}$$

* **NDVI > 0.5:** Indica vegetación densa y saludable (Bosque de coníferas).
* **NDVI < 0.2:** Indica suelo desnudo, roca o zonas urbanas.

##  Resultados Clave (Enero 2026)
El procesamiento de más de 120 millones de píxeles reveló la fenología invernal de la región:
* **75.9%** del territorio analizado se encuentra en estado de latencia o es suelo desnudo (agricultura de temporal).
* **0.5%** representa el núcleo de bosque denso residente, destacando la alta fragmentación del ecosistema.
* **Hallazgo Geológico:** La vegetación saludable en invierno se refugia casi exclusivamente en las barrancas y cañadas del volcán, que actúan como microclimas húmedos.

##  Tecnologías Utilizadas
* **Python 3.9+**
* **Rasterio:** Manipulación de datos geoespaciales matriciales.
* **NumPy:** Cálculo matricial de alto rendimiento.
* **Matplotlib:** Visualización de datos y generación de mapas de calor.

##  Cómo usar este proyecto
1. Clonar el repositorio.
2. Instalar dependencias: `pip install rasterio numpy matplotlib`
3. Descargar una imagen L2A de Sentinel-2 y colocar la carpeta `.SAFE` en el directorio.
4. Ejecutar el Jupyter Notebook.


---
Autora: Anahí Juárez Ramírez | Lic en Matemáticas

