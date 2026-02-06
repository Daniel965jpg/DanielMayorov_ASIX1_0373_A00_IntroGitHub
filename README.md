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
| 32      | Lakers  | Maegic Johnson        |
| 33      | Celtics | Boston Celtics       |
| 23      | Bulls   | Michael "Air" Jordan |


# Apuntes Completos: Git, Github y Fundamentos Web.

## 1. Conceptos Clave: Git vs. GitHub


![Imágen Github](/html/github.png)

**¿Qué diferencia hay entre ellos?**

**Git:** Es un **sistema de control de versiones distribuido**. Funciona localmente en tu ordenador. Su trabajo es guardar el código para registrar todo el historial de cambios.

**GitHub:** Es una **plataforma web** que aloja repositorios Git en la nube. Sirve para guardar copias remotas de tu código y **colaborar** con otras personas.

### El Flujo de Trabajo Básico de Git


![Imágen Git](/html/git.png)

Git organiza el trabajo en tres áreas locales:

1. **Working Directory** (Directorio de Trabajo): Es la carpeta de tu proyecto con los archivos que estás editando en ese momento.

2. **Staging Area** (Área de Preparación): Es una zona de espera. Aquí añades los archivos modificados que quieres incluir en el siguiente *commit*.

3. **Local Repository** (Repositorio Local): Es la base de datos interna (*.git*) donde se guardan permanentemente los cambios confirmados.

**Esquema del flujo:**

Modificar archivos -> git add -> Área de Preparación -> git commit` -> Repositorio Local

---

### 2.1. Creación de la Cuenta de GitHub

![Creación de cuenta GitHub](html/crear-cuenta-git.jpg)

1. **Regístrate:** Vamos a *github.com* y creamos una cuenta gratuita. Este será nuestro espacio para guardar repositorios en la nube.

2. **Envía la URL:** La URL de tu perfil (ej. *https://github.com/tu-usuario*) es tu identidad pública para compartir código.

### 2.2. Instalación de Herramientas Locales

**1. Instalar Git:**
Ve a *git-scm.com* y descarga el instalador.
Abre un terminal y **configura tu identidad** (obligatorio para firmar tus *commits*):
    
git config --global user.name "Tu Nombre"
git config --global user.email "tu-correo@ejemplo.com"


**2. Instalar Visual Studio Code (VSC):**

![Imágen VisalStudio](/html/visualstudio.jpg)

Ir a code.visualstudio.com.

Es un editor de código que se integra con Git. Facilita ver cambios y realizar *commits* sin usar siempre la terminal.


# Git y Fundamentos Web
## 3. Empezando un Proyecto

Un **repositorio** (o *repo*) es simplemente una carpeta de proyecto que está siendo rastreada por **Git** así en un futuro podremos hacer un mejor manejo de ello.


### 3.1. Opción 1: Clonar un Repositorio Existente (la más común)

![Imágen Clonar Respositorio](/html/clonar-repositorio.png)

Clonar significa descargar una copia completa de un proyecto existente en **GitHub** (incluyendo todo su historial) a tu ordenador.

1. **Busca el botón verde “Code”** en el repositorio de GitHub y copia la URL HTTPS.
Ejemplo: `https://github.com/usuario/nombre-del-repo.git`


2. **Clona el repositorio**:
git clone https://github.com/usuario/nombre-del-repo.git

3. **Accede a la carpeta creada**:

cd nombre-del-repo

### 3.2. Opción 2: Crear un Repositorio Local Nuevo (desde cero)

![Imágen Clonar Respositorio](/html/añadir-repositorio.png)

Si estás empezando un proyecto nuevo desde tu ordenador:

1. **Crea una carpeta de proyecto**:
mkdir mi-proyecto
cd mi-proyecto

2. **Inicializa Git dentro de la carpeta**:

git init

3. **Haz tu primer commit**:
git add .
git commit -m "Commit inicial"


### 3.3. Sincronizar Cambios

Para bajar los cambios del repositorio remoto y fusionarlos con tu trabajo local, usa:

*git pull*


## 4. Colaboracion: Ramas y Pull Requests

Esta es la parte mas potente de **GitHub**. Permite trabajar en equipo sin romper el codigo principal del proyecto.

![Imágen Branch](/html/brach-git.png)

### Conceptos Basicos

**Rama (Branch):** Es una linea de tiempo paralela de *commits*. La rama principal se llama main.

