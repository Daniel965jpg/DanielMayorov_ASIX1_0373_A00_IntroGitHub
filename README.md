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

Un repositorio ("repo") es simplemente una carpeta de proyecto que está siendo rastreada por Git.

### 3.1. Creación de un Repositorio Nuevo

Tienes tres caminos principales:

### Opción 1: Clonar un Repositorio Existente (El más común)

Clonar descarga una copia completa de un proyecto existente en GitHub (incluyendo todo el historial) a tu ordenador.


# Busca el botón verde "Code" en GitHub y copia la URL HTTPS
git clone [https://github.com/usuario/nombre-del-repo.git](https://github.com/usuario/nombre-del-repo.git)

# Esto crea una nueva carpeta "nombre-del-repo". Entra en ella:
cd nombre-del-repo

### Opción 2: Crear un Repositorio Local Nuevo (desde cero)

Si empiezas un proyecto nuevo desde tu ordenador.

# Crea tu carpeta de proyecto
mkdir mi-proyecto
cd mi-proyecto

# Inicializa Git dentro de esta carpeta
git init

# Ahora Git está observando. Haz tu primer commit:
git add .
git commit -m "Commit inicial"

Para bajar los cambios del remoto y fusionarlos con nuestro trabajo el comando es:
git pull

## 4. Colaboración: Ramas y Pull Requests

Esta es la parte más potente de GitHub.

* **Rama (Branch):** Una rama es una línea de tiempo paralela de commits. La rama principal se llama `main`. **Nunca se debería trabajar directamente sobre `main`**.
* **Flujo de trabajo:**
    1.  Creas una rama nueva para cada tarea (ej. `feature/añadir-formulario`).
    2.  Trabajas y haces commits en esa rama.
    3.  Cuando terminas, abres un **Pull Request (PR)**.
    4.  Un PR es una "solicitud para fusionar" tu rama con `main`.
    5.  Otras personas pueden revisar tu código, dejar comentarios y, finalmente, aprobarlo.
    6.  Una vez aprobado, fusionas el PR y tu trabajo se incorpora a `main`.

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