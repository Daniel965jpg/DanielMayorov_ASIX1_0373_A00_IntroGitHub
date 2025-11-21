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


| Jugador | Equipo  | Nombre               |
| ------- | ------- | -------------------- |
| 32      | Lakers  | Magic Johnson        |
| 33      | Celtics | Boston Celtics       |
| 23      | Bulls   | Michael "Air" Jordan |


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

1.  **Asegúrate de que estás en "main" y tienes la última versión**
    ```bash
    git checkout main
    git pull
    ```

2.  **Crea y cámbiate a una nueva rama**
    ```bash
    git checkout -b feature/nuevo-formulario
    ```

3.  **Haz tu trabajo... (edita, 'git add', 'git commit')**
    ```bash
    # ...
    git add .
    git commit -m "Añade formulario de contacto"
    ```

4.  **Sube tu *nueva rama* a GitHub**
    ```bash
    git push -u origin feature/nuevo-formulario
    ```

5.  **Ve a GitHub: la plataforma detectará la nueva rama y te mostrará un botón para "Crear un Pull Request".**

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
```

---

### 5. Fundamentos Web

---

### 5.2. ¿Qué es HTML?

* HTML (**HyperText Markup Language**) es el **lenguaje estándar de marcado**.
* Se utiliza para **crear la estructura y el contenido** de una página web.
* No es un lenguaje de programación, sino un **lenguaje descriptivo** que indica al navegador cómo mostrar el contenido.
* Actúa como el **esqueleto** de cualquier sitio web.
* Define elementos como: Títulos (`<h1>` a `<h6>`), Párrafos (`<p>`), Enlaces (`<a>`), Imágenes (`<img>`), Listas (`<ul>`, `<ol>`, `<li>`), Tablas (`<table>`, `<tr>`, `<td>`) y Formularios (`<form>`, `<input>`, `<button>`).

---

### Estructura básica de un documento HTML

```html
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Título de la Página</title>
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
## Organización y Legibilidad

* El código debe ser **legible** para otros humanos, no solo para el navegador.
* **Comentarios:** Se usan para dejar notas en el código que el navegador ignorará. La sintaxis es ``.
* **Sangrado (Indentación):** Se usa para ver claramente qué etiquetas están dentro de otras (anidación) y facilitar la lectura.
* **Organización de Archivos:** Se recomienda organizar el proyecto en carpetas (ej. `/css` para estilos, `/imatges` para imágenes).
* **`index.html`:** El archivo HTML principal de la web debe llamarse `index.html`, ya que es el nombre que los servidores buscan por defecto.

## Elementos y Atributos

---

### Tipos de Elementos

* **Elementos de Bloque (Block):** Ocupan todo el ancho disponible y empiezan en una nueva línea (ej. `<p>`, `<h1>`, `<div>`).
* **Elementos de Línea (Inline):** Ocupan solo el espacio necesario y fluyen dentro del texto (ej. `<a>`, `<strong>`, `<img>`).

---

### Atributos Genéricos

* Los atributos proporcionan **información adicional** a una etiqueta.
* **`id`:** Identificador **único** para un elemento en la página.
* **`class`:** Nombre de clase para agrupar múltiples elementos (muy usado para CSS).
* **`style`:** Se usa para aplicar estilos CSS directamente (inline).
* **`title`:** Muestra un texto (tooltip) cuando el ratón pasa por encima.
* **`lang`:** Especifica el idioma del contenido (ej. `<html lang="ca">`).

---

## Etiquetas de Texto Principales

* **`<h1>` a `<h6>`:** Encabezados o Títulos. `<h1>` es el más importante y `<h6>` el menos importante. 
* **`<p>`:** Define un párrafo. 
* **`<em>`:** Para dar énfasis (normalmente se ve en cursiva). 
* **`<strong>`:** Para dar una énfasis fuerte (normalmente se ve en negrita). 
* **`<br/>`:** Inserta un salto de línea forzado. 
* **`<hr/>`:** Crea una línea horizontal separadora. 
* **`<blockquote>`:** Se usa para citar un bloque de texto largo.
* **`<div>`:** Contenedor genérico de **bloque**. Se usa para agrupar y estructurar secciones.
* **`<span>`:** Contenedor genérico en **línea**. Se usa para agrupar texto o elementos dentro de un bloque.

