# DanielMayorov_ASIX1_0373_A00_IntroGitHub
## Primer repositorio del curso 2025-26 de ASIX 1
### Es mi primera toma de contacto con gitHub.
#### Soy Daniel Mayorov

Esto está en __negrita__
Esto está en **negrita** también 

Esto está en _cursiva_ 
Esto está en *cursiva*

**_TEXTO_** 
    
1. Elemento 1 
    * Elemento desordenado 1,1
    * Elemento desordenado 1,2
2. Elemento 2 
    * Elemento desordenado 2,1
    * Elemento desordenado 2,2
3. Elemento 3 

ASDasdASDAsDpOAFfAPSFMpasofmPAOSFMpoasmfpoASMFPOASMFPOAMSFPOMfpomsPOSMFPomPOMFPOpsofmPOASMFPAasdASDasdSDdsmd ALSM Kg kÑD Fñkjdnfañjkdnfñaksdjnfñaksdjnfañkdfnjañksdjnfañksjdnfakñsjdnfñaksjndfñkasjdnfñkajsdnfñkajsndfñkajsndfñakjsdnf

KASJNDjsdnLKSJDnksladnlkANDKJAsndKLASJDNkljsndKLJSDNkljnsdlkJNDkljndsklJNDKLjndLKJDNSKljsndKJNDkljsndLKJSNDlkjdnKJLNSDKLndJKLDSNljksdnLKJSDNlkjsndsKLJDSNlkjnsdJKASDNnsjdk

´´´html
<p> Esto es un párrafo<p>
´´´