**Pull Request (PR):** Es una "solicitud para fusionar" tu rama con la rama `main`. Permite que otros revisen tu codigo antes de incluirlo.

# 5. Fundamentos Web

## 5.1. Markdown (`.md`)

![Imágen Markdown](/html/markdown-repo1.png)

Markdown es el lenguaje con el que se escriben archivos como los **README.md**.
Es una **sintaxis sencilla** para formatear texto plano, ideal para documentación, blogs o notas técnicas.


### Sintaxis básica de Markdown

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

### Flujo de trabajo típico


1. Crea una rama nueva para cada tarea

2. Se Trabaja y se hacen commits en esa rama.
# HTML Semántico y la importancia de *index.html*

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

## HTML Semántico

Utiliza etiquetas como `<header>`, `<main>`, `<footer>`, `<nav>`, `<section>` y `<article>` para dar **significado** a la estructura.

### Importancia del HTML Semántico

**Accesibilidad:** los lectores de pantalla pueden interpretar mejor la página.

**SEO:** los motores de búsqueda como Google entienden mejor el contenido de tu web.

**Ejemplos de uso semántico:**

`<nav>` → barra de navegación
`<section>` → sección del contenido
`<article>` → artículo independiente
`<footer>` → pie de página


* Mantener tu HTML limpio y organizado.

* Usa comentarios: `<!-- comentario -->` para documentar tu código, ya sea para acordarte o facilitar a tus compañeros leer con mayor facilidad el código

## La importancia de `index.html`

![Index HTML](/html/index-html.png)

El archivo *index.html* es fundamental en cualquier sitio web. Los servidores web buscan automáticamente este archivo cuando un usuario visita la URL raíz de un directorio (ej. `www.ejemplo.com`).

### Por qué es importante

**Página de inicio:** index.html actúa como la puerta de entrada a tu sitio web, mostrando el contenido inicial que los usuarios verán.

**Navegación:** Facilita que los visitantes accedan a otras páginas del sitio mediante enlaces desde esta página principal.

**SEO y motores de búsqueda:** Tener un index.html correctamente estructurado ayuda a que los motores de búsqueda indexen tu sitio de manera eficiente.

**Compatibilidad:** La mayoría de servidores y servicios de hosting esperan este archivo como punto de entrada.

## 5. Fundamentos Web

### 5.2. ¿Qué es HTML?

![Logo HTML](/html/html-logo.jpg)

* HTML (**HyperText Markup Language**) es el **lenguaje estándar de marcado**.

* Se utiliza para **crear la estructura y el contenido** de una página web.

* No es un lenguaje de programación, sino un **lenguaje de marcas** que indica al navegador cómo mostrar el contenido.

* Actúa como el **esqueleto** de cualquier sitio web.
* Define elementos como: Títulos (`<h1>` a `<h6>`), Párrafos (`<p>`), Enlaces (`<a>`), Imágenes (`<img>`), Listas (`<ul>`, `<ol>`, `<li>`), Tablas (`<table>`, `<tr>`, `<td>`) y Formularios (`<form>`, `<input>`, `<button>`).

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

## Elementos y Atributos
### Tipos de Elementos

* **Elementos de Bloque (Block):** Ocupan todo el ancho disponible y empiezan en una nueva línea (ej. `<p>`, `<h1>`, `<div>`).

* **Elementos de Línea (Inline):** Ocupan solo el espacio necesario y fluyen dentro del texto (ej. `<a>`, `<strong>`, `<img>`).

### Atributos Genéricos

![Explicación breve deatributos genéricos](/html/atributo-generico.webp)

Los atributos proporcionan **información adicional** a una etiqueta.

**id:** Identificador **único** para un elemento en la página.

**`class`:** Nombre de clase para agrupar múltiples elementos (muy usado para CSS).

**`style`:** Se usa para aplicar estilos CSS directamente (inline).

**`title`:** Muestra un texto (tooltip) cuando el ratón pasa por encima.

**`lang`:** Especifica el idioma del contenido (ej. `<html lang="ca">`).


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

### Etiquetas "antiguas" (Evitar)

* No se deben usar etiquetas como `<b>` (negrita) o `<i>` (cursiva), ya que solo definen presentación y no estructura.

* Para eso se usa CSS. En su lugar, usa `<strong>` y `<em>` que tienen valor semántico (de significado).

##  Enlaces e Imágenes
### Enlaces (Hipervínculos)