### ⚠️ Etiquetas "antiguas" (Evitar)

* No se deben usar etiquetas como `<b>` (negrita) o `<i>` (cursiva), ya que solo definen presentación y no estructura.
* Para eso se usa CSS. En su lugar, usa `<strong>` y `<em>` que tienen valor semántico (de significado).

---
##  Enlaces e Imágenes

---

### Enlaces (Hipervínculos)

* Se crean con la etiqueta `<a>` (de ancla) y el atributo `href` que indica el destino.
* **Enlaces externos:** Apuntan a otra web (ej. `<a href="https://google.com">Google</a>`).
* **Enlaces locales:** Apuntan a otra página de tu propio sitio (ej. `<a href="contacto.html">Contacto</a>`).
* **Enlaces tipo ancla (internos):** Permiten navegar a otra parte *de la misma página*.
    * Primero se crea el ancla con un `id` (ej. `<h2 id="seccion1">Sección 1</h2>`).
    * Luego se enlaza a ella usando `#` (ej. `<a href="#seccion1">Ir a Sección 1</a>`).

---

### Imágenes

* Se insertan con la etiqueta `<img>`, que es un elemento en línea y no tiene etiqueta de cierre.
* **`src`:** Atributo obligatorio que indica la **ruta** de la imagen (URL o archivo local).
* **`alt`:** Atributo obligatorio que provee un **texto alternativo** si la imagen no se puede cargar.
* **Ejemplo:** `<img src="media/logo.png" alt="Logo de la web">`.
* Una imagen puede ser un enlace si se envuelve en una etiqueta `<a>`.

---
## 📊 Tablas

---

* Se usan para mostrar **información tabular** (datos en filas y columnas).
* **Importante:** No se deben usar tablas para la maquetación de la página (para eso se usan `<div>` y CSS).
* **`<table>`:** El contenedor principal de la tabla.
* **`<tr>`:** (Table Row) Define una **fila**.
* **`<td>`:** (Table Data) Define una **celda** de datos.
* **`<th>`:** (Table Header) Define una celda de **encabezado** (resaltada).
* **`<thead>`, `<tbody>`, `<tfoot>`:** Etiquetas semánticas para agrupar las filas de la cabecera, el cuerpo y el pie de la tabla. 
* **`colspan="2"`:** Hace que una celda se expanda para ocupar 2 columnas.
* **`rowspan="2"`:** Hace que una celda se expanda para ocupar 2 filas.

---

## 📋 Formularios

---

* Se usan para **interactuar con el usuario** y permitirle enviar información.
* El formulario completo se envuelve en la etiqueta **`<form>`**.

### Atributos de `<form>`

* **`action`:** La URL (script o página) a la que se **enviarán los datos**.
* **`method`:** El método HTTP para enviar los datos.
    * **`get`:** Envía los datos en la URL (visibles, ej. `...php?nom=Anna`).
    * **`post`:** Envía los datos de forma oculta en la cabecera HTTP.

### Controles de Formulario Comunes

* **`name`:** Atributo **crucial**. Es el nombre que identifica al dato que se envía (ej. `name="nom"`).
* **`<label>`:** Etiqueta de texto para un control (mejora la accesibilidad).
* **`<fieldset>` y `<legend>`:** Agrupan controles relacionados (`<fieldset>`) con un título (`<legend>`).
* **`<input type="text">`:** Campo de texto de una línea.
* **`<input type="password">`:** Campo de contraseña (oculta el texto).
* **`<input type="radio">`:** Botón de opción (permite seleccionar solo uno de un grupo).
* **`<input type="checkbox">`:** Casilla de verificación (permite seleccionar varios).
* **`<select>` y `<option>`:** Crean una lista desplegable.
* **`<textarea>`:** Área para texto de múltiples líneas.
* **`<input type="submit">`:** Botón que **envía** el formulario.
* **`<input type="reset">`:** Botón que **borra** los datos del formulario.

