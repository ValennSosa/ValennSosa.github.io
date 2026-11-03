# Portafolio · Valentina Sosa

Sitio personal de **Valentina Sosa**, Software Developer (SAP ABAP & BTP · full-stack SAP UI5/Fiori) e Ingeniera en Sistemas de Información (UTN FR San Francisco).

🌐 **Sitio en vivo:** [valennsosa.github.io](https://valennsosa.github.io/)

---

## Qué muestra

| Sección | Contenido |
|---|---|
| Sobre mí | Perfil profesional y formación |
| Experiencia | SAP ABAP & BTP Developer en Alan Consulting (desde marzo 2024) |
| Proyectos | Proyectos profesionales SAP (descritos de forma general por confidencialidad) y proyectos académicos con demo y código |
| Habilidades | SAP, lenguajes y desarrollo web, análisis y diseño, gestión de proyectos |
| Certificados | Cursos de Coderhouse: Ciberseguridad y Desarrollo Web, con vista previa y PDF |
| Contacto | Email (con botón para copiar) y LinkedIn |

## Características

- **Bilingüe ES / EN** con selector de idioma; el español está pre-renderizado en el HTML y el inglés se aplica con JavaScript.
- **Un solo archivo** (`index.html`) con HTML, CSS y JS, sin frameworks ni paso de build.
- **Responsive** con CSS Grid / Flexbox y breakpoints para móvil.
- **Accesibilidad:** HTML semántico, foco visible, `prefers-reduced-motion` respetado, `alt` traducible en las imágenes y `aria-pressed` en el selector de idioma.
- **SEO y redes:** `meta description`, Open Graph, URL canónica y favicon.
- Fuentes de Google Fonts (Quicksand y Karla).

## Estructura

```
ValennSosa.github.io/
├── index.html
├── README.md
└── assets/
    └── certificados/
        ├── ciberseguridad-coderhouse.pdf
        ├── ciberseguridad-coderhouse.jpg
        ├── desarrollo-web-coderhouse.pdf
        └── desarrollo-web-coderhouse.jpg
```

## Cómo editar

**Textos.** Cada elemento con `data-i="clave"` toma su texto del objeto `T` al final de `index.html`, que tiene un bloque `es` y otro `en`. Para cambiar un texto hay que editarlo en ambos idiomas y, para que el español también salga en el HTML estático, en el elemento correspondiente.

**Agregar un certificado.**

1. Copiar el PDF a `assets/certificados/` y generar una vista previa JPG (por ejemplo `pdftoppm -jpeg -scale-to-x 1000 -singlefile archivo.pdf nombre`).
2. Duplicar un `<article class="card cert">` dentro de `<section id="certificados">` y ajustar rutas y claves.
3. Agregar las claves nuevas (`certN_h`, `certN_meta`, `certN_p`, `certN_alt`, etc.) en los bloques `es` y `en` de `T`.

## Ejecutar en local

No requiere instalación. Abrir `index.html` en el navegador, o levantar un servidor estático:

```bash
python3 -m http.server 8000
# http://localhost:8000
```

## Despliegue

El sitio se publica con **GitHub Pages** desde la rama `main` (repositorio `ValennSosa.github.io`). Cada `git push` a `main` actualiza el sitio en un par de minutos.

## Proyectos enlazados

- [ServiceShop](https://github.com/ValennSosa/ServiceShop) · Python, Django, SQLite · [demo en vivo](https://valentinasosa.pythonanywhere.com/appserviceshop/)
- [EstacionamientoFacu](https://github.com/ValennSosa/EstacionamientoFacu) · Vue.js, Django, Arduino (IoT)

## Contacto

- Email: valeensoosa@gmail.com
- LinkedIn: [valentina-sosa-55b455254](https://www.linkedin.com/in/valentina-sosa-55b455254/)
- GitHub: [@ValennSosa](https://github.com/ValennSosa)

---

© 2026 Valentina Sosa · Frontera, Santa Fe, Argentina
