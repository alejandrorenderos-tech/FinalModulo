# Portafolio personal

Portafolio web académico creado para la evaluación final del módulo de Fundamentos de Desarrollo Web. Presenta un perfil, una selección de proyectos y un formulario de contacto con un diseño adaptable a móviles, tablets y escritorio.

El proyecto está desarrollado únicamente con **HTML5 y CSS3**: no usa JavaScript, frameworks, dependencias ni procesos de compilación.

## Contenido del proyecto

| Archivo o carpeta | Descripción |
| --- | --- |
| `index.html` | Página de inicio y presentación. |
| `acerca.html` | Perfil, imagen, habilidades, herramientas y áreas de interés. |
| `proyectos.html` | Proyecto destacado y tabla de trabajos. |
| `contacto.html` | Información de contacto y formulario de demostración. |
| `style.css` | Hoja de estilos compartida por las cuatro páginas. |
| `assets/avatar.svg` | Ilustración provisional de perfil, reemplazable por una fotografía. |
| `GITHUB-PAGES.md` | Instrucciones para publicar el sitio mediante GitHub Pages. |

## Requisitos de la evaluación implementados

- **Navegación compartida:** las cuatro páginas incluyen un menú principal con enlaces entre ellas y cargan `style.css`.
- **Estructura semántica:** se utilizan elementos como `header`, `nav`, `main`, `section`, `aside` y `footer`, con jerarquía de encabezados.
- **Página de inicio:** presenta el portafolio y ofrece un enlace directo a los proyectos.
- **Acerca de:** muestra una imagen provisional y listas de habilidades, herramientas e intereses.
- **Proyectos:** incorpora una tabla con encabezado semántico y cuatro filas de datos. En pantallas estrechas, la tabla puede desplazarse horizontalmente.
- **Contacto:** incluye campos de texto y correo, contraseña temporal, selector, opciones de radio, casilla de aceptación, archivo y área de texto. Usa atributos nativos como `required`, `type="email"`, `minlength`, `maxlength` y `accept`.
- **Diseño adaptable:** el CSS utiliza un enfoque mobile-first, Grid, Flexbox y media queries para adaptar el contenido a distintos anchos de pantalla.
- **Accesibilidad básica:** hay etiquetas asociadas a los campos, foco visible, enlace para saltar al contenido, texto alternativo para la imagen y soporte para reducir movimiento.
- **CSP:** cada página define una política básica de Content Security Policy mediante una etiqueta `meta`.
- **Organización CSS:** los nombres de clase siguen una convención inspirada en BEM, por ejemplo `site-nav__link` y `site-nav__link--active`.

## Abrir y probar el sitio

No es necesario instalar nada:

1. Abre `index.html` en un navegador, o sirve la carpeta con una herramienta local como Live Server.
2. Usa la navegación para recorrer Inicio, Acerca de, Proyectos y Contacto.
3. Prueba el diseño en una ventana estrecha y otra amplia.
4. En Contacto, comprueba los campos obligatorios y los formatos aceptados.

## Personalizar el portafolio

1. En las páginas HTML, reemplaza el contenido de ejemplo por tu nombre, ubicación, perfil y datos de contacto.
2. En `proyectos.html`, actualiza nombres, tecnologías, fechas y estados de la tabla.
3. Para usar tu fotografía, guarda el archivo dentro de `assets/` y actualiza el atributo `src` de la imagen en `acerca.html`.
4. Si cambias o agregas páginas, conserva la navegación y el enlace a `style.css`.
5. Si incorporas imágenes, fuentes u otros recursos externos, revisa la política CSP de cada página para permitir únicamente los recursos necesarios.

## Formulario y seguridad

El formulario es una **demostración visual**. GitHub Pages sirve archivos estáticos y no proporciona un servidor para recibir, procesar ni almacenar los datos del formulario. No introduzcas contraseñas reales ni información sensible. Para recibir mensajes se necesita conectar un servicio de formularios o desarrollar un backend, y validar también los datos en el servidor.

Los atributos de validación HTML ayudan al navegador a detectar entradas incompletas o con formato incorrecto, pero no son una medida de seguridad ni sustituyen la validación del servidor. El atributo `accept` orienta el selector de archivos, pero no garantiza la seguridad del archivo.

## Tecnologías

- HTML5
- CSS3 (Grid, Flexbox, variables, media queries y estados interactivos)
- Git y GitHub Pages para control de versiones y publicación
