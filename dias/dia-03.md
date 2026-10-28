# Día 3 · Publicar la primera página

[← Día 2](dia-02.md) · [Volver al README](../README.md) · [Día 4 →](dia-04.md)

Hoy hacen su primera página web y la publican en internet. Al final del día cualquiera con el link puede verla.

**Cómo trabajan:** directo en este repo, sin fork ni pull request. Editan en VS Code, guardan con commit y push desde GitHub Desktop (los pasos están en el [README](../README.md#cómo-trabajan-desde-ahora)).

## Cómo se maneja el tiempo

| Minutos | Qué hacen |
|---|---|
| 0 – 15 | [Bloque 1](#bloque-1--abrir-el-repo-15-min): abrir el repo |
| 15 – 45 | [Bloque 2](#bloque-2--su-primer-indexhtml-30-min): su primer `index.html` |
| 45 – 55 | Descanso |
| 55 – 85 | [Bloque 3](#bloque-3--primer-commit-y-push-30-min): primer commit y push |
| 85 – 115 | [Bloque 4](#bloque-4--activar-github-pages-30-min): activar GitHub Pages |
| 115 – 150 | [Bloque 5](#bloque-5--completar-la-página-35-min): completar la página |
| 150 – 175 | [Bloque 6](#bloque-6--compartir-el-link-25-min): compartir el link |
| 175 – 180 | Cierre |

---

## Bloque 1 · Abrir el repo (15 min)

1. Abran **GitHub Desktop**. Arriba a la izquierda, en *Current repository*, tiene que decir `pasantes`.
2. Si no aparece, vayan a **File → Clone repository**, elijan `virydelfi/pasantes` y una carpeta.
3. Menú **Repository → Open in Visual Studio Code**.

**Cómo saben que salió bien:** VS Code muestra, a la izquierda, las carpetas `dias` y `bienvenida`.

---

## Bloque 2 · Su primer `index.html` (30 min)

GitHub Pages busca un archivo llamado exactamente `index.html` en la raíz del repo y lo muestra como página principal.

1. En VS Code, en el panel de la izquierda, creen un archivo nuevo (ícono de hoja con un `+`) y llámenlo `index.html`. Tiene que estar suelto, **no dentro de una carpeta**.
2. Pegan esto:

```html
<!DOCTYPE html>
<html lang="es">
  <head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Vir y Delfi</title>
  </head>
  <body>
    <h1>Hola, somos Vir y Delfi</h1>
    <p>Esta es nuestra primera página web.</p>
  </body>
</html>
```

3. Guarden con `Ctrl+S`.

### Verla en el navegador

1. Si todavía no la instalaron: en VS Code, abran extensiones (`Ctrl+Shift+X`), busquen **Live Server** (de *Ritwick Dey*) e instálenla.
2. Clic derecho sobre `index.html` → **Open with Live Server** (o el botón **Go Live** abajo a la derecha).
3. Cambien el texto del `<h1>`, guarden, y miren cómo el navegador se actualiza solo.

### Qué es cada cosa

| Etiqueta | Para qué sirve |
|---|---|
| `<h1>` | Título principal |
| `<p>` | Un párrafo |
| `<title>` | El nombre que sale en la pestaña del navegador |
| `<body>` | Todo lo que se ve en la página |

**Cómo saben que salió bien:** ven su título en el navegador.

---

## Descanso (10 min)

---

## Bloque 3 · Primer commit y push (30 min)

1. Abran GitHub Desktop. En **Changes** aparece `index.html`.
2. Escriban un resumen: `Agrego mi primera página`.
3. **Commit to main**.
4. **Push origin**.
5. Entren a <https://github.com/virydelfi/pasantes> en el navegador y comprueben que `index.html` está en la lista de archivos.

**Pregunta para pensar:** ¿qué pasó con el archivo entre que lo guardaron en VS Code y que lo vieron en GitHub?

---

## Bloque 4 · Activar GitHub Pages (30 min)

Esto lo hace una vez la **dueña del repo** (la cuenta `virydelfi`). Si Delfi usa otra cuenta, la dueña primero la agrega: **Settings → Collaborators → Add people**.

1. En GitHub, en el repo `pasantes`, toquen **Settings** (arriba a la derecha).
2. A la izquierda, **Pages**.
3. En *Build and deployment* → *Source*, elijan **Deploy from a branch**.
4. En *Branch*, elijan **main** y la carpeta **/ (root)**. Toquen **Save**.
5. Esperen uno o dos minutos y refresquen la pestaña. Arriba aparece:

> Your site is live at `https://virydelfi.github.io/pasantes/`

**Cómo saben que salió bien:** abrir esa dirección muestra la misma página que vieron con Live Server.

Si dice 404, esperen otro minuto y prueben de nuevo. Si sigue igual a los 10 minutos, avisen a Mauro.

---

## Bloque 5 · Completar la página (35 min)

Agreguen estas secciones, de a una, y **hagan un commit y push después de cada una**:

1. Un `<h2>` con **Quiénes somos** y un párrafo cada una.
2. Un `<h2>` con **Qué estamos aprendiendo** y una lista:

```html
<ul>
  <li>Git y GitHub</li>
  <li>HTML</li>
</ul>
```

3. Un `<h2>` con **Links** y un enlace a la app de Hook:

```html
<a href="https://app.balanzashook.com.ar">La app de Hook</a>
```

Después de cada push, esperen un minuto y refresquen la dirección pública: vean el cambio en vivo.

---

## Bloque 6 · Compartir el link (25 min)

1. Mándenle a Mauro el link de la página.
2. Ábranlo desde el celular de cada una.
3. Anoten en [`preguntas-app.md`](../preguntas-app.md) algo que quieran cambiar de la página. Mañana lo hacen.

---

## Cierre (5 min)

- Tienen una página publicada. Eso ya es un logro.
- Mañana: colores, tipografías y fotos con CSS.
