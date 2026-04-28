# Proyecto 02 — Creative Agency Landing Page

Página web estática de presentación para una agencia creativa ficticia llamada **Livia**. Construida con HTML5 semántico y CSS3 puro como ejercicio de maquetación estructurada.

---

## 🎯 Objetivos

Conceptos que se practican en este proyecto:

| Concepto | Descripción |
|---|---|
| **Maquetación con Flexbox** | Uso de `display: flex` para construir el header y la barra de navegación de forma alineada y responsiva. |
| **CSS Grid** | Implementación de `display: grid` con `repeat(3, 1fr)` para crear la sección de categorías en tres columnas de igual ancho. |
| **`image-set()`** | Uso de la función CSS `image-set()` para servir imágenes de alta resolución (retina/2x) en el fondo del body. |
| **Google Fonts** | Integración de tipografías externas (`Bebas Neue` y `Poppins`) mediante `<link>` en el `<head>`. |
| **HTML5 Semántico** | Uso correcto de etiquetas `<header>`, `<section>`, `<nav>`, `<figure>`, `<article>`. |
| **Background responsivo** | Control de imagen de fondo con `background-size`, `background-position` y `background-repeat`. |
| **Boilerplate HTML5** | Comprensión y uso del template HTML5 Boilerplate con sus utilidades CSS de ayuda (`.hidden`, `.visually-hidden`, `.clearfix`). |
| **Webpack** | Configuración de un entorno de desarrollo con servidor local (`webpack-dev-server`) y un proceso de build de producción. |
| **Web App Manifest** | Inclusión de `site.webmanifest`, favicons e íconos PWA para compatibilidad multi-dispositivo. |

---

## 📁 Estructura de archivos

```
Proyectos02-CreativeAgency/
│
├── index.html              # Documento principal HTML del sitio
├── 404.html                # Página de error personalizada (no encontrado)
├── robots.txt              # Directivas para motores de búsqueda
├── site.webmanifest        # Manifiesto de la Web App (nombre, iconos, colores)
├── favicon.ico             # Ícono del sitio para navegadores (formato ICO)
├── icon.png                # Ícono PNG para dispositivos Apple (apple-touch-icon)
├── icon.svg                # Ícono SVG escalable del sitio
├── icon-512.png            # Ícono de alta resolución para PWA (512×512 px)
├── package.json            # Configuración del proyecto Node.js y dependencias
├── webpack.common.js       # Configuración base compartida de Webpack
├── webpack.config.dev.js   # Configuración de Webpack para modo desarrollo
├── webpack.config.prod.js  # Configuración de Webpack para build de producción
├── .editorconfig           # Reglas de formato de código para el editor
├── .gitattributes          # Reglas de manejo de archivos para Git
├── .gitignore              # Archivos y carpetas ignorados por Git
├── LICENSE.txt             # Licencia del proyecto
├── README.md               # Documentación del proyecto
│
├── css/
│   └── style.css           # Hoja de estilos principal (Boilerplate + estilos propios)
│
├── img/
│   ├── logo_livia.svg      # Logotipo de la agencia Livia (SVG)
│   ├── group.jpg           # Fotografía hero (resolución estándar 1x)
│   ├── group@2x.jpg        # Fotografía hero (resolución retina 2x)
│   ├── arrow.svg           # Ícono de flecha para el botón CTA del hero
│   ├── web_design.svg      # Ícono de la categoría "Web Design Projects"
│   ├── social_media.svg    # Ícono de la categoría "Social Media Templates"
│   ├── design.svg          # Ícono de la categoría "Digital Artwork"
│   └── .gitkeep            # Archivo vacío para que Git rastree la carpeta
│
└── js/
    ├── app.js              # Punto de entrada JavaScript del proyecto
    └── vendor/             # Librerías JavaScript de terceros
        └── .gitkeep        # Archivo vacío para que Git rastree la carpeta
```

---

## 🖥️ Secciones del sitio

### Header

La barra de navegación superior divide la pantalla en dos extremos: a la izquierda el **logotipo de Livia** seguido del menú de navegación, y a la derecha un botón de llamada a la acción **"Contact Us"** con el color corporativo azul. El resultado es un encabezado limpio, profesional y orientado a la conversión desde el primer vistazo.

---

### Hero

Es la sección de mayor impacto visual del sitio. Ocupa el área central de la página y se superpone sobre una fotografía de fondo en alta resolución (con soporte retina 2x). Presenta:

- Un saludo introductorio discreto (`Hi, There!`)
- Un titular principal de gran tamaño con la propuesta de valor de la agencia
- Un párrafo breve que refuerza el mensaje
- Un botón CTA **"Let's Collaborate"** acompañado de una flecha SVG que invita a la acción

El diseño del hero comunica autoridad creativa: tipografía dominante, mucho espacio en blanco y un botón claro que contrasta con el fondo azul profundo.

---

### Categorías

Un panel de **tres tarjetas** ubicado en la parte inferior del hero que presenta los servicios principales de la agencia:

| Tarjeta | Servicio |
|---|---|
| 🎨 | Web Design Projects |
| 📱 | Social Media Templates |
| 🖼️ | Digital Artwork |

