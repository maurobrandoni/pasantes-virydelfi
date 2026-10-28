# Día 1 · Cuentas e instalación

[← Volver al README](../README.md) · [Día 2 →](dia-02.md)

> **Ya lo hicieron.** Las cuentas, VS Code, Git y GitHub Desktop ya están instalados. Dos cosas cambiaron desde que se escribió esta guía:
>
> - **Ya no hay fork ni pull request.** Este repo es de ustedes: guardan con commit y push directo, desde GitHub Desktop (ver el [README](../README.md#cómo-trabajan-desde-ahora)).
> - **Node.js ya no hace falta** por ahora (ver el [README](../README.md#y-nodejs)). Saltéense el bloque 7.

Datos de acceso (mail, app demo, PIN de la computadora): están en la tabla del [README](../README.md#datos-que-necesitan).

## Cómo se maneja el tiempo

El día 1 son **180 minutos**. Descargar e instalar programas lleva rato, y mirar la pantalla esperando es tiempo perdido. Por eso:

> **Regla de oro:** mientras algo se descarga o se instala, no te quedes mirando la barra. Pasá a la columna **"Mientras tanto"** y mirá la app.

| Minutos | Qué hacés | Mientras tanto |
|---|---|---|
| 0 – 10 | [Bloque 1](#bloque-1--leer-y-abrir-el-mail-10-min): leer este README y abrir el mail | |
| 10 – 25 | [Bloque 2](#bloque-2--cuenta-de-github-15-min): crear tu cuenta de GitHub | |
| 25 – 40 | [Bloque 3](#bloque-3--visual-studio-code-15-min): descargar e instalar VS Code | [Recorrer la app](#mientras-tanto-a-recorrer-la-app) y anotar 5 cosas que no entiendas |
| 40 – 55 | [Bloque 4](#bloque-4--git-15-min): descargar e instalar Git | Mirar **Animales** y **Corrales** en la app |
| 55 – 65 | Descanso | |
| 65 – 85 | [Bloque 5](#bloque-5--configurar-vs-code-y-git-20-min): configurar VS Code y Git | Mirar **Dietas** y **Pesajes** en la app |
| 85 – 115 | [Bloque 6](#bloque-6--tu-primer-aporte-en-github-30-min): tu primer aporte | |
| 115 – 145 | [Bloque 7](#bloque-7--nodejs-30-min--ya-no-hace-falta): Node.js (ya no hace falta, saltear) | Mirar **Balanzas** y **Reportes** en la app |
| 145 – 170 | [Bloque 8](#bloque-8--pull-request-y-cuestionario-25-min): pull request y cuestionario | Completar [`preguntas-app.md`](../preguntas-app.md) |
| 170 – 180 | [Cierre](#cierre-10-min) | |

Marcá cada bloque como hecho a medida que avanzás. Si terminás uno antes, pasá al siguiente. Si un bloque se te pasa del tiempo, avisale a Mauro.

---

## Bloque 1 · Leer y abrir el mail (10 min)

1. Leíste hasta acá: ya hiciste la primera parte.
2. Abrí <https://mail.balanzashook.com.ar>.
3. Entrá con `pasantes@balanzashook.com.ar` y la contraseña que te dio Mauro.

**Cómo sé que salió bien:** ves una bandeja de entrada.

Vas a usar este mail para todas las cuentas que creés en estos días.

---

## Bloque 2 · Cuenta de GitHub (15 min)

GitHub es el lugar donde se guarda el código de los proyectos en internet, con todo su historial de cambios. Es como un Google Drive para programadores.

1. Entrá a <https://github.com/signup>.
2. Usá el mail `pasantes@balanzashook.com.ar`.
3. Elegí una contraseña y un nombre de usuario (sin espacios, por ejemplo `nombre-apellido`). **Anotalos en un lugar seguro.**
4. GitHub te manda un código por mail: volvé a la pestaña del mail, copialo y pegalo.
5. Cuando te pregunte para qué lo usás, elegí lo que quieras o saltá las preguntas.

**Cómo sé que salió bien:** ves tu página principal de GitHub con tu usuario arriba a la derecha.

---

## Bloque 3 · Visual Studio Code (15 min)

VS Code es el programa donde se escribe el código. Es como un procesador de texto, pero hecho para programar.

1. Entrá a <https://code.visualstudio.com>.
2. Tocá el botón de descarga que te ofrece para tu sistema.
3. Cuando termine, abrí el archivo descargado y seguí el instalador con **Siguiente** en todo. Si te aparecen opciones, dejá las marcadas como están.
4. Abrí VS Code una vez para ver que arranca.

**Cómo sé que salió bien:** se abre una ventana oscura con "Welcome" o "Bienvenido".

### Mientras tanto: a recorrer la app

Mientras se descarga, abrí otra pestaña en <https://app.balanzashook.com.ar>, entrá con el usuario demo y:

1. Mirá todo el menú, sin apuro.
2. Abrí cada sección, aunque no entiendas qué es.
3. Anotá **5 cosas que no entiendas** en [`preguntas-app.md`](../preguntas-app.md). Más adelante las vas a subir a GitHub.

---

## Bloque 4 · Git (15 min)

Git es el programa que anota todos los cambios que hacés en el código. GitHub guarda eso en internet; Git es lo que corre en tu computadora.

1. Entrá a <https://git-scm.com/downloads> y descargá la versión para tu sistema.
2. Instalalo con **Next / Siguiente** en todas las pantallas.
3. Para comprobar que quedó bien, abrí una **terminal** (una ventana donde se escriben comandos):
   - **Windows:** apretá la tecla Windows, escribí `Git Bash` y abrilo.
   - **Mac:** abrí la app `Terminal`.
4. Escribí esto y apretá Enter:

```
git --version
```

**Cómo sé que salió bien:** aparece algo como `git version 2.x.x`.

**Mientras tanto:** mirá **Animales** y **Corrales** en la app. ¿Podés encontrar un animal puntual? ¿En qué corral está?

---

## Descanso (10 min)

Pará diez minutos. Tomá agua, caminá un poco.

---

## Bloque 5 · Configurar VS Code y Git (20 min)

### Decirle a Git quién sos

En la terminal (la misma de antes), escribí estas dos líneas, cambiando lo que está entre comillas por tus datos:

```
git config --global user.name "Tu Nombre"
git config --global user.email "pasantes@balanzashook.com.ar"
```

No aparece nada si sale bien.

### Conectar VS Code con GitHub

1. En VS Code, hacé clic en el ícono de la persona (abajo a la izquierda) → **Iniciar sesión con GitHub**.
2. Se abre el navegador: aceptá los permisos con tu cuenta de GitHub.
3. Volvé a VS Code. Tiene que mostrar tu nombre de usuario.

### Extra (opcional)

Si querés VS Code en español: apretá `Ctrl+Shift+X` (en Mac `Cmd+Shift+X`), buscá **Spanish Language Pack** e instalalo.

**Mientras tanto:** mirá **Dietas** y **Pesajes** en la app. ¿Qué creés que es una "dieta" para un animal?

---

## Bloque 6 · Tu primer aporte en GitHub (30 min)

Acá vas a hacer lo que hace cualquier programador todos los días: copiar un proyecto, cambiar algo y proponer el cambio.

### 1. Hacer tu copia (fork)

1. Estando logueado/a en GitHub, entrá a <https://github.com/Balanzas-Hook/pasantes>.
2. Tocá el botón **Fork** (arriba a la derecha) → **Create fork**.
3. Ahora tenés tu propia copia, que se llama `tu-usuario/pasantes`.

### 2. Bajarla a tu computadora (clonar)

1. En tu copia, tocá el botón verde **Code** y copiá la dirección que aparece (la que empieza con `https://`).
2. En VS Code: `Ctrl+Shift+P` (Mac: `Cmd+Shift+P`), escribí `Git: Clone`, pegá la dirección y elegí una carpeta (por ejemplo, Documentos).
3. Cuando pregunte si querés abrir la carpeta, decí **Abrir**.

### 3. Crear tu archivo de bienvenida

1. En el panel de la izquierda, abrí la carpeta `bienvenida`.
2. Creá un archivo nuevo: `tu-nombre.md` (por ejemplo, `lucia.md`).
3. Escribí lo siguiente, cambiando lo que haga falta:

```
# Hola, soy Lucía

- Me gusta: ...
- Lo que más me interesa de la pasantía: ...
- Algo que hice en Scratch: ...
```

4. Guardá con `Ctrl+S`.

### 4. Guardar el cambio (commit y push)

1. En VS Code, hacé clic en el ícono de ramitas de la izquierda (**Control de código fuente**).
2. Vas a ver tu archivo en la lista. Escribí un mensaje arriba, por ejemplo `Agrego mi bienvenida`.
3. Tocá **Commit** (si pregunta algo, elegí **Sí**).
4. Tocá **Sincronizar cambios** o **Push**.

**Cómo sé que salió bien:** en GitHub, en tu copia (`tu-usuario/pasantes`), la carpeta `bienvenida` ya tiene tu archivo.

---

## Bloque 7 · Node.js (30 min) · ya no hace falta

> Para publicar una página con HTML, CSS y JavaScript no se necesita Node.js. Si ya lo instalaron, no pasa nada. Si no, no lo instalen todavía.

Node.js es lo que permite ejecutar JavaScript fuera del navegador.

1. Entrá a <https://nodejs.org> y descargá la versión **LTS** (la que dice "Recomendado para la mayoría").
2. Instalalo con **Siguiente** en todo.
3. Cerrá y abrí de nuevo la terminal. Escribí:

```
node --version
```

**Cómo sé que salió bien:** aparece un número como `v22.x.x` (o mayor).

**Mientras tanto:** mirá **Balanzas** y **Reportes** en la app. ¿Qué datos se pueden sacar de una balanza?

---

## Bloque 8 · Pull request y cuestionario (25 min)

### Proponer tu cambio (pull request)

Un pull request es pedirle al dueño del proyecto: "Che, mirá mi cambio, ¿lo sumamos?".

1. En GitHub, en tu copia `tu-usuario/pasantes`, aparece un cartel amarillo con **Compare & pull request**. Tocalo.
2. Escribí un título (por ejemplo, `Bienvenida de Lucía`).
3. Tocá **Create pull request**.
4. Avisale a Mauro que ya lo abriste.

### Cuestionario

Abrí [`preguntas-app.md`](../preguntas-app.md) en VS Code, completalo con lo que anotaste mientras mirabas la app, y repetí el paso "Guardar el cambio" del bloque 6 (commit y push). El cambio se suma solo a tu pull request.

---

## Cierre (10 min)

- Revisá que hayas marcado todos los bloques.
- Contale a Mauro qué fue lo más difícil y qué fue lo más fácil.
- Mañana seguimos con Git y GitHub en la práctica.
