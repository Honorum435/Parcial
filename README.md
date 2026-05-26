# Kimetsu no Yaiba - El Castillo Infinito (Sitio web)

Sitio web estático sobre la película **Kimetsu no Yaiba: El Castillo Infinito**, desarrollado como recuperación del Primer Parcial.

## Estructura del proyecto

```
.
├── index.html               # Página de inicio (landing con tráiler)
├── 404.html                 # Página de error (la usa Vercel automáticamente)
├── img/                     # Imágenes
├── css/
│   ├── base.css             # Estructura y elementos generales (compartido)
│   ├── index.css            # Estilos específicos por página
│   ├── characters.css
│   ├── reparto.css
│   ├── produccion.css
│   ├── curiosidades.css
│   ├── sobre-la-pelicula.css
│   ├── contacto.css
│   ├── confirmacion.css
│   └── error.css
└── pages/
    ├── sobre-la-pelicula.html   # Incluye reproductor de audio
    ├── characters.html          # Layout en grid
    ├── reparto.html
    ├── produccion.html
    ├── curiosidades.html
    ├── contacto.html            # Formulario con validaciones
    └── confirmacion.html        # Confirmación del envío
```

## Características

- **CSS modular**: un `base.css` con la estructura y elementos generales, y un CSS por página con selectores específicos. Se eliminó código repetido usando combinaciones de clases (`.card`, `.card--accent`, `.boxed`, `.boxed--bordered`, `.btn`, `.btn--solid`).
- **Favicon y navegación** en todas las páginas.
- **Página de error 404** con la misma estética y enlace al inicio.
- **Animaciones y transiciones** (fade-in, hover, latido) con respeto a `prefers-reduced-motion`.
- **Formulario de contacto** (nombre, apellido, correo, mensaje) con labels, inputs específicos y validaciones HTML. Redirige a una página de confirmación.
- **Reproductor de la banda sonora** (iframe de YouTube) en la sección "Sobre la Película".
- **Layout con grid y flex** en columnas (personajes, reparto, ficha técnica).
- **Responsive** para celulares.

## Cómo verlo localmente

Abrí `index.html` en el navegador, o serví la carpeta con cualquier servidor estático.

## Despliegue

Desplegado en Vercel como sitio estático.