Cada tarjeta incluye un ícono SVG representativo, un título y un texto descriptivo breve. El panel tiene fondo blanco roto (`#FBFBFB`) que lo hace destacar sobre el fondo azul del sitio, y está desplazado ligeramente hacia la izquierda para romper la simetría y lograr un efecto visual más dinámico.

---

## 🛠️ Tecnologías

| Tecnología | Versión | Uso |
|---|---|---|
| **HTML5** | — | Estructura semántica del sitio |
| **CSS3** | — | Estilizado completo (Flexbox, Grid, `image-set`) |
| **JavaScript** | ES6+ | Punto de entrada (`app.js`) para futuras interacciones |
| **HTML5 Boilerplate** | v9.0.1 | Base de estilos cross-browser y buenas prácticas |
| **Google Fonts** | — | Tipografías `Bebas Neue` y `Poppins` |
| **Webpack** | ^5.105.3 | Bundler: servidor de desarrollo y build de producción |
| **webpack-dev-server** | ^5.2.3 | Servidor local con recarga automática (HMR) |
| **html-webpack-plugin** | ^5.6.6 | Generación automática del HTML en el build |
| **copy-webpack-plugin** | ^13.0.1 | Copia de assets estáticos al directorio de build |
| **webpack-merge** | ^6.0.1 | Fusión de configuraciones comunes y específicas |

---

## 🚀 Instalación y uso

### Requisitos previos

- [Node.js](https://nodejs.org/) (versión LTS recomendada)
- [npm](https://www.npmjs.com/) (incluido con Node.js)

### Pasos

```bash
# 1. Clonar el repositorio
git clone <url-del-repositorio>
cd proyecto_02/code

# 2. Instalar dependencias
npm install

# 3. Iniciar el servidor de desarrollo (con recarga automática)
npm start

# 4. (Opcional) Generar el build de producción
npm run build
```

> El servidor de desarrollo abrirá automáticamente el navegador en `http://localhost:8080` (o el puerto disponible).
> El build de producción se genera en la carpeta `dist/`.

---

## 🎨 Paleta de colores

| Color | Hex | Uso |
|---|---|---|
| Azul corporativo | `#515DEF` | Fondo principal, botón del header |
| Blanco roto | `#FBFBFB` | Textos, botón CTA y fondo de categorías |
| Gris oscuro | `#333333` | Títulos de tarjetas y texto del botón CTA |
| Gris medio | `#909090` | Texto descriptivo de tarjetas |
| Rosa claro (hover) | `#d6c1c1` | Acento en hover de enlaces |
| Azul selección | `#b3d4fc` | Resaltado al seleccionar texto |

---

## 🔤 Tipografías

Dos fuentes importadas desde **Google Fonts**:

| Fuente | Pesos | Uso principal |
|---|---|---|
| **Poppins** | 100, 200, 400, 600 | Tipografía base del sitio: nav, párrafos, botones y tarjetas |
| **Bebas Neue** | 400 | Disponible para títulos de alto impacto (sin regla CSS asignada aún) |

---

## 💡 Aprendizajes clave

### 1. Flexbox y Grid como herramientas complementarias
El proyecto demuestra de forma clara que **Flexbox y Grid no son rivales sino complementarios**. Flexbox se usa para distribución unidimensional (el header en fila, el nav horizontal), mientras que Grid se usa para el layout bidimensional de la sección de categorías. Saber elegir la herramienta correcta según el eje de distribución es una habilidad fundamental del maquetador moderno.

### 2. Imágenes responsivas con `image-set()`
La función CSS `image-set()` es el equivalente en CSS puro del atributo HTML `srcset`. Permite servir automáticamente la imagen de mayor resolución (`group@2x.jpg`) en pantallas de alta densidad de píxeles (Retina, OLED) sin JavaScript. Esto optimiza la experiencia visual y el peso de carga simultáneamente.

### 3. Semántica HTML como base del diseño
El uso correcto de `<header>`, `<section>`, `<figure>`, `<nav>`, `<article>` no es solo una buena práctica: **define la arquitectura visual**. Las reglas CSS se anclan directamente en estos elementos semánticos (`header`, `header nav ul`), lo que hace el código más mantenible y predecible que si se usaran clases genéricas para todo.

### 4. El poder del `transform: translateX()`
La sección de categorías usa `transform: translateX(-40px)` para romper levemente la alineación de cuadrícula y lograr un efecto visual asimétrico y moderno. Este recurso, sin coste de layout (no desplaza otros elementos), es una forma efectiva de añadir dinamismo a diseños que de otro modo serían demasiado rígidos.


### 5. HTML5 Boilerplate como punto de partida
Usar un boilerplate experimentado en lugar de un archivo HTML en blanco introduce al desarrollador en decisiones ya resueltas por la comunidad: estilos cross-browser, manejo de `::selection`, clases de accesibilidad (`.visually-hidden`), estilos de impresión. Entender qué hace cada parte del boilerplate es más valioso que simplemente borrarlo.

---

> Proyecto desarrollado como ejercicio de práctica de maquetación web con HTML y CSS.