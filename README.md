📊 Infografía Interactiva: Aprendizaje Digital en Educación Médica
Infografía web de tipo "lista" (Top 5) construida exclusivamente con HTML y CSS puro (cero JavaScript). Presenta los hallazgos principales del artículo de investigación de Kulkarni et al. (2025) sobre la plataforma Osmosis en educación médica, transformando viñetas tradicionales en iconos interactivos con animaciones avanzadas.

HTML5CSS3Sin JS

✨ Características Principales
Efecto de Icono Circular (Semicírculos): Al pasar el cursor, dos arcos de colores separados rotan y se unen formando un anillo completo alrededor del emoji.
Línea Ondulada Animada: Aparece debajo de cada título al hacer hover y fluye continuamente usando un patrón SVG en data URI.
Microinteracciones en Tarjetas: Elevación con sombra dinámica, cambio de color en textos y escala en el badge numérico.
Timeline Visual: Una línea vertical punteada conecta los cinco elementos de la lista.
100% Responsivo: Adaptado con tres breakpoints específicos para escritorio, tablet y móviles pequeños.
Accesible: Respeta la preferencia prefers-reduced-motion: reduce desactivando animaciones para usuarios sensibles al movimiento.
🚀 Cómo utilizar
No requiere instalación de dependencias, servidores ni procesos de compilación.

Clona o descarga este repositorio.
Abre el archivo index.html en cualquier navegador moderno.
Pasa el cursor sobre las tarjetas para ver las animaciones.
🗂 Estructura del Proyecto
├── index.html       # Archivo único (contiene HTML结构与 estilos CSS embebidos)└── README.md        # Documentación del proyecto
🎨 Paleta de Colores
La identidad visual está basada en 3 colores principales, definidos como variables CSS (:root):

Color
Código Hex
Uso Principal
Azul Oscuro	#1F3C88	Header, footer, títulos, semicírculo inferior
Teal	#00A8A8	Acentos, semicírculo superior, línea ondulada
Gris Claro	#F2F4F8	Fondo del body, relleno de los iconos

⚙️ Guía de Personalización (CSS)
El archivo CSS contiene comentarios detallados explicando cada animación. Aquí un resumen rápido de qué modificar y dónde:

1. Anillo de Semicírculos
Ubicación: Clase .icon-ring y sus pseudo-elementos ::before / ::after

Tamaño del gap inicial: Modifica transform: rotate(-35deg) y rotate(35deg). (Ej: -50deg/50deg para un gap más grande).
Grosor del anillo: Cambia border: 3px solid.
Distancia del icono: Modifica inset: -5px (Ej: -8px para alejarlo más).
Velocidad de cierre: Cambia transition-duration: 0.5s.
Colores: Cambia var(--teal) en ::before y var(--azul) en ::after.
2. Línea Ondulada
Ubicación: Clase .item-title::after y @keyframes wave-scroll

Amplitud de la onda: Edita los valores Y en la ruta del SVG (Q6 0 12 4 Q18 8 24 4).
Velocidad de flujo: Cambia animation-duration: 1.3s.
Dirección: Cambia el valor to en @keyframes a -24px 0 para fluir a la izquierda.
Detener el flujo: Elimina la propiedad animation en el estado :hover para que solo se dibuje estática.
📱 Responsive Design
La infografía se adapta mediante tres media queries:

Dispositivo
Breakpoint
Ajustes Principales
Escritorio / Tablet	> 640px	Diseño base completo. Iconos de 68px.
Tablets pequeñas	≤ 640px	Iconos de 56px, tipografía reducida, timeline movida.
Móviles estrechos	≤ 400px	Iconos de 48px, padding compacto, onda de 18px de ciclo.

♿ Accesibilidad
Se implementa @media (prefers-reduced-motion: reduce) para anular todas las transiciones y animaciones (transition: none, animation: none).
Etiquetas semánticas correctas (<header>, <main>, <section>, <article>, <footer>).
Atributos aria-hidden="true" en elementos puramente decorativos.
Atributo aria-label en la sección de la lista.
📄 Fuente Académica
Este contenido está basado en el siguiente artículo de investigación de acceso abierto:

Kulkarni, S., Lawson-Smith, E., Mongan, L., Westacott, R., & Jackson, D. (2025). Exploring student perceptions of the Osmosis digital learning platform in undergraduate medical education and its influences on motivation and inclusivity. BMC Medical Education, 25, 1041.

🔗 DOI: 10.1186/s12909-025-07591-z
📜 Licencia del artículo: Creative Commons Attribution 4.0 International (CC BY 4.0)

👤 Créditos de Diseño y Desarrollo
Diseñador y Desarrollador Front-end: Nikoll Yauri Mendoza (Reemplazar con enlace real si aplica)
Tipografía utilizada: Plus Jakarta Sans (Google Fonts)
Tecnologías: HTML5 Puro, CSS3 Puro (Flexbox, Clip-path, Data URI SVG, Keyframes).
📜 Licencia
Este proyecto de infografía se distribuye bajo los términos de la licencia Creative Commons Attribution 4.0 International (CC BY 4.0), en coherencia con la publicación científica original. Eres libre de compartir y adaptar este material con los debidos créditos.
```