![Explicación a href](/html/a-hred.png)

Se crean con la etiqueta `<a>` (de ancla) y el atributo `href` que indica el destino.

* **Enlaces externos:** Apuntan a otra web (ej. `<a href="https://google.com">Google</a>`).

**Enlaces locales:** Apuntan a otra página de tu propio sitio (ej. `<a href="contacto.html">Contacto</a>`)
.
**Enlaces tipo ancla (internos):** Permiten navegar a otra parte *de la misma página*.

Primero se crea el ancla con un `id` (ej. `<h2 id="seccion1">Sección 1</h2>`).
Luego se enlaza a ella usando `#` (ej. `<a href="#seccion1">Ir a Sección 1</a>`).

### Imágenes

![Explicación etiqueta img resumida](/html/etiqueta-img.png)

Se insertan con la etiqueta `<img>`, que es un elemento en línea y no tiene etiqueta de cierre.

**src:** Atributo obligatorio que indica la **ruta** de la imagen (URL o archivo local).

**alt:** Atributo obligatorio que provee un **texto alternativo** si la imagen no se puede cargar.

**Ejemplo:** `<img src="media/logo.png" alt="Logo de la web">`.

* Una imagen puede ser un enlace si se envuelve en una etiqueta `<a>`.


## Tablas

![Explicación a href](/html/tablas-html.jpg)

* Se usan para mostrar **información tabular** (datos en filas y columnas).

* **Importante:** No se deben usar tablas para la maquetación de la página (para eso se usan `<div>` y CSS).

**`<table>`:** El contenedor principal de la tabla.
**`<tr>`:** (Table Row) Define una **fila**.

**`<td>`:** (Table Data) Define una **celda** de datos.

**`<th>`:** (Table Header) Define una celda de **encabezado** (resaltada).

**`<thead>`, `<tbody>`, `<tfoot>`:** Etiquetas semánticas para agrupar las filas de la cabecera, el cuerpo y el pie de la tabla. 

**`colspan="2"`:** Hace que una celda se expanda para ocupar 2 columnas.

**`rowspan="2"`:** Hace que una celda se expanda para ocupar 2 filas.


## Formularios

![Imagen de un forulario en HTML](/html/formularios-html.png)

* Se usan para **interactuar con el usuario** y permitirle enviar información.

El formulario completo se envuelve en la etiqueta **`<form>`**.

### Atributos de `<form>`

![Explicación a <form> y diferentes tipos](/html/atributos-form.jpg)

**`action`:** La URL (script o página) a la que se **enviarán los datos**.

**`method`:** El método HTTP para enviar los datos.

**`get`:** Envía los datos en la URL (visibles, ej. `...php?nom=Anna`).

**`post`:** Envía los datos de forma oculta en la cabecera HTTP.

### Controles de Formulario Comunes

![Explicación breve atributos](/html/input-label.jpg)

**`name`:** Atributo **crucial**. Es el nombre que identifica al dato que se envía (ej. `name="nom"`).

**`<label>`:** Etiqueta de texto para un control (mejora la accesibilidad).

**`<fieldset>` y `<legend>`:** Agrupan controles relacionados (`<fieldset>`) con un título (`<legend>`).

**`<input type="text">`:** Campo de texto de una línea.

**`<input type="password">`:** Campo de contraseña (oculta el texto).

**`<input type="radio">`:** Botón de opción (permite seleccionar solo uno de un grupo).

**`<input type="checkbox">`:** Casilla de verificación (permite seleccionar varios).

**`<select>` y `<option>`:** Crean una lista desplegable.

**`<textarea>`:** Área para texto de múltiples líneas.

**`<input type="submit">`:** Botón que **envía** el formulario.

**`<input type="reset">`:** Botón que **borra** los datos del formulario.


### 5.3. Validador HTML del W3C

![Imágen Validador](/html/validador.png)

El W3C (World Wide Web Consortium) es el organismo que define los estándares oficiales de HTML. Para asegurarte de que tu código HTML es correcto, profesional y sigue estos estándares, debes utilizar su validador en línea.

Usar esta herramienta es fundamental por varias razones:

**Encuentra errores:** Detecta sintaxis incorrecta, como etiquetas mal cerradas (`<p>...</div>`), atributos obsoletos o elementos obligatorios que faltan (como el atributo `alt` en las imágenes `<img>`).

