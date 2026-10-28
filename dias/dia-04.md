# Día 4 · Darle estilo con CSS

[← Día 3](dia-03.md) · [Volver al README](../README.md) · [Día 5 →](dia-05.md)

Su página ya existe pero se ve como un documento de texto. Hoy le ponen colores, tipografía, secciones y fotos.

Trabajan igual que ayer: editan, guardan, **Commit to main**, **Push origin**, y a los dos minutos se ve en la dirección pública.

## Cómo se maneja el tiempo

| Minutos | Qué hacen |
|---|---|
| 0 – 10 | Repaso: abrir la página pública y el repo |
| 10 – 40 | [Bloque 1](#bloque-1--el-archivo-de-estilos-30-min): el archivo de estilos |
| 40 – 50 | Descanso |
| 50 – 85 | [Bloque 2](#bloque-2--colores-y-tipografía-35-min): colores y tipografía |
| 85 – 120 | [Bloque 3](#bloque-3--secciones-y-cajas-35-min): secciones y cajas |
| 120 – 155 | [Bloque 4](#bloque-4--imágenes-35-min): imágenes |
| 155 – 175 | [Bloque 5](#bloque-5--probar-en-el-celular-20-min): probar en el celular |
| 175 – 180 | Cierre |

---

## Bloque 1 · El archivo de estilos (30 min)

HTML dice **qué** hay en la página. CSS dice **cómo se ve**. Van en archivos separados.

1. Creen un archivo `estilos.css` junto a `index.html`.
2. Pongan esto adentro:

```css
body {
  background-color: #fdf6e3;
}
```

3. En `index.html`, dentro de `<head>` (debajo de `<title>`), agreguen:

```html
<link rel="stylesheet" href="estilos.css">
```

4. Guarden ambos archivos y miren Live Server: el fondo cambió.
5. Commit y push: `Agrego estilos.css`.

**Cómo saben que salió bien:** el fondo es crema, en Live Server y en la dirección pública.

---

## Descanso (10 min)

---

## Bloque 2 · Colores y tipografía (35 min)

Prueben y cambien los valores hasta que les guste:

```css
body {
  background-color: #fdf6e3;
  color: #333333;
  font-family: Georgia, serif;
  max-width: 40rem;
  margin: 0 auto;
  padding: 1rem;
}

h1 {
  color: #b5338a;
}

a {
  color: #1d6fa5;
}
```

| Propiedad | Qué hace |
|---|---|
| `color` | Color del texto |
| `background-color` | Color de fondo |
| `font-family` | Tipo de letra |
| `max-width` | Ancho máximo del contenido |
| `margin: 0 auto` | Centra el contenido |
| `padding` | Espacio interior |

Para elegir colores: en VS Code, al escribir un `#`, aparece un selector de color.

Commit y push: `Pongo colores y tipografía`.

---

## Bloque 3 · Secciones y cajas (35 min)

1. En `index.html`, envuelvan cada parte (Quiénes somos, Qué estamos aprendiendo, Links) en una etiqueta `<section>`:

```html
<section>
  <h2>Quiénes somos</h2>
  <p>...</p>
</section>
```

2. En `estilos.css`, denles aspecto de tarjeta:

```css
section {
  background-color: #ffffff;
  border-radius: 12px;
  padding: 1rem 1.5rem;
  margin-bottom: 1rem;
}
```

3. Prueben cambiar `border-radius`, `padding` y `margin-bottom` y vean qué pasa con cada uno.

Commit y push: `Separo la página en secciones`.

---

## Bloque 4 · Imágenes (35 min)

1. Creen una carpeta `imagenes` en el repo y copien adentro una foto o dibujo de ustedes.
2. **El nombre del archivo, todo en minúsculas, sin espacios y sin tildes ni ñ**: `foto-equipo.jpg`, no `Foto Equipo.JPG`. GitHub Pages distingue mayúsculas de minúsculas y un nombre distinto da una imagen rota.
3. Agréguenla:

```html
<img src="imagenes/foto-equipo.jpg" alt="Vir y Delfi trabajando en la compu">
```

El `alt` describe la imagen para quien no puede verla y se muestra si falla la carga.

4. Que no se salga de la pantalla:

```css
img {
  max-width: 100%;
  height: auto;
  border-radius: 12px;
}
```

Commit y push: `Agrego una foto`. Si la imagen no aparece en la dirección pública, revisen el nombre del archivo y de la carpeta.

---

## Bloque 5 · Probar en el celular (20 min)

1. Abran la dirección pública en el celular.
2. En la compu: en el navegador apreten `F12` y después `Ctrl+Shift+M` para simular distintos celulares.
3. Si algo se ve mal (texto muy chico, algo cortado), anótenlo y corríjanlo.

---

## Cierre (5 min)

- Cuéntenle a Mauro qué cambio les gustó más.
- Mañana: botones que hacen cosas con JavaScript.
