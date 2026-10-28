# Día 5 · Hacerla interactiva con JavaScript y compartirla

[← Día 4](dia-04.md) · [Volver al README](../README.md)

Hoy la página deja de ser solo para mirar: reacciona cuando alguien la toca. Y se la muestran a Mauro.

## Cómo se maneja el tiempo

| Minutos | Qué hacen |
|---|---|
| 0 – 10 | Repaso: abrir la página pública y el repo |
| 10 – 50 | [Bloque 1](#bloque-1--conectar-javascript-40-min): conectar JavaScript |
| 50 – 60 | Descanso |
| 60 – 100 | [Bloque 2](#bloque-2--un-botón-que-saluda-40-min): un botón que saluda |
| 100 – 140 | [Bloque 3](#bloque-3--modo-oscuro-40-min): modo oscuro |
| 140 – 170 | [Bloque 4](#bloque-4--pulir-y-presentar-30-min): pulir y presentar |
| 170 – 180 | Cierre |

---

## Bloque 1 · Conectar JavaScript (40 min)

HTML es el contenido, CSS el aspecto y **JavaScript** el comportamiento.

1. Creen un archivo `app.js` junto a `index.html`, con una sola línea:

```js
console.log("Hola desde JavaScript");
```

2. En `index.html`, justo antes de `</body>`, agreguen:

```html
<script src="app.js" defer></script>
```

3. Abran la página con Live Server, apreten `F12` y vayan a la pestaña **Console**.

**Cómo saben que salió bien:** en la consola aparece `Hola desde JavaScript`.

Commit y push: `Conecto JavaScript`.

---

## Descanso (10 min)

---

## Bloque 2 · Un botón que saluda (40 min)

1. En `index.html`, dentro del `<body>`, agreguen:

```html
<button id="saludo">Tocá para saludar</button>
<p id="mensaje"></p>
```

2. En `app.js` (pueden borrar el `console.log`):

```js
const boton = document.getElementById("saludo");
const mensaje = document.getElementById("mensaje");

boton.addEventListener("click", () => {
  mensaje.textContent = "¡Hola! Gracias por visitar nuestra página.";
});
```

Qué hace cada parte:

| Código | Qué hace |
|---|---|
| `getElementById("saludo")` | Busca en la página el elemento con ese `id` |
| `addEventListener("click", ...)` | Avisa: "cuando hagan clic, ejecutá esto" |
| `textContent = ...` | Cambia el texto de un elemento |

3. Cambien el mensaje y agreguen un segundo botón con otro mensaje.

Commit y push: `Agrego un botón que saluda`.

---

## Bloque 3 · Modo oscuro (40 min)

1. En `index.html`, agreguen un botón:

```html
<button id="tema">Cambiar a modo oscuro</button>
```

2. En `estilos.css`:

```css
body.oscuro {
  background-color: #1b1b1b;
  color: #eeeeee;
}

body.oscuro section {
  background-color: #2a2a2a;
}
```

3. En `app.js`:

```js
const botonTema = document.getElementById("tema");

botonTema.addEventListener("click", () => {
  document.body.classList.toggle("oscuro");
});
```

`classList.toggle` pone la clase `oscuro` si no está y la saca si está.

4. Prueben que ande en la dirección pública, no solo en Live Server.

Commit y push: `Agrego modo oscuro`.

---

## Bloque 4 · Pulir y presentar (30 min)

1. Revisen la página completa en el celular. Corrijan lo que no les guste.
2. Revisen que **no haya contraseñas ni datos personales** en ningún archivo del repo: es público.
3. Preparen una presentación de 3 minutos para Mauro: qué hicieron, qué fue lo más difícil, qué cambiarían.

---

## Cierre (10 min)

- Presenten la página a Mauro, desde el link público.
- Sigan con la recomendación de [Para seguir en tu casa](../para-seguir-en-casa.md).
- Pueden seguir editando su página todos los días: cada push se publica solo.