[Esto es markdown](https://markdown.es/ "Texto adicional sobre el enlace")   

![Alt text](./imagen%201%20jpg.webp "Imagen de un archivo") 


| *Jugador* | *Equipo* | *Nombre* |
|-----:-----|------:-------|---------:-----------|
| 32 | Lakers | Magic Johnson |
| 33 | Celtics | Boston Celtics |
| 23 | Bulls | Michael "air" Jordan |

# Apuntes Completos: Git, Github y Fundamentos Web.
## 1. Conceptos Clave: Git vs. GitHub

Que es Git y que es Github?

* **Git:** Es un **sistema de control de versiones distribuido (DVCS)**. Es una herramienta que se ejecuta localmente en tu ordenador. Su trabajo es tomar "instantáneas" (llamadas *commits*) de tu código para guardar su historial, permitiéndote viajar en el tiempo entre diferentes versiones.
* **GitHub:** Es una **plataforma web** que aloja repositorios Git en la nube. Es un servicio que te permite almacenar tus copias de repositorios (remotas) y, sobre todo, **colaborar** con otras personas de manera organizada.

### El Flujo de Trabajo Básico de Git

Localmente, Git gestiona tres "áreas" principales:

1.  **Working Directory (Directorio de Trabajo):** Tu carpeta de proyecto con todos los archivos que estás editando.
2.  **Staging Area (Área de Preparación):** Una "zona de espera". Aquí es donde añades los cambios que quieres incluir en el próximo *commit*.
3.  **Local Repository (Repositorio Local):** La base de datos (`.git`) donde Git guarda permanentemente tus *commits* (el historial del proyecto).

El flujo es:
`Modificas archivos` -> `(git add)` -> `Los pasas a Preparación` -> `(git commit)` -> `Los guardas permanentemente en el Repositorio Local`

-----------------

### 2.1. Creación de la Cuenta de GitHub

1.  **Regístrate:** Ve a `github.com` y crea una cuenta gratuita. Este será tu "hogar" remoto.
2.  **Envía la URL:** La URL de tu perfil (ej. `https://github.com/tu-usuario`) es tu identidad pública.

### 2.2. Instalación de Herramientas Locales

* **1. Instalar Git:**
    * Ve a `git-scm.com` y descarga el instalador para tu sistema operativo.
    * Una vez instalado, abre un terminal (Git Bash en Windows, Terminal en Mac/Linux) y **configura tu identidad**. Esto es obligatorio y enlazará tus *commits* con tu nombre y correo.
        ```bash
        git config --global user.name "Tu Nombre"
        git config --global user.email "tu-correo@ejemplo.com"
        ```
    * **2. Instalar Visual Studio Code (VSC):**
    * Ve a `code.visualstudio.com`.
    * Es un editor de código moderno con una excelente integración con Git. Facilitará la visualización de cambios, la preparación (staging) y la validación (commit).

    * **3. Instalar GitHub Desktop (Opcional):**
    * Ve a `desktop.github.com`.
    * Es un cliente oficial de GitHub con una interfaz gráfica. Es muy útil si prefieres no usar el terminal para todo, ya que simplifica visualmente acciones como clonar, subir cambios o crear ramas.

    ---------------
# Git y Fundamentos Web


---


## 3. Empezando un Proyecto


Un **repositorio** (o *repo*) es simplemente una carpeta de proyecto que está siendo rastreada por **Git**.


---


### 3.1. Opción 1: Clonar un Repositorio Existente (la más común)


Clonar significa descargar una copia completa de un proyecto existente en **GitHub** (incluyendo todo su historial) a tu ordenador.


1. **Busca el botón verde “Code”** en el repositorio de GitHub y copia la URL HTTPS.
Ejemplo: `https://github.com/usuario/nombre-del-repo.git`


2. **Clona el repositorio**:
```bash
git clone https://github.com/usuario/nombre-del-repo.git
```


3. **Accede a la carpeta creada**:
```bash
cd nombre-del-repo
```
---

### 3.2. Opción 2: Crear un Repositorio Local Nuevo (desde cero)


Si estás empezando un proyecto nuevo desde tu ordenador:


1. **Crea una carpeta de proyecto**:
```bash
mkdir mi-proyecto
cd mi-proyecto
```


2. **Inicializa Git dentro de la carpeta**:
```bash
git init
```


3. **Haz tu primer commit**:
```bash
git add .
git commit -m "Commit inicial"
```


---


### 3.3. Sincronizar Cambios


Para bajar los cambios del repositorio remoto y fusionarlos con tu trabajo local, usa:
```bash
git pull
```


---


## 4. Colaboración: Ramas y Pull Requests


Esta es la parte más potente de **GitHub**.


---


### Rama (*Branch*)


Una **rama** es una línea de tiempo paralela de commits. La rama principal se llama `main`.
### Flujo de trabajo

1. Crea una rama nueva para cada tarea (ej. `feature/añadir-formulario`).
2. Trabaja y haz commits en esa rama.
3. Cuando termines, abre un **Pull Request (PR)**.
4. Un PR es una "solicitud para fusionar" tu rama con `main`.
5. Otras personas pueden revisar tu código, dejar comentarios y aprobarlo.
6. Una vez aprobado, fusiona el PR y tu trabajo se incorpora a `main`.

> **Importante:** Nunca deberías trabajar directamente sobre `main`.

# 1. Asegúrate de que estás en "main" y tienes la última versión
git checkout main
git pull

# 2. Crea y cámbiate a una nueva rama
git checkout -b feature/nuevo-formulario

# 3. Haz tu trabajo... (edita, 'git add', 'git commit')
# ...
git add .
git commit -m "Añade formulario de contacto"

# 4. Sube tu *nueva rama* a GitHub
git push -u origin feature/nuevo-formulario

# 5. Ve a GitHub: la plataforma detectará la nueva rama
#    y te mostrará un botón para "Crear un Pull Request".

---
# 5. Fundamentos Web


---


## 5.1. Markdown (`.md`)


Markdown es el lenguaje con el que se escriben archivos como los **README.md**.
Es una **sintaxis sencilla** para formatear texto plano, ideal para documentación, blogs o notas técnicas.


### Sintaxis básica de Markdown


```markdown
# Título H1
## Título H2
### Título H3


**Texto en negrita**
*Texto en cursiva*
`Código en línea`


- Elemento de lista 1
- Elemento de lista 2
- Sub-elemento 2.1
- Sub-elemento 2.2


> Esto es un texto citado (blockquote).


[Esto es un enlace a Google](https://www.google.com)


![Esto es una imagen](ruta/a/la/imagen.png)
```


### Bloques de código


Para escribir bloques de código de varias líneas, se utilizan tres tildes invertidas (```) seguidas del lenguaje opcional:


```html
<!-- Ejemplo de bloque de código HTML -->
<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8">
<title>Mi página</title>
</head>
<body>
<h1>Hola Mundo</h1>
<p>Esto es un párrafo de ejemplo.</p>
</body>
</html>
```


### Tips adicionales


- Puedes usar listas anidadas para organizar mejor tu información.
- Para enlaces relativos a tu proyecto, usa rutas locales: `[Archivo](docs/archivo.md)`.
- Las imágenes también pueden usar rutas locales o URLs absolutas.
- Markdown soporta tablas, listas de tareas y líneas horizontales (`---`) para estructurar el contenido.
- Mantén tu archivo `.md` limpio y organizado para facilitar la lectura.

### Flujo de trabajo típico


1. Crea una rama nueva para cada tarea (por ejemplo: `feature/añadir-formulario`).
2. Trabaja y haz commits en esa rama.
# HTML Semántico y la importancia de `index.html`

---

## Ejemplo básico de HTML

```html
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Título de la Página (aparece en la pestaña)</title>
    <link rel="stylesheet" href="style.css">
    <link rel="icon" href="favicon.ico">
</head>
<body>
    <header>
        <h1>Mi Sitio Web</h1>
    </header>

    <main>
        <section>
            <h2>Sobre mí</h2>
            <p>Esto es un párrafo con un <a href="contacto.html">enlace</a>.</p>
        </section>
    </main>

    <footer>
        <p>&copy; 2025 Mi Nombre.</p>
    </footer>
</body>
</html>
```

---

## HTML Semántico

Utiliza etiquetas como `<header>`, `<main>`, `<footer>`, `<nav>`, `<section>` y `<article>` para dar **significado** a la estructura.

### Importancia del HTML Semántico

**Esto es vital para:**

* **Accesibilidad:** los lectores de pantalla pueden interpretar mejor la página.
* **SEO:** los motores de búsqueda como Google entienden mejor el contenido de tu web.

**Ejemplos de uso semántico:**

* `<nav>` → barra de navegación
* `<section>` → sección del contenido
* `<article>` → artículo independiente
* `<footer>` → pie de página

**Consejos adicionales:**

* Mantén tu HTML limpio y organizado con sangrías consistentes.
* Usa comentarios: `<!-- comentario -->` para documentar tu código.
* Combina HTML con CSS para diseño y estilo y con JavaScript para interactividad.

---

## La importancia de `index.html`

El archivo `index.html` es fundamental en cualquier sitio web. Los servidores web buscan automáticamente este archivo cuando un usuario visita la URL raíz de un directorio (ej. `www.ejemplo.com`).

### Por qué es importante

* **Página de inicio:** `index.html` actúa como la puerta de entrada a tu sitio web, mostrando el contenido inicial que los usuarios verán.
* **Navegación:** Facilita que los visitantes accedan a otras páginas del sitio mediante enlaces desde esta página principal.
* **SEO y motores de búsqueda:** Tener un `index.html` correctamente estructurado ayuda a que los motores de búsqueda indexen tu sitio de manera eficiente.
* **Compatibilidad:** La mayoría de servidores y servicios de hosting esperan este archivo como punto de entrada.

### Buenas prácticas

* Mantén la estructura limpia: `<!DOCTYPE html>`, `<html>`, `<head>`, `<body>` correctamente anidados.
* Incluye títulos (`<title>`), meta etiquetas (`<meta>`), y enlaces a hojas de estilo o scripts.
* Usa contenido relevante y jerarquía clara de encabezados (`<h1>`, `<h2>`, `<h3>`).
* Optimiza el rendimiento: minimiza scripts y CSS innecesarios para que la página cargue rápido.
* Incluye accesibilidad: etiquetas semánticas y atributos como `alt` en imágenes.

### Ejemplo básico de `index.html`


```html
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Mi Página Principal</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <header>
        <h1>Bienvenido a Mi Sitio</h1>
    </header>

    <main>
        <section>
            <h2>Sobre Nosotros</h2>
            <p>Esta es la página de inicio donde presentamos nuestro sitio web.</p>
        </section>
    </main>

    <footer>
        <p>&copy; 2025 Mi Sitio Web.</p>
    </footer>
</body>
</html>

---

### 5. Fundamentos Web

### ¿Qué es HTML?

* HTML significa **HyperText Markup Language**.
* Es el lenguaje estándar para crear la **estructura y contenido** de una página web.
* **No es un lenguaje de programación**, sino un lenguaje de marcado (descriptivo).
* Actúa como el "esqueleto" de un sitio web.
* Define elementos como: títulos, párrafos, enlaces, imágenes, listas, tablas, etc.

### Estructura básica de un documento HTML

```html
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Título de la Página (aparece en la pestaña)</title>
    
    <link rel="stylesheet" href="style.css">
    <link rel="icon" href="favicon.ico">
</head>
<body>
    <header>
        <h1>Mi Sitio Web</h1>
    </header>

    <main>
        <section>
            <h2>Sobre mí</h2>
            <p>Esto es un párrafo con un <a href="contacto.html">enlace</a>.</p>
        </section>
    </main>

    <footer>
        <p>&copy; 2025 Mi Nombre.</p>
    </footer>
</body>
</html>

## La importancia de `index.html`

* Es el **punto de entrada principal** de un sitio web.
* Los servidores web lo buscan automáticamente cuando un usuario visita la raíz de un dominio (ej. `www.ejemplo.com`).
* Actúa como la **página de inicio** o portada del sitio.

### ¿Por qué es importante?

* **Página de inicio:** Es la primera página que ven los usuarios.
* **Navegación:** Suele contener los enlaces a otras secciones.
* **SEO:** Ayuda a los motores de búsqueda a indexar el sitio.
* **Compatibilidad:** Es el archivo estándar que esperan los servidores y hostings.
* **Profesionalismo:** Un sitio sin `index.html` se considera incompleto.

### Buenas prácticas

* Mantén la estructura limpia: `<!DOCTYPE html>`, `<html>`, `<head>`, `<body>` correctamente anidados.
* Incluye títulos (`<title>`), meta etiquetas (`<meta>`), y enlaces a hojas de estilo o scripts.
* Usa contenido relevante y jerarquía clara de encabezados (`<h1>`, `<h2>`, `<h3>`).
* Optimiza el rendimiento: minimiza scripts y CSS innecesarios para que la página cargue rápido.
* Incluye accesibilidad: etiquetas semánticas y atributos como `alt` en imágenes.