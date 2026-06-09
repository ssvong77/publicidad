#  Te Lo Cuento - Producción Pro 

**Te Lo Cuento - Producción Pro** es una herramienta web de código abierto diseñada para crear videos musicales y narrativos con visualizadores de audio reactivos. Permite mezclar pistas de audio, agregar fondos personalizados y exportar el resultado final en alta calidad, optimizado tanto para PC (YouTube) como para dispositivos móviles (TikTok, Instagram Reels, Shorts).

Todo el proyecto está contenido en un **único archivo HTML**, lo que lo hace extremadamente ligero, fácil de implementar y sin dependencias externas.

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)

---

## ✨ Características Principales

*   🖼️ **Fondos Dinámicos:** Soporte para imágenes y videos en bucle. El fondo se renderiza directamente en el lienzo (Canvas) en modo "contain" (sin recortes ni deformaciones).
*   🎵 **Mezcla de Audio Dual:** Carga una pista principal (voz/narración) y una música de fondo, con control de volumen independiente para la música.
*   🎨 **4 Visualizadores de Audio Reactivos:**
    *   Barras de Frecuencia (Inferior)
    *   Onda Suave (Línea única estilo neón)
    *   Círculos Concéntricos (Simétricos)
    *   Partículas Reactivas (Simétricas)
*   📱 **Multi-Formato (Responsive):** Selector de orientación para exportar en **Horizontal (16:9)** para YouTube/PC o **Vertical (9:16)** para TikTok/Reels/Shorts.
*   💾 **Exportación y Descarga Automática:** Utiliza la `MediaRecorder API` para capturar el lienzo y el audio, generando y descargando un archivo `.webm` automáticamente.
*   ️ **Tiempo Extra (Fade Out):** Opción para agregar 5, 10 o 15 segundos extra al final para que la música de fondo se desvanezca naturalmente.
*   🧠 **Renderizado Inteligente:** Los efectos visuales se desactivan automáticamente cuando termina la pista principal, dejando el fondo limpio durante el tiempo extra.

---

## 🚀 Cómo Usar

1.  **Cargar Fondos:** Selecciona una imagen o un video desde tu dispositivo para usar como fondo del lienzo.
2.  **Cargar Audios:** Sube tu **Audio Principal** (voz) y opcionalmente tu **Música de Fondo**.
3.  **Configurar:** 
    *   Ajusta el **Volumen** de la música de fondo.
    *   Selecciona la **Orientación** (Automática, Horizontal o Vertical).
    *   Elige tu **Efecto de Visualización** favorito.
    *   Define el **Tiempo Extra** al final del audio.
4.  **Exportar:** Haz clic en el botón **💾 Exportar**. 
    *   *Nota:* La reproducción y la grabación iniciarán automáticamente desde el segundo 0.
5.  **Descarga Automática:** Cuando el audio principal termine (más el tiempo extra configurado), el video se detendrá y se descargará solo en tu dispositivo.

---

## 🛠️ Tecnologías Utilizadas

*   **HTML5 Canvas API:** Para el renderizado en tiempo real del fondo y los efectos visuales.
*   **Web Audio API:** Para el análisis de frecuencias (`AnalyserNode`), mezcla de audio y control de ganancia.
*   **MediaRecorder API:** Para la captura del stream del canvas y el audio, generando el archivo de video final.
*   **Vanilla JavaScript:** Sin frameworks ni librerías externas. Código puro y optimizado.
*   **CSS3 Moderno:** Diseño responsivo, modo oscuro y efectos de *backdrop-filter*.

---

## 📂 Estructura del Proyecto

```text
te-lo-cuento-produccion-pro/
│
└── marketing.html   # Archivo único que contiene HTML, CSS y JS.
