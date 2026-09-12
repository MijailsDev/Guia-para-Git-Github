# 📘 Guía básica de Git + GitHub

## Para equipos principiantes --- Windows 11

> **Objetivo:** aprender a trabajar en equipo usando Git y GitHub de una
> manera sencilla, sin ramas ni procesos complicados.

------------------------------------------------------------------------

# 📑 Índice

1.  [Primero: ¿qué es Git y GitHub?](#1-primero-qué-es-git-y-github)
2.  [Cómo será el trabajo de
    ustedes](#2-cómo-será-el-trabajo-de-ustedes)
3.  [Parte 1 --- Crear una cuenta de
    GitHub](#3--parte-1--crear-una-cuenta-de-github)
4.  [Parte 2 --- Instalar Git en Windows
    11](#4--parte-2--instalar-git-en-windows-11)
5.  [Parte 3 --- Comprobar que Git
    funciona](#5--parte-3--comprobar-que-git-funciona)
6.  [Parte 4 --- Configurar Git](#6--parte-4--configurar-git)
7.  [Parte 5 --- Crear el
    repositorio](#7--parte-5--crear-el-repositorio)
8.  [Parte 6 --- Agregar a los
    integrantes](#8--parte-6--agregar-a-los-integrantes)
9.  [Parte 7 --- Descargar el
    proyecto](#9--parte-7--descargar-el-proyecto)
10. [Parte 8 --- Entrar al proyecto](#10--parte-8--entrar-al-proyecto)
11. [Parte 9 --- Abrir el proyecto](#11--parte-9--abrir-el-proyecto)
12. [Ahora viene lo más importante](#12--ahora-viene-lo-más-importante)
13. [Juan trabaja](#13--juan-trabaja)
14. [Guardar los cambios](#14--guardar-los-cambios)
15. [Preparar los cambios](#15--preparar-los-cambios)
16. [Crear el commit](#16--crear-el-commit)
17. [Subir a GitHub](#17--subir-a-github)
18. [Al día siguiente: María](#18--al-día-siguiente-maría)
19. [Y así durante meses](#19--y-así-durante-meses)
20. [La "chuleta" que deben tener
    todos](#20--la-chuleta-que-deben-tener-todos)
21. [Reglas de oro del grupo](#21--reglas-de-oro-del-grupo)
22. [¿Qué pasa si aparece un error?](#22--qué-pasa-si-aparece-un-error)
23. [Entender Git en 30 segundos](#23--entender-git-en-30-segundos)

------------------------------------------------------------------------

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

# 11. 🟢 PARTE 9 --- Abrir el proyecto

Si utilizan Visual Studio Code:

``` bash
code .
```

Se abrirá el proyecto.

Si `code .` no funciona, simplemente pueden abrir Visual Studio Code y
seleccionar la carpeta del proyecto.

------------------------------------------------------------------------

# 12. 🟡 AHORA VIENE LO MÁS IMPORTANTE

Supongamos que **hoy le toca trabajar a Juan**.

Antes de tocar absolutamente nada:

``` bash
git pull
```

Esto significa:

> "GitHub, dame la versión más reciente del proyecto."

------------------------------------------------------------------------

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

# 15. 🟢 Preparar los cambios

Escriban:

``` bash
git add .
```

El punto significa:

> "Agregar todos los cambios."

------------------------------------------------------------------------

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
