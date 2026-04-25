# BYTEC — Introducción al Diseño Web

## Sobre la academia

- La academia se llama **BYTEC**
- Estilo visual: **espacio y pixel** (fuentes pixeladas, estrellas animadas en canvas, tema oscuro)
- Colores principales: naranja `#f75001` y azul `#04589d`
- Fuentes: Press Start 2P (pixel), Orbitron (headings), Space Mono (body/code)

## Sobre el curso

- **8 clases** de **1 hora y media** (90 minutos) cada una
- Se ve **solo HTML y CSS**, nada de JavaScript ni otros lenguajes
- El público es principiante absoluto (no saben nada de programación)
- Lenguaje: español argentino (vos, usá, poné, etc.)
- Comentarios y texto en código en **inglés**

## Estructura del proyecto

```
/
├── index.html          ← Portal principal (landing con links a cada clase)
├── style.css           ← Estilos del portal
├── clase-1/            ← Cada clase tiene su propia carpeta
│   ├── index.html      ← Presentación estilo PPT (slides navegables)
│   ├── style.css       ← Estilos de la presentación
│   └── ejercicios/     ← Ejercicios prácticos para los alumnos
│       ├── 01-*.html
│       ├── 01-style.css (si corresponde)
│       ├── 02-*.html
│       └── ...
├── clase-2/
│   └── (misma estructura)
└── clase-N/
    └── (misma estructura)
```

## Programa de clases

| # | Título | Contenido | Estado |
|---|--------|-----------|--------|
| 01 | ¿Cómo Funciona la Web? | Navegador, semántico vs sintáctico, qué es HTML, IDE (VS Code) | Creada |
| 02 | Interactividad & CSS | Formularios (form, label, input, select, button), sintaxis CSS, selectores | Creada |
| 03 | El Modelo de Caja | Box Model (content, padding, border, margin), box-sizing, display block/inline/inline-block | Creada |
| 04 | Layout con Flexbox | Alinear, distribuir y ordenar elementos con flexbox | Creada |
| 05 | Diseño Responsive | Media queries, mobile first | Creada |
| 06 | Tipografía, Colores & Diseño Visual | Google Fonts, paletas, imágenes, fondos | Creada |
| 07 | Proyecto Final: Maquetación | Sitio web completo desde cero | Pendiente |
| 08 | Pulido Final & Publicación | Animaciones CSS, deploy en GitHub Pages | Pendiente |

## Contenido de la Clase 1

- Cómo funciona un navegador (cliente-servidor, request/response)
- Anatomía de una URL
- Semántico vs sintáctico (significado vs forma de escritura)
- Qué es HTML (HyperText Markup Language, no es lenguaje de programación)
- Estructura base: DOCTYPE, html, head, body
- Etiquetas: h1-h6, p, br, hr, ul, ol, li, strong, em, a, img
- Qué es un IDE, por qué usar VS Code
- Truco Emmet (! + Tab)

## Formato de las presentaciones (slides)

- Cada clase es una página HTML con slides navegables
- Navegación: flechas del teclado, botones en la nav bar, swipe touch en celulares
- Primera vez en mobile: aparece un toast "¡Deslizá para navegar!" (se guarda en localStorage)
- El logo "BYTEC" en la nav bar es un link que vuelve al portal principal
- Cada slide tiene la clase `.slide` y se activa con `.active`
- Fondo: canvas con estrellas animadas parpadeantes
- Responsive: breakpoints en 768px y 380px
- Cada presentación incluye: portada, objetivo, repaso de la clase anterior, teoría, prácticas guiadas, ejercicios y tarea semanal

## Formato de los ejercicios

- 4 ejercicios por clase, con dificultad progresiva: Fácil, Fácil/Medio, Medio, Desafío
- Los primeros ejercicios son guiados (con "TU-VALOR" o "TU-CODIGO" como placeholders)
- Los últimos son más libres para fomentar investigación
- Cada ejercicio tiene instrucciones detalladas en comentarios HTML
- Los CSS de ejercicios guiados tienen comentarios explicando qué completar

## Portal principal (index.html raíz)

- Muestra las 8 clases como tarjetas (cards)
- Clases disponibles: clase `available` + badge "DISPONIBLE" + link a la carpeta
- Clases pendientes: clase `locked` + badge "PRÓXIMAMENTE" + href="#"
- Cuando se crea una nueva clase, actualizar el portal: cambiar `locked` → `available`, `href="#"` → `href="clase-N/index.html"`, y el badge a "DISPONIBLE"
- Fondo con estrellas + estrellas fugaces naranjas

## Reglas generales

- Siempre responder en **español**
- Comentarios y texto dentro del código en **inglés**
- Mantener el estilo visual consistente entre clases (mismos colores, fuentes, componentes)
- Todo debe ser responsive y funcionar en celulares
- Incluir teoría, ejemplos de código, prácticas guiadas y ejercicios para resolver en cada clase
- Hacer el contenido práctico y orientado a que el alumno codee
