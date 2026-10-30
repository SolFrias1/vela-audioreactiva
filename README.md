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

El proyecto explora la **fragilidad, el calor y la transformación** a través de la metáfora visual de una vela, o pelea, que se consume, respondiendo orgánicamente a la canción chilena ***Piedad*** de **Camila Moreno** (*álbum Mala madre, 2:57 min*).

* **Respuesta Audioreactiva:** Ondas de calor (*heat shimmer*) y distorsión líquida de la cera que se licúa al ritmo de la voz y los pulsos de percusión.
* **Golpes de Beat:** Aberración cromática sutil (*RGB channel split*) y chispas doradas que emergen del núcleo de la llama con cada golpe de bombo.
* **Clímax y Palabra «PIEDAD»:** Sincronizada milimétricamente con el momento exacto en que la voz canta el verso (*segundos 25.8 y 172.3*), proyectándose en tipografía monumental y traslúcida que se disuelve en el humo.
* **Extinción Poética:** Hacia el final de la canción, la vela colapsa, la llama titila hasta apagarse y la escena transiciona gradualmente hacia cenizas y escala de grises.

* **¿Qué relación se propone y por qué?
*Se propone una relación de traducción sinestésica y transcodificación material. En lugar de utilizar la imagen como un mero acompañamiento ilustrativo de la música, el sonido se conceptualiza como una fuerza termodinámica y gravitacional que altera físicamente la materia visible en tiempo real.

*La obra Piedad de Camila Moreno transita en una tensión constante entre la intimidad confesional de la voz y el desgarro tribal de su percusión. Frente a esto, la vela actúa como una metáfora de consunción y vulnerabilidad: un cuerpo orgánico que arde, respira, sangra cera y finalmente se extingue. La música se convierte en el calor que licúa el cuerpo y en el viento que perturba su llama.

* **¿Cómo funcionan los cambios y perillas en la plataforma?
La plataforma está diseñada no como un reproductor estático, sino como un sintetizador visual interactivo. Cada perilla modula la física del entorno:

*Sensibilidad de Beat / Profundidad de Derretimiento: Controlan el umbral elástico y la viscosidad de la cera (cuánta masa se desplaza ante cada golpe).
*Calor y Aberración Cromática: Modulan la temperatura óptica del aire (distorsión ondulatoria y separación de canales RGB simulando una lente sobrecalentada).
*Tiempo de Extinción: Permite coreografiar el destino fatal de la vela, determinando cuándo la llama colapsa en humo y el color transiciona a la ceniza.
*Modos de Visualización: El botón 📱 Marco 9:16 / ⛶ Full Pantalla permite alternar entre el encuadre cerrado para dispositivos móviles (donde la vela es protagonista absoluta) y una experiencia inmersiva atmosférica con márgenes oscuros y letras flotantes.

##¿Qué parámetros del sonido se modifican/analizan y por qué esos?
* **A través de la Web Audio API y un analizador FFT (Fast Fourier Transform), se descompone la señal en bandas específicas:

* **Graves y Bombo (~40Hz – 200Hz):
*Por qué: El registro grave posee impacto físico y peso corporal. En la canción, los golpes de percusión marcan el pulso vital; por eso gobiernan el desplazamiento vertical de la cera (derretimiento) y la aberración cromática.
* **Frecuencias Medias / Registro Vocal (~340Hz – 2000Hz):
*Por qué: Es la zona tonal donde habita la voz de Camila Moreno. Mapear este rango a las ondas de calor (heat shimmer) hace que la refracción del aire alrededor de la llama literalmente "hable" al ritmo del canto.
* **Agudos (~2100Hz – 6800Hz):
*Por qué: Aportan brillo y fragilidad. Modulan la velocidad de ascenso y el titileo sutil de las partículas flotantes.
* **Detección Dinámica de Transitorios (Beat Flux):
*Por qué: Permite detectar el ataque percusivo instantáneo, logrando una respuesta sin latencia perceptible que amarra la pulsación de la palabra «PIEDAD» al compás exacto.

##¿Qué se descubre durante el proceso y la interacción?
* **La materialización del tiempo sonoro: La música deja de ser un fenómeno abstracto e invisible que transcurre en el tiempo; en la pantalla, la música adquiere volumen, masa y viscosidad. Ver cómo la voz calienta la imagen y cómo el bombo derrite la cera produce una percepción única del sonido.
* **La sublimación de la palabra: La palabra «PIEDAD» no se percibe leyendo letras, sino como un pulso lumínico que explota y se encoge. Se descubre que la tipografía en nuevos medios puede funcionar como luz 
* **El usuario como co-creador performativo: La interactividad rompe la unidireccionalidad del videoclip tradicional. El usuario ya no solo "consume" la canción: define qué tan violento es el derretimiento, qué tan abrasivo es el calor o cuándo precipitar la extinción de la vela.
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