---

### 5.3. Validador HTML del W3C

El W3C (World Wide Web Consortium) es el organismo que define los estándares oficiales de HTML. Para asegurarte de que tu código HTML es correcto, profesional y sigue estos estándares, debes utilizar su validador en línea.

Usar esta herramienta es fundamental por varias razones:

* **Encuentra errores:** Detecta sintaxis incorrecta, como etiquetas mal cerradas (`<p>...</div>`), atributos obsoletos o elementos obligatorios que faltan (como el atributo `alt` en las imágenes `<img>`).
* **Mejora la compatibilidad (Cross-Browser):** Un HTML válido asegura que tu página se vea y funcione de manera similar en todos los navegadores (Chrome, Firefox, Safari, etc.).
* **Ayuda al SEO:** A los motores de búsqueda (como Google) les es más fácil entender y clasificar una página con código limpio y bien estructurado.
* **Base para la accesibilidad (A11y):** Un HTML semántico y válido es el primer paso para que las tecnologías de asistencia (como lectores de pantalla) puedan interpretar tu web correctamente.

### ¿Cómo se usa el validador?

El validador es una herramienta en línea gratuita a la que puedes acceder aquí:
**[validator.w3.org](https://validator.w3.org/)**



Tienes tres formas principales de comprobar tu código:

1.  **Validar por URI (URL):** Pegas la URL de tu sitio web si ya está publicado (ej. `https://www.ejemplo.com`).
2.  **Validar por subida de archivo (File Upload):** Subes tu archivo `index.html` directamente desde tu ordenador.
3.  **Validar por entrada directa (Direct Input):** Copias todo tu código HTML y lo pegas directamente en la caja de texto del validador.

> **Objetivo:** Tu meta debería ser que el validador muestre un mensaje verde de éxito y reporte **"0 Errors"**. No te preocupes tanto por los "Warnings" (advertencias) al principio, pero los **"Errors" (errores) son obligatorios de corregir.**

---

## 6. Publicar tu Sitio Web con GitHub Pages

**GitHub Pages** es un servicio gratuito de GitHub que te permite alojar y publicar sitios web estáticos (es decir, hechos solo con HTML, CSS y JavaScript) directamente desde tu repositorio.

Es la forma más rápida de poner tu proyecto en línea y compartirlo con el mundo.

### Cómo activar GitHub Pages

El proceso es muy sencillo y se hace desde la configuración de tu repositorio:

1.  En tu repositorio de GitHub, ve a la pestaña principal y haz clic en **"Settings"** (Configuración).
    
2.  En el menú lateral izquierdo, busca y haz clic en **"Pages"**.
3.  En la sección "Build and deployment" (Construcción y despliegue), mira la opción **"Source"** (Fuente).
4.  Asegúrate de que esté seleccionada la opción **"Deploy from a branch"** (Desplegar desde una rama).
5.  En el menú desplegable, elige la rama que contiene tu código final (normalmente será **`main`**).
6.  Deja la carpeta como `/(root)` y haz clic en **"Save"** (Guardar).

¡Y ya está! Después de unos segundos (a veces puede tardar un minuto), GitHub procesará tus archivos y publicará tu sitio.

> **Importante:** Tu página estará disponible públicamente en una URL con este formato. Podrás ver el enlace exacto en la misma página de "Settings" una vez que se publique.
>
> `https://tu-usuario.github.io/nombre-del-repositorio/`
>
> (Recuerda que para que esto funcione, tu archivo HTML principal **debe llamarse `index.html`**).

---

## 3. Otras Herramientas Útiles

### Font Awesome (Iconos)

Es un popular conjunto de herramientas de iconos y fuentes basado en CSS. Te permite añadir fácilmente miles de iconos vectoriales (escalables y personalizables con CSS) a tu página web con una simple línea de código.

> **Ejemplo de uso:**
> ```html
> <i class="fas fa-rocket"></i>
> ```
> (Esto mostraría un icono de cohete 🚀).

### Favicons

Un **favicon** (icono de favorito) es el pequeño icono (normalmente de 16x16 o 32x32 píxeles) que aparece en la pestaña del navegador, justo al lado del título de la página.


* **¿Para qué sirve?** Es clave para la imagen de marca (*branding*) y la usabilidad, ya que ayuda a los usuarios a identificar rápidamente tu pestaña entre muchas otras.

### ¿Cómo crearlos?

1.  Crea una versión simplificada y cuadrada de tu logo.
2.  Guárdala como `.png` o utiliza un generador en línea (como `favicon.io`) para crear un archivo `.ico` (que ofrece mayor compatibilidad).
3.  Añade el archivo al directorio de tu proyecto.
4.  Enlázalo dentro de la etiqueta `<head>` de tu HTML:

```html
<head>
  <meta charset="UTF-8">
  <title>Título de mi Página</title>
  
  <link rel="icon" href="favicon.ico" type="image/x-icon">
  <link rel="shortcut icon" href="favicon.ico" type="image/x-icon">
</head>
```

# Apuntes de **CSS**  (Hojas de Estilo en Cascada)

![CSS](css.png) 
## Antes de nada, **que es CSS?** 

Es un lenguaje de estilo que se utiliza para controlar la presentación, el diseño y la apariencia de documentos escritos en un lenguaje de marcado como HTML 
En resumen, es un tipo de lenguaje que se utiliza para darle estilo a nuestro código hecho en *HTML* a través de un archivo adicional en **Visual Studio code**

## 1. Origen y Evolución
* **Problema inicial:** En los inicios, HTML era solo estructura. Al querer mejorar el diseño, el código se ensuciaba mezclando contenido y presentación.
* **Solución:** Nace CSS para separar la **estructura** (HTML) de la **presentación** (CSS). <br>
    * *HTML*: Define qué es cada cosa (título, vínculo)
    * *CSS*: Define cómo se ve (color, espacio posición)
* **Empezó** en el 1996-1998 y se publicó el primer contenido CSS en ese año.
<br>
Los navegadores cuando van apareciendo nuevas funciones las van implementando poco a poco. <br>

**Ejemplo:**
<br>
* **Microsoft Edge** En su día (2020), antes de aplicar su nuevo motor, carecía de soporte para efectos gráficos
<br> 
Mientras que **Google Chome** Utiliza el motor *Blink* y suele marcar la pauta en nuevos estandáres. Tiene funciones con mejor adaptabilidad en el día a día. <br>
Aquí podemos **ver y notar las diferencias** del porque en un navegador carga con mayor rapidez o mayor sencillez algunos detalles de diferentes páginas (por ejemplo).

## 2. Ventajas e Inconvenientes

* ### Ventajas
    * Código más fácil de leer.
    * Mayor potencia de diseño que el HTML antiguo.
    * Lenguaje sencillo.
    * **Reutilización**: Una misma hoja de estilo sirve para muchas páginas HTML.
    * **Adaptabilidad**: Puedes definir hojas distintas según el dispositivo (pantalla ordenador vs impresión).

* ## Inconveniente principal

    * Inconsistencia entre navegadores: Recordando la mención anterior, no todos los navegadores interpretan el código igual ni cumplen con los estándares al 100%, obligando a crear *"parches"* para navegadores específicos.


## 3.  Formas de aplicar CSS

Existen 3 formas principales de aplicar estilos, aunque en el siguiente ejemplo práctico **solo veremos dos de ellas**:

1.  **Estilo "Externo"** (Recomendado).
2.  **Estilo "Interno"** (En la cabecera).
3.  **Estilo "Inline"** (En línea).

### Ejemplo Práctico 

![IntroduccionCSS](css2.png)

En esta captura de código podemos ver dos de las formas mencionadas arriba en el mismo archivo:

* **Estilo Externo (Flecha Superior):**
    Vemos la etiqueta `<link>` dentro del `<head>`. Esta línea conecta el HTML con el archivo `estilo.css`.
    > **Nota:** Se coloca en el head para evitar que la web se vea "rota" mientras carga.

* **Estilo Inline (Flecha Inferior):**
    Vemos el atributo `style="..."` dentro de la etiqueta `<p>`.
    * *Ejemplo:* `<p style="color: green;">`
    Aquí se está aplicando un color y tamaño específico solo para ese párrafo.
    > **Ojo:** Al ser "Inline", este estilo **tiene prioridad** y sobrescribirá lo que diga el archivo externo.

* **Que falta?**
    En esta imagen **NO** se está usando el **Estilo Interno** (etiquetas `<style>` en el head).

### Demostración: Reglas Generales vs. Excepciones

"El estilo.css dice una cosa y el resultado otra, veremos porque.

![Código CSS](cass4.png)

![Resultado en Navegador](css3.png)

**¿Qué está pasando aquí?**

1.  **La Regla General (El archivo externo):**
    En nuestro archivo CSS (imagen izquierda), hemos dictado una norma para toda la web: *"Todos los párrafos (`p`) deben ser de color rojo"*.
    * *Resultado:* El primer párrafo obedece y se pinta de rojo.

2.  **La Excepción (El estilo en línea):**
    El último párrafo, sin embargo, aparece en **verde**.
    Esto ocurre porque el estilo en línea (`style="..."`) actúa como una excepción directa. Aunque la norma general diga "rojo", la instrucción específica en la etiqueta HTML dice "verde".

> **Conclusión:**
> El navegador siempre hará caso a la instrucción **más cercana** al elemento.
> * El archivo CSS está "lejos" (es una norma global).
> * El atributo `style` está "pegado" al texto (es una orden directa).
>
> Por eso: **Orden directa (Inline) > Norma global (Externo).**

--- 
## Sistema de Puntos

Cuando hay un conflicto (como el rojo y verde de las capturas) el navegador suma puntos. **Gana el que más tenga**

### 1. La Tabla de Puntuación
* **1000 puntos:** Estilo Inline (`style="..."`). 
* **100 puntos:** ID (`#header`).
* **10 puntos:** Clases (`.menu`, `:hover`).
* **1 punto:** Elementos (`h1`, `div`, `p`).
* **0 puntos:** Universal (`*`).    

### 2. Las cuentas claras 

![Código CSS](css2.png)
![Código CSS](cass4.png)
![Resultado](css3.png)

* **El CSS externo (Rojo):** Es una etiqueta `p` -> **1 punto**.
* **El HTML inline (Verde):** Es un atributo `style` -> **1000 puntos**.

**Resultado:** Gana el **VERDE** por una diferencia enorme (1000 > 1).

---

### 3. Notas Extra
* **`!important`:** Es el "botón nuclear". Si lo usas, gana a todos los puntos anteriores.
* **Herencia:** Es lo más débil. Cualquier regla directa (aunque valga 1 punto) gana a lo heredado del padre.

##  Sintaxis Básica: Comentarios

Los comentarios son notas para ti (el programador) que **el navegador ignora** completamente (no afectan al diseño).

* **Símbolos:** Se escriben entre `/*` y `*/`.
* **Característica:** En CSS **solo existen comentarios de bloque**, por lo que pueden ocupar una o varias líneas sin problema.

```css
/* Este es un comentario explicativo
   que no afectará a la web 
*/

p {
    color: red; /* Comentario en la misma línea */
}