**Mejora la compatibilidad (Cross-Browser):** Un HTML válido asegura que tu página se vea y funcione de manera similar en todos los navegadores (Chrome, Firefox, Safari, etc.).

**Ayuda al SEO:** A los motores de búsqueda (como Google) les es más fácil entender y clasificar una página con código limpio y bien estructurado.

### ¿Cómo se usa el validador?

El validador es una herramienta en línea gratuita a la que puedes acceder aquí:
**[validator.w3.org](https://validator.w3.org/)**

Tienes tres formas principales de comprobar tu código:

1.  **Validar por URI (URL):** Pegas la URL de tu sitio web si ya está publicado (ej. `https://www.ejemplo.com`).

2.  **Validar por subida de archivo (File Upload):** Subes tu archivo `index.html` directamente desde tu ordenador.

3.  **Validar por entrada directa (Direct Input):** Copias todo tu código HTML y lo pegas directamente en la caja de texto del validador.


## 6. Publicar tu Sitio Web con GitHub Pages

**GitHub Pages** es un servicio gratuito de GitHub que te permite alojar y publicar sitios web estáticos (es decir, hechos solo con HTML, CSS y JavaScript) directamente desde tu repositorio.

Es la forma más rápida de poner tu proyecto en línea y compartirlo con el mundo.


### Cómo activar GitHub Pages

El proceso es muy sencillo y se hace desde la configuración de tu repositorio:

![Imágen Pages 1](/html/github-pages1.png)

1.  En tu repositorio de GitHub, ve a la pestaña principal y haz clic en **"Settings"** (Configuración).
    
2.  En el menú lateral izquierdo, busca y haz clic en **"Pages"**.

![Imágen Pages 2](/html/github-pages2.png)

3.  En la sección "Build and deployment" (Construcción y despliegue), mira la opción **"Source"** (Fuente).

4.  Asegúrate de que esté seleccionada la opción **"Deploy from a branch"** (Desplegar desde una rama).

5.  En el menú desplegable, elige la rama que contiene tu código final (normalmente será **`main`**).

6.  Deja la carpeta como `/(root)` y haz clic en **"Save"** (Guardar).

![Imágen Pages 3](/html/github-pages3.png)

Y ya está, después de unos segundos (a veces puede tardar un minuto), GitHub procesará tus archivos y publicará tu sitio.

![Imágen Pages 4](/html/github-pages4.png)

> **Importante:** La página estará disponible públicamente en una URL con este formato. Podrás ver el enlace exacto en la misma página de "Settings" una vez que se publique.

> `https://tu-usuario.github.io/nombre-del-repositorio/`

> (Para que funcione **debe llamarse `index.html`**).


## 3. Otras Herramientas Útiles

### Font Awesome (Iconos)

![Imágen Logo Fontawesome](/html/fontawesome.png)

Es un popular conjunto de herramientas de iconos y fuentes basado en CSS. Te permite añadir fácilmente miles de iconos vectoriales (escalables y personalizables con CSS) a tu página web con una simple línea de código.

**Ejemplo de uso:**
```
> <i class="fas fa-rocket"></i>
> (Esto mostraría un icono de cohete).
```

### Favicons

![Imágen Logo Favicon](/html/favicon.jpg)

Un **favicon** (icono de favorito) es el pequeño icono que aparece en la pestaña del navegador, justo al lado del título de la página.


**¿Para qué sirve?** Es clave para la imagen de marca y la usabilidad, ya que ayuda a los usuarios a identificar rápidamente tu pestaña entre muchas otras.

### Creación de Favicons

![Generador de Favicons](html/favicon-generator.png)

1. **Diseño:** Crea una versión simplificada y cuadrada de tu logo.

2. **Formato:** Guárdala como `.png` o utiliza un generador en línea (como `favicon.io`) para crear un archivo `.ico` (mayor compatibilidad).

3. **Ubicación:** Añade el archivo al directorio principal de tu proyecto.

4. **Código:** Enlázalo dentro de la etiqueta `<head>` de tu HTML.

```html
<head>
    <meta charset="UTF-8">
    <title>Título de mi Página</title>
    
    <link rel="icon" href="favicon.ico" type="image/x-icon">
</head>
```

# Apuntes de **CSS**  (Hojas de Estilo en Cascada)

![CSS](/css/css.png) 
## Antes de nada, **que es CSS?** 

Es un lenguaje de estilo que se utiliza para controlar la presentación, el diseño y la apariencia de documentos escritos en un lenguaje de marcado como HTML 
En resumen, es un tipo de lenguaje que se utiliza para darle estilo a nuestro código hecho en *HTML* a través de un archivo adicional en **Visual Studio code**

## 1. Origen y Evolución

**Problema inicial:** En los inicios, HTML era solo estructura. Al querer mejorar el diseño, el código se ensuciaba mezclando contenido y presentación.

**Solución:** Nace CSS para separar la **estructura** (HTML) de la **presentación** (CSS). <br>

*HTML*: Define qué es cada cosa (título, vínculo)

*CSS*: Define cómo se ve (color, espacio posición)

**Empezó** en el 1996-1998 y se publicó el primer contenido CSS en ese año.

![Línea de Tiempo Evolución CSS](/css/línea-del-tiempo-css.png)

Los navegadores cuando van apareciendo nuevas funciones las van implementando poco a poco. 

**Ejemplo:**

**Microsoft Edge** En su día (2020), antes de aplicar su nuevo motor, carecía de soporte para efectos gráficos


Mientras que **Google Chome** Utiliza el motor *Blink* y suele marcar la pauta en nuevos estandáres. Tiene funciones con mejor adaptabilidad en el día a día. 

Aquí podemos **ver y notar las diferencias** del porque en un navegador carga con mayor rapidez o mayor sencillez algunos detalles de diferentes páginas.

## 2. Ventajas e Inconvenientes

### Ventajas
Código más fácil de leer.

Mayor potencia de diseño que el HTML antiguo.

Lenguaje sencillo.

**Reutilización**: Una misma hoja de estilo sirve para muchas páginas HTML.

**Adaptabilidad**: Puedes definir hojas distintas según el dispositivo (pantalla ordenador vs impresión).

## Inconveniente principal

Inconsistencia entre navegadores: Recordando la mención anterior, no todos los navegadores interpretan el código igual ni cumplen con los estándares al 100%, obligando a crear *"parches"* para navegadores específicos.


## 3.  Formas de aplicar CSS

Existen 3 formas principales de aplicar estilos, aunque en el siguiente ejemplo práctico **solo veremos dos de ellas**:

1.  **Estilo "Externo"** (Recomendado).
2.  **Estilo "Interno"** (En la cabecera).
3.  **Estilo "Inline"** (En línea).

### Ejemplo Práctico 

![IntroduccionCSS](/css/css2.png)

En esta captura de código podemos ver dos de las formas mencionadas arriba en el mismo archivo:

**Estilo Externo (Flecha Superior):**
Vemos la etiqueta `<link>` dentro del `<head>`. Esta línea conecta el HTML con el archivo *estilo.css*.

**Nota:** Se coloca en el head para evitar que la web se vea "rota" mientras carga.

**Estilo Inline (Flecha Inferior):**

Vemos el atributo *style="..."* dentro de la etiqueta `<p>`.
* *Ejemplo:* `<p style="color: green;">`
Aquí se está aplicando un color y tamaño específico solo para ese párrafo.

**Importante:** Al ser "Inline", este estilo **tiene prioridad** y sobrescribirá lo que diga el archivo externo.

* **Que falta?**
    En esta imagen **NO** se está usando el **Estilo Interno** (etiquetas `<style>` en el head).

### Demostración: Reglas Generales vs. Excepciones

"El estilo.css dice una cosa y el resultado otra, veremos porque.

![Código CSS](/css/cass4.png)

![Resultado en Navegador](/css/css3.png)

**¿Qué está pasando aquí?**

1.  **La Regla General (El archivo externo):**

En nuestro archivo CSS, hemos puesto una norma para toda la web: *"Todos los párrafos (p) deben ser de color rojo"*.

* *Resultado:* El primer párrafo obedece y se pinta de rojo.

2.  **La Excepción (El estilo en línea):**

El último párrafo, sin embargo, aparece en **verde**.
Esto ocurre porque el estilo en línea (*style="..."*) actúa como una excepción directa. Aunque la norma general diga "rojo", la instrucción específica en la etiqueta HTML dice "verde".

 **Conclusión:**
 El navegador siempre hará caso a la instrucción **más cercana** al elemento.

* El archivo CSS está "lejos" (es una norma global).

* El atributo *style* está "pegado" al texto (es una orden directa).

Por eso: **Orden directa (Inline) > Norma global (Externo).**


## Sistema de Puntos

![Explicación de los puntos en una imágen](/css/explicación-puntos.png)

Cuando hay un conflicto (como el rojo y verde de las capturas) el navegador suma puntos. **Gana el que más tenga**

### 1. La Tabla de Puntuación
* **1000 puntos:** Estilo Inline (style="..."). 
* **100 puntos:** ID (#header).
* **10 puntos:** Clases (.menu, :hover).
* **1 punto:** Elementos (h1, div, p).
* **0 puntos:** Universal (*).    

### 2. Las cuentas claras 

![Código CSS](/css/css2.png)
![Código CSS](/css/cass4.png)
![Resultado](/css/css3.png)

* **El CSS externo (Rojo):** Es una etiqueta *p* -> **1 punto**.

* **El HTML inline (Verde):** Es un atributo *style* -> **1000 puntos**.

**Resultado:** Gana el **VERDE** por una diferencia enorme (1000 > 1).

---

### 3. Notas Extra

* **!important:** Es el "botón nuclear". Si lo usas, gana a todos los puntos anteriores.

* **Herencia:** Es lo más débil. Cualquier regla directa (aunque valga 1 punto) gana a lo heredado.

##  Sintaxis Básica: Comentarios

Los comentarios son notas para nosotros o el quipo que esté detrás del código que **el navegador ignora** completamente (no se ven).

* **Símbolos:** Se escriben entre /* y */.

* **Característica:** En CSS **solo existen comentarios de bloque**, por lo que pueden ocupar una o varias líneas sin problema.


/* Este es un comentario explicativo
   que no afectará a la web 
*/

p {
    color: blue; /* Comentario en la misma línea */
}

![Representación de los comentarios](/css/comentarios-css.png)

# Apuntes: Selectores CSS (Tipos y Uso)

Selectores --> Para que sirven?

Sirven para decirle al navegador quiero cambiar *"x"* (color, tamaño, borde , etc..)

![Estructura de una Regla CSS](/css/sintáxis-básica.png)

## 1. Los Básicos 

### A. Selector de Elemento (o Tipo)
**¿Qué es?** Elige todas las etiquetas iguales de la página.

**Cómo se aplica:** Se escribe el nombre de la etiqueta.

**Ejemplo:**
    
p { color: red; } 
 Pone todos los párrafos en rojo
    

### B. Selector de ID
**¿Qué es?** Elige un elemento **único**. Es como el DNI, no puede haber dos iguales en la misma página.

**Cómo se aplica:** Se usa el símbolo almohadilla **#**.

**Ejemplo:**
    #menu-principal { background: black; }
    

### C. Selector de Clase
**¿Qué es?** Elige un **grupo** de elementos a los que has puesto la misma etiqueta "class". Es ideal para repetir estilos en varios sitios.

**Cómo se aplica:** Se usa el punto **.**

**Ejemplo:**
    .boton-azul { background: blue; }


## 2. Los Avanzados 

Sirven para seleccionar cosas muy específicas sin tener que llenar el HTML de clases extra.

### A. Selector Universal
**¿Qué es?** Elige **TODO** lo que hay en la página.

Se aplica usando el asterísco *.

**Ejemplo:**
{ margin: 0; } 


### B. Selector de Atributos
**¿Qué es?** Elige elementos que tengan una propiedad específica.

**Ejemplos:**
    
1. Por existencia (solo tener el atributo) */
    img[alt] { border: 1px solid red; }

* Afecta a todas las imágenes que tengan un texto alternativo

img[src="alert.gif"] { border: 1px solid black; }


### C. Hijos (>) vs. Descendientes
Hay que entender la diferencia de "profundidad":

1. **Selector de Hijos (>)**:

Solo afecta a los hijos **directos** (el nivel inmediatamente inferior).
    
div > p → Solo los párrafos que están justo dentro del div.

![Esquema Hijos vs Descendientes](/css/selectores-padrehijo.png)

2. **Selector de Descendientes (espacio)**:
Afecta a los hijos, nietos, bisnietos... a cualquiera que esté dentro (hablando de ramas de importancia)
    
div p → Cualquier párrafo dentro del div

### D. Selector de Hermanos Adyacentes (+)
**¿Qué es?** Elige el elemento que está **justo después** de otro.

**Ejemplo:**
    h1 + p { margin-top: 0; } 
* Solo afecta al primer párrafo que va justo después de un título

### E. Pseudoclases (:)

![Lista de los diferentes atributos](/css/lista-pseudoclases.png)

**¿Qué es?** Define estilos según el **estado** del elemento o la interacción del usuario.

**Ejemplo:**
    a:hover { color: orange; } 
* Cambia a naranja cuando pasas el ratón por encima

### F. Pseudoelementos (::)
**¿Qué es?** Da estilo a una **parte específica** del elemento, no a todo entero.

**Ejemplo:**
    p::first-line { font-weight: bold; } 

* Solo pone en negrita la primera línea del párrafo 

### G. Selector de Hijo N-ésimo (:nth-child) 
**¿Qué es?** Elige a un hijo específico según su posición (el 1º, el 2º, el 4º...), sin importar qué etiqueta sea.
**Ejemplo:**
.parent :nth-child(4) { 
    color: red; 
}
* Selecciona el cuarto hijo del elemento con clase *.parent*


## 3. Prioridad: 
A veces hay conflicto (por ejemplo, el archivo CSS dice "rojo" pero el HTML dice "verde").

El navegador usa un **sistema de puntos**, pero la regla fácil es: **"Cuanto más específico y cercano, más manda"**.

1. **Estilo en línea (*style="..."*): **El Jefe Supremo**. Gana a casi todo porque es una orden directa en la etiqueta.

2. **ID (#)**: **Subjefe**. Como es único, tiene mucha fuerza.

3. **Clase (.)**: **Manda normal**.

4. **Etiqueta (p, div)**: **La última opción**. Es muy genérico, así que cualquiera lo sobrescribe.

## 4. El Modelo de Caja (Box Model)

![Imágen representativa de Box Model](/css/boxmargin.png)

**¿Qué es?**

Es el sistema que usa el navegador para calcular el tamaño total de cualquier elemento web. Considera que **toda** etiqueta HTML (div, h1, img) es una caja rectangular compuesta por capas.

**Explicación técnica:**

1.  **Contenido:** Es la parte útil del elemento, lo que realmente ves (el texto, la imagen o el vídeo).

2.  **Padding (Relleno):** Es un espacio transparente que está **dentro** de la caja. Sirve para que el contenido no quede pegado a la línea del borde.

3.  **Border (Borde):** Es la línea física que rodea la caja. Marca el límite exacto donde termina tu elemento.

4.  **Margin (Margen):** Es un espacio transparente que está **fuera** de la caja. Sirve únicamente para separar este elemento de los demás que tenga al lado.

### A. El Margen (Margin)

**¿Qué es técnicamente?**
Es la propiedad que define el espacio **externo** alrededor de la caja. Es un área transparente que no tiene color de fondo.

**Control por lados:** Se puede definir una medida diferente para cada uno de los cuatro lados: arriba (top), derecha (right), abajo (bottom) e izquierda (left).

![Lista Propiedades Margin](/css/margin-css.png)

**Centrado automático:** Si usas el valor auto, el navegador calcula el espacio sobrante y lo reparte (se usa comúnmente para centrar bloques horizontalmente).

**Excepción importante:** Los elementos que son "de línea" (como un < span> o un enlace dentro de un texto) ignoran los márgenes de arriba y abajo; solo aplican los de los lados.

---

### B. Atajo: Escribir los 4 lados de golpe (Shorthand)
En lugar de escribir 4 líneas de código, puedes definir el margen (o el relleno) en una sola línea. El navegador interpreta los lados según cuántos valores pongas:

![Ejemplos Shorthand Colores](/css/padding-css.png)

**1 valor:** Aplica a los **4 lados** por igual.
    
padding: 10px; /* Arriba, Abajo, Izq, Der = 10px */

**2 valores:** El primero es **Vertical** (Arriba/Abajo) y el segundo **Horizontal** (Izq/Der).
    
padding: 10px 20px; /// 10px Arriba/Abajo | 20px Izq/Der

* **4 valores:** Sigue el sentido de las **agujas del reloj** (empezando a las 12:00).

padding: 10px 20px 30px 40px; 

1. Arriba - 2. Derecha - 3. Abajo - 4. Izquierda


## 5. Comportamiento de la Caja (Display y Tamaño)

### A. Propiedad *display*
Controla cómo se comporta el elemento dentro de la página.

**block (Bloque):** El elemento ocupa **todo el ancho** disponible y fuerza un salto de línea (se pone uno debajo de otro).

**inline (En línea):** El elemento solo ocupa el espacio de su contenido y se coloca al lado de otros.

### B. El problema del tamaño (*box-sizing*)
Por defecto, si añades relleno (*padding*) o borde a una caja, estos se suman al ancho total, haciendo la caja más grande de lo planeado.

![Solución Box Sizing](/css/display-block.png)

**Solución (*border-box*):** Cambia el cálculo para que el relleno y el borde se incluyan **dentro** de las medidas que has definido. 

## 6. Control del Desbordamiento

### A. Desbordamiento General (*overflow*)

Define qué pasa cuando el contenido es más grande que la caja y no cabe.

![Tipos de Overflow](/css/desbordamientos-overflow.png)

**visible:** El contenido se sale de la caja y se ve por fuera (es lo que pasa por defecto).

**hidden:** Lo que sobra se corta y se oculta.

**scroll:** Añade barras de desplazamiento siempre.

**auto:** El navegador decide: si cabe no hace nada, y si no cabe añade barras de desplazamiento.

### B. Desbordamiento de Texto (text-overflow)

![Tipos de Overflow](/css/desbordamiento-overflow.png)

Sirve específicamente para controlar qué pasa con el **texto** cuando se corta por falta de espacio.

1. **clip:** Corta el texto tajantemente justo donde acaba la caja.

2. **ellipsis:** Corta el texto pero añade tres puntos suspensivos (...) al final para indicar que hay más.


## 7. Diseño Flexible (Flexbox)
**¿Qué es?**
Es un sistema moderno para ordenar elementos en una web. Permite que los elementos se adapten automáticamente al espacio disponible, haciendo más fácil crear diseños que funcionen en móviles y ordenadores.

### A. Conceptos Básicos
Para que funcione, necesitas definir dos roles:

1. **Contenedor (Padre):** Es el elemento que envuelve a los demás. Aquí aplicas *display: flex*.

2. **Ítem (Hijo):** Son los elementos que están dentro. Estos son los que se mueven y se adaptan.

### B. Los Ejes (Dirección)
Flexbox organiza los elementos siguiendo dos líneas imaginarias:

![Imágen representativa de los ejes de FlexBox](/css/ejes.png)

**Eje Principal:** Es la dirección principal hacia donde van los elementos (por defecto es horizontal, en fila).

**Eje Secundario:** Es la dirección perpendicular (por defecto es vertical, de arriba a abajo).

### Resumen Visual

![Representación del FlexBox](/css/resumen-displayflex.png)

## 8. Diseño Responsivo (Responsive Design)

![Representación del Responsive](/css/diseño-responsive.png)

**¿Qué es?**
Es una técnica de diseño que permite que un sitio web se ajuste y reorganice automáticamente según el tamaño de la pantalla (móvil, tablet u ordenador) para que siempre se lea bien.

**Características Principales:**

**Flexible:** Los elementos no tienen tamaños fijos, si no que se estiran o encogen.

**Rejillas fluidas:** Se usan porcentajes (ej: *width: 50%*) en lugar de píxeles fijos para que los contenedores se adapten.

**Reorganización:** Lo que en un ordenador se ve en 3 columnas, en un móvil se coloca en una sola columna vertical para facilitar la lectura para el usuario.


## 9. Media Queries (*@media*)

**¿Qué son?**
Son reglas especiales de CSS que funcionan como un "condicional". 
Sirven para aplicar estilos específicos **solo** si la pantalla cumple ciertos requisitos (como tener un ancho mínimo o máximo).

![Representación de Media Queries](/css/media-queries.png)

**Funcionamiento Técnico (Lógica Condicional):**
Las *Media Queries* actúan como una sentencia lógica. 
El navegador evalúa constantemente el ancho de la ventana de visualización (**viewport**). Si la condición se cumple (ej: el ancho es menor a 768px), el navegador activa ese bloque de código CSS respetándolo.

**Jerarquía y Cascada (Estrategia Desktop-First):**
El ejemplo utiliza una estrategia de **sobreescritura**. El navegador lee el código de arriba a abajo:

1.  **Estilo Global (Default):** Se carga el *background-color: blue*. Esto aplica a todas las pantallas inicialmente.

2.  **Punto de Ruptura (Tablet):** Si el viewport es *<=* 768px, la regla condicional se activa y **sobreescribe** el color anterior a verde.

3.  **Punto de Ruptura (Móvil):** Si el viewport es *<=* 480px, esta nueva regla tiene prioridad por estar más abajo en la cascada y **vuelve a sobreescribir** el color a amarillo.
