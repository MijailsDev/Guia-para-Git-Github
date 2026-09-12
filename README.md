# 📘 Guía básica de Git + GitHub

## Para equipos principiantes --- Windows 11

> **Objetivo:** aprender a trabajar en equipo usando Git y GitHub de una
> manera sencilla, sin ramas ni procesos complicados.

------------------------------------------------------------------------

# 📑 Índice

1.  [Primero: ¿qué es Git y GitHub?](#seccion-1)
2.  [Cómo será el trabajo de ustedes](#seccion-2)
3.  [Parte 1 --- Crear una cuenta de GitHub](#seccion-3)
4.  [Parte 2 --- Instalar Git en Windows 11](#seccion-4)
5.  [Parte 3 --- Comprobar que Git funciona](#seccion-5)
6.  [Parte 4 --- Configurar Git](#seccion-6)
7.  [Parte 5 --- Crear el repositorio](#seccion-7)
8.  [Parte 6 --- Agregar a los integrantes](#seccion-8)
9.  [Parte 7 --- Descargar el proyecto](#seccion-9)
10. [Parte 8 --- Entrar al proyecto](#seccion-10)
11. [Parte 9 --- Abrir el proyecto](#seccion-11)
12. [Ahora viene lo más importante](#seccion-12)
13. [Juan trabaja](#seccion-13)
14. [Guardar los cambios](#seccion-14)
15. [Preparar los cambios](#seccion-15)
16. [Crear el commit](#seccion-16)
17. [Subir a GitHub](#seccion-17)
18. [Al día siguiente: María](#seccion-18)
19. [Y así durante meses](#seccion-19)
20. [La "chuleta" que deben tener todos](#seccion-20)
21. [Reglas de oro del grupo](#seccion-21)
22. [¿Qué pasa si aparece un error?](#seccion-22)
23. [Entender Git en 30 segundos](#seccion-23)

------------------------------------------------------------------------

<a id="seccion-1"></a>

# 1. Primero: ¿qué es Git y GitHub?

Piensen en esto:

**Git** = programa que guarda el historial de cambios de su proyecto en
la computadora.

**GitHub** = página web donde guardan el proyecto y lo comparten entre
todos.

Una forma sencilla de verlo:

``` text
TU PC                         GITHUB
┌──────────────┐              ┌──────────────┐
│   Proyecto   │   ───────►   │ Repositorio  │
│              │    push      │    main      │
│   Git        │   ◄───────   │              │
└──────────────┘     pull     └──────────────┘
```

### Las 3 palabras que deben aprender primero

  Palabra    Significado sencillo
  ---------- -------------------------------------
  `clone`    Descargar el proyecto de GitHub
  `pull`     Traer los últimos cambios de GitHub
  `push`     Subir tus cambios a GitHub
  `commit`   Guardar un punto de cambio en Git

------------------------------------------------------------------------

<a id="seccion-2"></a>

# 2. Cómo será el trabajo de ustedes

Supongamos que son 5 personas.

Van a tener:

``` text
GITHUB
   │
   └── main
        │
        ├── Día 1 → Persona 1
        ├── Día 2 → Persona 2
        ├── Día 3 → Persona 3
        ├── Día 4 → Persona 4
        └── Día 5 → Persona 5
```

### 🚨 REGLA PRINCIPAL

> **SOLO UNA PERSONA MODIFICA Y SUBE EL PROYECTO A LA VEZ.**

No importa si trabajan durante 2 semanas o 6 meses.

Todos utilizan:

``` text
main
```

No necesitan crear ramas todos los días.

------------------------------------------------------------------------

<a id="seccion-3"></a>

# 3. 🟢 PARTE 1 --- Crear una cuenta de GitHub

Cada integrante necesita una cuenta.

Entren a [GitHub](https://github.com/).

Presionen:

**Sign up**

Creen su cuenta.

### Recomendación

Utilicen un correo que revisen regularmente.

Por ejemplo:

``` text
nombre@gmail.com
```

------------------------------------------------------------------------

<a id="seccion-4"></a>

# 4. 🟢 PARTE 2 --- Instalar Git en Windows 11

En **cada computadora** deben instalar Git.

Descarguen Git para Windows desde:

https://git-scm.com/download/win

Instalen normalmente.

Durante la instalación pueden dejar prácticamente **todas las opciones
predeterminadas**.

Al terminar, tendrán:

**Git Bash**

No necesitan aprender Linux. Git Bash simplemente será nuestra terminal
para trabajar con Git.

------------------------------------------------------------------------

<a id="seccion-5"></a>

# 5. 🟢 PARTE 3 --- Comprobar que Git funciona

Abrir:

**Inicio → Git Bash**

Aparecerá una ventana parecida a:

``` text
MINGW64
usuario@PC ~
$
```

Escriban:

``` bash
git --version
```

Debería aparecer algo parecido a:

``` text
git version 2.x.x
```

✅ Si aparece una versión, Git está instalado.

------------------------------------------------------------------------

<a id="seccion-6"></a>

# 6. 🟢 PARTE 4 --- Configurar Git

Cada integrante debe hacer esto **una sola vez**.

Escriban:

``` bash
git config --global user.name "Tu Nombre"
```

Por ejemplo:

``` bash
git config --global user.name "Juan Perez"
```

Luego:

``` bash
git config --global user.email "tu-correo@gmail.com"
```

Utilicen el correo asociado a su cuenta de GitHub.

Para comprobar:

``` bash
git config --global --list
```

------------------------------------------------------------------------

<a id="seccion-7"></a>

# 7. 🟢 PARTE 5 --- Crear el repositorio

Esto lo hará **una sola persona**.

Entren a GitHub.

Arriba a la derecha:

**+ → New repository**

Pongan el nombre.

Por ejemplo:

``` text
sistema-ventas
```

Seleccionen:

``` text
Public
```

o:

``` text
Private
```

Para un proyecto universitario normalmente pueden usar **Private** si no
quieren que cualquiera vea el código.

Marquen:

``` text
☑ Add a README file
```

Finalmente:

**Create repository**

🎉 Ya tienen su repositorio.

------------------------------------------------------------------------

<a id="seccion-8"></a>

# 8. 🟢 PARTE 6 --- Agregar a los integrantes

La persona que creó el repositorio debe entrar a:

``` text
Repository
   ↓
Settings
   ↓
Collaborators
```

Luego:

**Add people**

Busquen el nombre de usuario de GitHub de cada integrante.

Por ejemplo:

``` text
juan123
maria456
pedro789
ana123
```

Cada integrante recibirá una invitación.

⚠️ **Cada uno debe aceptar la invitación.**

------------------------------------------------------------------------

<a id="seccion-9"></a>

# 9. 🟢 PARTE 7 --- Descargar el proyecto

Ahora cada integrante necesita tener una copia del proyecto en su PC.

Entren al repositorio.

Presionen:

**Code → HTTPS**

Copien la dirección.

Será parecida a:

``` text
https://github.com/usuario/sistema-ventas.git
```

------------------------------------------------------------------------

## Crear una carpeta para sus proyectos

Por ejemplo:

``` text
C:\Proyectos
```

En Windows pueden crearla desde el Explorador.

Después:

**Clic derecho dentro de la carpeta → Open Git Bash here**

Y escriben:

``` bash
git clone https://github.com/usuario/sistema-ventas.git
```

⚠️ Reemplacen la dirección por la de **su repositorio**.

------------------------------------------------------------------------

<a id="seccion-10"></a>

# 10. 🟢 PARTE 8 --- Entrar al proyecto

Después de clonar:

``` bash
cd sistema-ventas
```

Ahora están dentro del proyecto.

Pueden comprobarlo:

``` bash
git status
```

Debería aparecer algo parecido a:

``` text
On branch main
Your branch is up to date with 'origin/main'.

nothing to commit, working tree clean
```

Perfecto. ✅

------------------------------------------------------------------------

<a id="seccion-11"></a>

# 11. 🟢 PARTE 9 --- Abrir el proyecto

Si utilizan Visual Studio Code:

``` bash
code .
```

Se abrirá el proyecto.

Si `code .` no funciona, simplemente pueden abrir Visual Studio Code y
seleccionar la carpeta del proyecto.

------------------------------------------------------------------------

<a id="seccion-12"></a>

# 12. 🟡 AHORA VIENE LO MÁS IMPORTANTE

Supongamos que **hoy le toca trabajar a Juan**.

Antes de tocar absolutamente nada:

``` bash
git pull
```

Esto significa:

> "GitHub, dame la versión más reciente del proyecto."

------------------------------------------------------------------------

<a id="seccion-13"></a>

# 13. 👨‍💻 Juan trabaja

Ahora Juan modifica el proyecto.

Por ejemplo:

``` text
src/
├── usuarios/
├── productos/
├── ventas/
└── clientes/
```

Juan modifica:

``` text
clientes
```

Termina su trabajo y prueba que todo funcione.

------------------------------------------------------------------------

<a id="seccion-14"></a>

# 14. 🟢 Guardar los cambios

Primero:

``` bash
git status
```

Git mostrará los archivos modificados.

Por ejemplo:

``` text
modified: clientes.cs
modified: clientes_form.cs
```

------------------------------------------------------------------------

<a id="seccion-15"></a>

# 15. 🟢 Preparar los cambios

Escriban:

``` bash
git add .
```

El punto significa:

> "Agregar todos los cambios."

------------------------------------------------------------------------

<a id="seccion-16"></a>

# 16. 🟢 Crear el commit

Ahora:

``` bash
git commit -m "Agregué módulo de clientes"
```

El mensaje debe explicar **qué hicieron**.

Ejemplos buenos:

``` bash
git commit -m "Agregué formulario de clientes"
```

``` bash
git commit -m "Corregí validación de usuario"
```

``` bash
git commit -m "Agregué conexión a MySQL"
```

Eviten:

``` bash
git commit -m "cambios"
```

o:

``` bash
git commit -m "xd"
```

😂

------------------------------------------------------------------------

<a id="seccion-17"></a>

# 17. 🟢 Subir a GitHub

Ahora:

``` bash
git push
```

Esto envía los cambios a GitHub.

``` text
PC de Juan
    │
    │ git push
    ▼
GitHub
    │
    ▼
  main
```

🎉 Juan terminó.

------------------------------------------------------------------------

<a id="seccion-18"></a>

# 18. 👩‍💻 Al día siguiente: María

Ahora le toca a María.

María **NO debe comenzar inmediatamente a modificar archivos**.

Primero:

``` bash
git pull
```

Así obtiene lo que Juan hizo ayer.

Después trabaja normalmente.

Cuando termina:

``` bash
git add .
```

``` bash
git commit -m "Agregué módulo de productos"
```

``` bash
git push
```

------------------------------------------------------------------------

<a id="seccion-19"></a>

# 19. 🔁 Y así durante meses

El ciclo será siempre:

``` text
        EMPIEZA TU TURNO
              ↓
          git pull
              ↓
           TRABAJAR
              ↓
           PROBAR
              ↓
         git add .
              ↓
      git commit -m "..."
              ↓
          git push
              ↓
         TERMINÓ TU TURNO
```

El siguiente integrante:

``` text
          git pull
              ↓
           TRABAJAR
              ↓
           ...
```

------------------------------------------------------------------------

<a id="seccion-20"></a>

# 20. 📋 La "chuleta" que deben tener todos

Esta es la parte que recomiendo incluso **imprimir y pegar al lado de la
PC**:

### 🟢 AL COMENZAR

``` bash
git pull
```

### 🔵 DESPUÉS DE TRABAJAR

``` bash
git status
```

``` bash
git add .
```

``` bash
git commit -m "Descripción de lo que hice"
```

``` bash
git push
```

### Eso es todo.

``` text
┌───────────────────────────┐
│      GIT BÁSICO           │
├───────────────────────────┤
│                           │
│  INICIO:                  │
│  git pull                 │
│                           │
│  TRABAJAR                 │
│                           │
│  TERMINÉ:                 │
│  git status               │
│  git add .                │
│  git commit -m "..."      │
│  git push                 │
│                           │
└───────────────────────────┘
```

------------------------------------------------------------------------

<a id="seccion-21"></a>

# 21. ⚠️ REGLAS DE ORO DEL GRUPO

## Regla 1

**Nunca trabajen dos personas al mismo tiempo.**

Si Juan está trabajando:

``` text
🔴 JUAN → TRABAJANDO
🟢 MARÍA → ESPERA
🟢 PEDRO → ESPERA
```

------------------------------------------------------------------------

## Regla 2

Antes de empezar:

``` bash
git pull
```

**Siempre.**

------------------------------------------------------------------------

## Regla 3

Antes de hacer `push`, prueben el programa.

No hagan:

``` text
Código roto
     ↓
git add .
     ↓
git commit
     ↓
git push
```

Primero:

``` text
Código
 ↓
Probar
 ↓
Funciona ✅
 ↓
commit
 ↓
push
```

------------------------------------------------------------------------

## Regla 4

No borren la carpeta `.git`.

Normalmente estará oculta.

``` text
sistema-ventas/
│
├── .git/       ← ❌ NO TOCAR
├── README.md
├── src/
└── ...
```

`.git` es donde Git guarda el historial y configuración del repositorio.

------------------------------------------------------------------------

## Regla 5

No utilicen:

``` bash
git push --force
```

❌ **No lo necesitan.**

------------------------------------------------------------------------

<a id="seccion-22"></a>

# 22. 🆘 ¿Qué pasa si aparece un error?

No entren en pánico. 😂

Por ejemplo, si hacen:

``` bash
git push
```

y aparece un error, **no empiecen a ejecutar comandos al azar**.

Copien el mensaje completo del error y pregúntenle al compañero que
administra el proyecto o busquen ayuda antes de continuar.

------------------------------------------------------------------------

<a id="seccion-23"></a>

# 🧠 23. Entender Git en 30 segundos

Imaginen que están haciendo un trabajo en Word.

### Archivo del proyecto

``` text
📁 Proyecto
```

### `git add`

Le dicen a Git:

> "Estos cambios son los que quiero guardar."

### `git commit`

Le dicen:

> "Guarda una versión de mi trabajo."

### `git push`

Le dicen:

> "Sube esa versión a GitHub."

### `git pull`

Le dicen:

> "Descarga lo último que mis compañeros subieron."

Por eso:

``` text
git pull
    ↓
TRABAJAR
    ↓
git add .
    ↓
git commit
    ↓
git push
```

es el flujo que deben memorizar.
