# practica-pixel-perfect

# Práctica: Maquetación Pixel Perfect — Página de Disney

Actividad de final de corte de la materia **Desarrollo de Aplicaciones Web I**. El objetivo es maquetar la página principal de Disney a partir de una imagen de diseño, lo más idéntica posible (_pixel perfect_), usando solo **HTML y CSS** y trabajando **en pareja con Git y GitHub**.

> Sitio construido únicamente con fines educativos.

**Integrantes:**

- Juan David Tello — navbar, banner, shop y Disney+
- Juan Arias — movies, parks and travel, more y footer

---

## 1. Estructura de carpetas

```
practica-pixel-perfect/
├── css/
│   └── styles.css      → estilos de toda la página
├── img/                → imágenes del diseño
├── index.html          → estructura de la página
├── APRENDIZAJES.md     → aprendizajes y dificultades de cada integrante
└── README.md           → esta documentación
```

## 2. Estructura HTML

```html
<body>
  <nav class="navbar">…</nav>
  <section class="banner">…</section>
  <main>
    <section id="shop">…</section>
    <section id="disney-plus">…</section>
    <section id="movies">…</section>
    <section id="parks-and-travel">…</section>
    <section id="more">…</section>
  </main>
  <footer>…</footer>
</body>
```

### Etiquetas semánticas usadas

- `<nav>`: navegación principal (logo, menú, login y buscador).
- `<section>`: agrupa cada bloque temático de la página.
- `<main>`: el contenido principal.
- `<article>`: cada tarjeta, porque es contenido independiente que se puede reutilizar.
- `<footer>`: enlaces secundarios y avisos legales.
- Todas las imágenes tienen un `alt` descriptivo para la accesibilidad.

## 3. Metodología BEM

Las clases siguen **BEM** (_Block, Element, Modifier_):

| Tipo        | Sintaxis                        | Ejemplos                                             |
| ----------- | ------------------------------- | ---------------------------------------------------- |
| Bloque      | `bloque`                        | `navbar`, `banner`, `shop-card`, `plus-card`         |
| Elemento    | `bloque__elemento`              | `navbar__link`, `banner__title`, `shop-card__image`  |
| Modificador | `bloque__elemento--modificador` | `banner__button--primary`, `banner__button--outline` |

## 4. Propiedades CSS principales

- **`box-sizing: border-box`** (reset global): el padding y el borde se cuentan dentro del tamaño del elemento.
- **Flexbox** (`display: flex`, `justify-content`, `align-items`, `gap`): navbar, contenido del banner y botones.
- **CSS Grid** (`grid-template-columns: repeat(4, 1fr)`): grillas de tarjetas del shop y de Disney+.
- **`background-image`, `background-size: cover`, `background-position: center`**: fondo del banner.
- **`aspect-ratio` + `object-fit: cover`**: imágenes del mismo tamaño sin deformarlas.
- **`flex: 1`** en el cuerpo de la tarjeta: todas las tarjetas de una fila quedan del mismo alto.
- **Font Awesome (CDN)**: ícono de la lupa en el buscador.

## 5. Flujo de trabajo en pareja con Git

1. Un integrante crea el repositorio e invita al otro como **colaborador**.
2. Los dos hacen `git clone` del mismo repositorio.
3. El trabajo se divide **por secciones**, para no editar las mismas líneas.
4. Cada integrante trabaja con este ciclo:

```
git pull
git add .
git commit -m "seccion: descripcion del cambio"
git pull
git push
```

## 6. Cómo ver el proyecto

- **En línea (GitHub Pages):** [https://davidtello17.github.io/practica-pixel-perfect/](https://davidtello17.github.io/practica-pixel-perfect/)
- **En local:** clonar el repositorio y abrir `index.html` en el navegador (o con Live Server en VS Code).
