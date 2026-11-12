# Mapa de categorías

Este proyecto es una página HTML estática que genera un mapa visual de categorías y relaciones entre ellas, usando la librería de visualización Graphica.js.

La aplicación representa un conjunto de nodos (categorías) con conexiones entre sí, organizados en un grafo tipo red de fuerza. Está pensado para mostrar de forma visual cómo se relacionan distintos grupos de productos, servicios o temas dentro de un catálogo.

## ¿Qué hace?

- Carga un grafo desde un bloque de datos en JavaScript.
- Muestra nodos con etiquetas visibles.
- Conecta categorías relacionadas con aristas.
- Aplica posición inicial de cada nodo para que el mapa se vea ordenado.
- Permite navegar/zoom con la vista generada por la librería.
- Tiene una estructura preparada para ser personalizada con otros datasets.

## Archivos principales

- `index.html.html` — archivo principal con la estructura HTML, estilos y datos del grafo.

## Estructura del proyecto

```text
Xadowdsgn/
├── index.html.html
├── README.md
└── .git/
```

## Cómo ejecutarlo

1. Abre el archivo `index.html.html` en tu navegador.
2. Si quieres verlo desde un servidor local, puedes usar un servidor sencillo como Python:

```bash
python -m http.server 8000
```

Luego abre en el navegador:

```text
http://localhost:8000/index.html.html
```

## Tecnologías usadas

- HTML5
- CSS
- JavaScript
- Graphica.js
- Papa Parse (cargado desde CDN)
- Mexp (cargado desde CDN)
- Google Fonts (Inter)

## Datos del grafo

El contenido principal del proyecto está dentro de un `main(function () { ... })` en JavaScript. Allí se define:

- `settings`: configuración del layout, tamaños, colores y estilo visual.
- `graph_positions`: coordenadas iniciales de cada nodo.
- `data`: listado de nodos y aristas del grafo.

Esto hace que el proyecto sea fácil de adaptar: basta con cambiar el contenido de `data` y/o `settings` para generar otra visualización.

## Personalización recomendada

Puedes modificar:

- los nombres de los nodos,
- las conexiones entre categorías,
- los colores y tamaños,
- la posición inicial de cada nodo,
- el texto de la leyenda o el título de la página.

## Nota

Este proyecto es un ejemplo de visualización de redes y está preparado como un archivo HTML autónomo, sin dependencias locales de instalación. Todo se carga desde CDN, por lo que basta con abrirlo en un navegador moderno.

## Estado del proyecto

Proyecto funcional como prototipo de visualización de categorías y relaciones.
