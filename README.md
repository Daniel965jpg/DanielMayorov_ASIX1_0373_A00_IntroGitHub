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


> **Importante:** Nunca deberías trabajar directamente sobre `main`.


---


### Flujo de trabajo típico


1. Crea una rama nueva para cada tarea (por ejemplo: `feature/añadir-formulario`).
2. Trabaja y haz commits en esa rama.
```html
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Título de la Página (aparece en la pestaña)</title>
    
    <!-- Vincular hoja de estilos CSS -->
    <link rel="stylesheet" href="style.css">
    
    <!-- Ícono de la página -->
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

### HTML Semántico
Utiliza etiquetas como `<header>`, `<main>`, `<footer>`, `<nav>`, `<section>` y `<article>` para dar significado a la estructura.

### Importancia del HTML Semántico

**Esto es vital para:**
* **Accesibilidad:** los lectores de pantalla pueden interpretar mejor la página.
* **SEO:** los motores de búsqueda como Google entienden mejor el contenido de tu web.

**Ejemplos de uso semántico:**
* `<nav>` &rarr; barra de navegación
* `<section>` &rarr; sección del contenido
* `<article>` &rarr; artículo independiente
* `<footer>` &rarr; pie de página

**Consejos adicionales:**
* Mantén tu HTML limpio y organizado con sangrías consistentes.
* Usa comentarios: `` para documentar tu código.
* Combina HTML con CSS para diseño y estilo y con JavaScript para interactividad (que aun no hemos hecho).