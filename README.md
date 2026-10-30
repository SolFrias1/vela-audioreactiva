# Crisol Audioreactivo — Piedad (Camila Moreno)
> **Ejercicio 05** — Proyecto de Programación Interactiva (PPI)  
> **Estudiante:** Victoria Sol Frías  
> **Escuela de Diseño — Universidad Diego Portales (UDP)**  
> **Formato:** Reel vertical 9:16  

---

## 🌟 Demo Interactiva en Vivo

👉 **[Probar la plataforma en GitHub Pages](https://TU-USUARIO.github.io/vela-audioreactiva)**  
*(No requiere instalación; se ejecuta directamente en el navegador con soporte para WebGL y Web Audio API)*.

---

## 🕯️ Concepto y Dirección de Arte

El proyecto explora la **fragilidad, el calor y la transformación** a través de la metáfora visual de una vela que se consume, respondiendo orgánicamente a la canción chilena ***Piedad*** de **Camila Moreno** (*álbum Mala madre, 2:57 min*).

* **Respuesta Audioreactiva:** Ondas de calor (*heat shimmer*) y distorsión líquida de la cera que se licúa al ritmo de la voz y los pulsos de percusión.
* **Golpes de Beat:** Aberración cromática sutil (*RGB channel split*) y chispas doradas que emergen del núcleo de la llama con cada golpe de bombo.
* **Clímax y Palabra «PIEDAD»:** Sincronizada milimétricamente con el momento exacto en que la voz canta el verso (*segundos 25.8 y 172.3*), proyectándose en tipografía monumental y traslúcida que se disuelve en el humo.
* **Extinción Poética:** Hacia el final de la canción, la vela colapsa, la llama titila hasta apagarse y la escena transiciona gradualmente hacia cenizas y escala de grises.

---

## 🛠️ Tecnologías y Arquitectura

* **WebGL (GLSL Shaders):** Deformación de malla por ruido fractal (*Value Noise*), simulación de calor convectivo y composición cromática en tiempo real.
* **Web Audio API:** Análisis FFT espectral por bandas de frecuencia (graves, medios y agudos) y detección dinámica de transitorios (*Flux*).
* **HTML5 Canvas 2D:** Sistema de partículas de ceniza/chispas y renderizado tipográfico tipográfico (*Cinzel*).
* **Grabadora de Video Integrada:** Grabación en tiempo real a **60 FPS** en formato nativo **MP4** con audio integrado para exportación directa a Reels / TikTok.
* **Soporte Multi-Fuente:** Capacidad de arrastrar cualquier video (.mp4, .mov) o canción (.mp3, .wav) para reaccionar a nuevos contenidos.

---

## 📂 Estructura del Repositorio

```text
vela-audioreactiva/
├── index.html           # Aplicación web interactiva completa (WebGL + Canvas + Audio)
├── song_b64.js          # Canción "Piedad" precargada en memoria (Base64 Blob)
├── candle_b64.js        # Textura inicial de vela en memoria (Base64)
├── cancion_piedad.mp3   # Archivo de audio original
├── frame_20s.jpg        # Fotograma de vista previa
├── README.md            # Documentación del proyecto
└── .gitignore           # Exclusión de archivos binarios pesados (>100MB)
```

---

## 🚀 Cómo ejecutar localmente

1. Clona este repositorio o descarga el archivo `.zip`:
   ```bash
   git clone https://github.com/TU-USUARIO/vela-audioreactiva.git
   ```
2. Entra a la carpeta y abre `index.html` con cualquier navegador moderno (Google Chrome, Safari, Firefox o Edge).
3. Haz clic en **Reproducir** para iniciar la experiencia interactiva.

---

## 📹 Video del Proceso y Entrega Final

* **Video Completo 4K (2:57 min):** Disponible en la sección de [Releases de este repositorio](https://github.com/TU-USUARIO/vela-audioreactiva/releases) o en el archivo de entrega.
