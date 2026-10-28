# Día 2 · Git y GitHub en la práctica

[← Día 1](dia-01.md) · [Volver al README](../README.md) · [Día 3 →](dia-03.md)

> **Qué cambió:** el objetivo ahora es publicar su primera página con GitHub Pages ([Día 3](dia-03.md)). Trabajan directo en su repo, así que los bloques de **ramas** y **pull request** de esta guía son opcionales. Lo que sí sirve: historial, deshacer cambios, issues y el [bloque 5](#bloque-5--charla-con-mauro-el-flujo-de-trabajo-30-min) con Mauro.

Ayer hiciste tu primer pull request. Hoy aprendés a trabajar con **ramas**, a **deshacer cambios** y a usar **issues**, y además le preguntás a Mauro cómo es el flujo de trabajo de verdad en Hook.

## Cómo se maneja el tiempo

| Minutos | Qué hacés |
|---|---|
| 0 – 15 | [Bloque 1](#bloque-1--repaso-y-sincronizar-tu-fork-15-min): repaso y sincronizar tu fork |
| 15 – 45 | [Bloque 2](#bloque-2--ramas-30-min): ramas |
| 45 – 55 | Descanso |
| 55 – 85 | [Bloque 3](#bloque-3--historial-y-deshacer-30-min): historial y deshacer cambios |
| 85 – 115 | [Bloque 4](#bloque-4--issues-30-min): issues |
| 115 – 145 | [Bloque 5](#bloque-5--charla-con-mauro-el-flujo-de-trabajo-30-min): charla con Mauro, el flujo de trabajo |
| 145 – 175 | [Bloque 6](#bloque-6--tus-notas-del-flujo-30-min): tus notas del flujo |
| 175 – 180 | Cierre |

Si algo no sale en **10 minutos**, avisale a Mauro.

---

## Bloque 1 · Repaso y sincronizar tu fork (15 min)

1. Entrá a tu pull request de ayer en GitHub. Si Mauro dejó comentarios, leelos y contestalos.
2. Tu copia (`tu-usuario/pasantes`) no se actualiza sola cuando el proyecto original cambia. Para traer lo nuevo: entrá a tu copia en GitHub y tocá **Sync fork** → **Update branch**.
3. En VS Code, abrí la terminal (`Ctrl+ñ`) y escribí:

```
git pull
```

**Cómo sé que salió bien:** ves la carpeta `dias` con los archivos de cada día.

---

## Bloque 2 · Ramas (30 min)

Una **rama** (branch) es una línea paralela de trabajo: probás cosas sin tocar la versión principal (`main`). Es lo que se hace en cualquier proyecto real.

1. Creá una rama nueva. En la terminal:

```
git switch -c dia-02/tu-nombre
```

2. Abajo a la izquierda de VS Code tiene que decir `dia-02/tu-nombre`.
3. Creá el archivo `bienvenida/tu-nombre-dia-2.md` con una frase sobre qué aprendiste ayer.
4. Hacé commit (ícono de ramitas → mensaje → **Commit**).
5. Subí la rama: **Publicar rama** (o `git push -u origin dia-02/tu-nombre`).
6. En GitHub, abrí un pull request de esa rama, como ayer.

**Cómo sé que salió bien:** en GitHub ves la lista de ramas con la tuya.

---

## Descanso (10 min)

---

## Bloque 3 · Historial y deshacer (30 min)

1. En GitHub, entrá a tu copia y tocá **Commits**. Ahí está todo lo que se hizo, quién lo hizo y cuándo.
2. En VS Code, abrí un archivo, hacé un cambio sin guardarlo en un commit y probá deshacerlo: en **Control de código fuente**, hacé clic derecho sobre el archivo → **Descartar cambios**.
3. Ahora hacé un cambio, commitealo, y después deshacelo con un commit nuevo:

```
git revert HEAD
```

4. Mirá el historial de nuevo: el cambio y su reversión quedan los dos. En Git nada se pierde.

**Pregunta para pensar:** ¿para qué sirve que el historial guarde todo, incluso los errores?

---

## Bloque 4 · Issues (30 min)

Un **issue** es una tarea o un problema anotado en GitHub. Así se organiza el trabajo en equipo.

1. En tu copia de GitHub, andá a la pestaña **Issues**. Si no aparece, entrá a **Settings** → buscá **Issues** y activalo.
2. Creá un issue: título `Mejorar mi bienvenida`, y en la descripción, qué te gustaría agregar.
3. Volvé a VS Code, hacé el cambio en tu archivo de bienvenida y commiteá con este mensaje, con el número que te dio GitHub:

```
Mejoro mi bienvenida (cierra #1)
```

4. Subí el cambio. Cuando el cambio llegue a `main`, GitHub cierra el issue solo.

---

## Bloque 5 · Charla con Mauro: el flujo de trabajo (30 min)

Hasta ahora aprendiste las herramientas de a una. Ahora tenés que ver cómo se usan juntas en un trabajo real.

**Tu tarea:** preguntale a Mauro **cómo es el flujo de trabajo** en Hook. Mauro te va a mostrar cómo trabaja con **Claude CLI** (un asistente de IA que corre en la terminal).

Mientras mira, anotá en `bienvenida/tu-nombre-flujo.md`:

1. ¿Por dónde empieza una tarea?
2. ¿Qué hace Claude y qué hace Mauro?
3. ¿Cómo se revisa lo que Claude escribió antes de subirlo?
4. ¿Cómo se sabe que un cambio llegó bien a producción (a los usuarios reales)?

**Preguntas sugeridas para hacerle:**

- ¿Por qué no se sube todo directo a `main`?
- ¿Qué pasa si la IA se equivoca?
- ¿Qué tengo que saber yo para poder pedirle cosas bien?

---

## Bloque 6 · Tus notas del flujo (30 min)

1. Ordená lo que anotaste en `bienvenida/tu-nombre-flujo.md`: un título, los 4 puntos de arriba y, al final, **una duda que te quedó**.
2. Commit y push en tu rama `dia-02/tu-nombre`.
3. Si el pull request del Bloque 2 sigue abierto, el cambio se suma solo. Avisale a Mauro.

---

## Cierre (5 min)

- Contale a Mauro cuál de las cosas de hoy te costó más.
- Mañana: tu primera página web con HTML y CSS.
