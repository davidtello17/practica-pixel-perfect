# Aprendizajes y dificultades

Práctica de maquetación _pixel perfect_ de la página de Disney, en parejas.

---

## Juan David Tello

**Secciones que hice:** navbar, banner, shop y Disney+.

### Lo que aprendí

- **Trabajar en pareja con Git:** crear el repositorio, invitar a un colaborador y usar el flujo `git pull` → `git add` → `git commit` → `git pull` → `git push` para no pisar el trabajo del otro.
- **Dividir el trabajo por secciones** (no por lenguaje): cada uno hace el HTML y el CSS de su parte, así los dos avanzan al mismo tiempo.
- **Metodología BEM:** bloques (`navbar`, `shop-card`), elementos (`navbar__link`, `shop-card__image`) y modificadores (`banner__button--primary`, `banner__button--outline`).
- **Rutas en CSS:** en `background-image: url("../img/...")` la ruta se cuenta desde el archivo CSS. Como `styles.css` está en la carpeta `css/`, hay que salir con `../` para llegar a `img/`.
- **Imágenes parejas:** `aspect-ratio` define la forma (1 / 1 cuadrada, 16 / 9 rectangular) y `object-fit: cover` la recorta sin deformarla.
- **Emparejar alturas de tarjetas:** la tarjeta con `display: flex` y `flex-direction: column`, y el cuerpo con `flex: 1` para que crezca y quede del mismo alto que las demás.
- **`justify-content: space-between`** para separar el logo y el menú a la izquierda y el buscador a la derecha.

### Dificultades que tuve

- **Carpetas en vez de archivos:** al crear la estructura, algunos archivos (`index.html`, `README.md`, `styles.css`) quedaron como carpetas. Lo solucioné con `rmdir` y `touch`, y aprendí a revisar con `ls -F` (las carpetas salen con `/`).
- **Pegar comandos en Git Bash:** al pegar con Ctrl + V se colaron caracteres raros (`^[[200~`) y el comando falló. Es mejor pegar con clic derecho o Shift + Insert.
- **Errores de escritura en las clases:** el estilo del LOG IN no se aplicaba porque el nombre de la clase estaba mal escrito. Hay que comparar letra por letra el HTML y el CSS.
- **Grilla que no funcionaba:** en Disney+ las tarjetas salían una debajo de otra porque faltaba el `div.disney-plus__grid` en el HTML. El CSS estaba bien, pero no encontraba ningún elemento con esa clase.
- **Imagen equivocada y rutas incompletas:** una imagen no cargaba porque le faltaba `img/` en el `src`.
- **Sangría al pegar código:** si se pega con el cursor en medio de una línea, todo queda corrido. Se arregla con Shift + Alt + F.

---

## Juan Arias

**Secciones que hice:** movies, parks and travel, more y footer.

### Lo que aprendí

- (completar)

### Dificultades que tuve

- (completar)
