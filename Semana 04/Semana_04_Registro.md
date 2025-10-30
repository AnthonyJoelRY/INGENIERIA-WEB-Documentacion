# Semana 03

## Ingeniería Web

**Fecha:** 30/10/2025  
**Estudiante:** Anthony Joel Romero Yaguana  
**Paralelo:** A  

# Practica en html
# 🌐 Práctica: Creación de la Página de Inicio "AppTurismo"

## 🧩 Objetivo
Desarrollar una página web inicial para un proyecto de turismo, aplicando los conceptos básicos de **HTML y CSS**, organizando correctamente las carpetas dentro del entorno **XAMPP** y visualizando el resultado desde el navegador utilizando `localhost`.

---

## 🗂️ Estructura del Proyecto

El proyecto fue guardado dentro del directorio de XAMPP:
```
C:\xampp\htdocs\appturismo
```

Dentro de la carpeta **appturismo** se crearon los siguientes subdirectorios:

- `css/` → contiene la hoja de estilos `estilos.css`
- `imagenes/` → destinada para futuros recursos gráficos
- `index.html` → archivo principal de la página

![Imagen de WhatsApp 2025-10-29 a las 12 06 41_1f8df7bc](https://github.com/user-attachments/assets/f17e83b8-fc8a-46cc-af66-cf993298f67e)

---

## 💻 Desarrollo del sitio web

### 1️⃣ Creación del archivo HTML
En el archivo **index.html** se definió la estructura base de la página utilizando etiquetas semánticas como:

```html
<header>, <nav>, <section>, <article> y <footer>
```

Dentro del encabezado (`<header>`) se colocaron dos divisiones: una para el logotipo y otra para el formulario de búsqueda.  
El menú de navegación (`<nav>`) incluyó enlaces simulados hacia las secciones principales: **Inicio**, **Servicios**, **Portafolio** y **Contactos**.

Además, se creó una sección para el **slider principal** y otra para las **noticias**, con un pie de página que contiene los créditos:
```html
<footer>
  <h6>Derechos reservados UTPL 2025 power by @ajromero12</h6>
</footer>
```

![Imagen de WhatsApp 2025-10-29 a las 12 04 54_266c8b23](https://github.com/user-attachments/assets/7671d7cb-e0e0-4492-8311-215ff297157e)

---

### 2️⃣ Diseño con CSS
Se agregó la hoja de estilos `estilos.css` dentro de la carpeta `css` y se enlazó en el `<head>` del HTML.

#### Estilos principales aplicados:
```css
* {
  padding: 0;
  margin: 0;
}

body {
  font-family: Arial, Helvetica, sans-serif;
  background-color: beige;
}
```

- Se normalizaron los márgenes y rellenos con el selector universal `*`.
- Se definió un fondo de color **beige** y la fuente principal.

📘 También se utilizó la fuente **Montserrat** importada desde Google Fonts.

---

### 3️⃣ Estilización de secciones
Cada bloque del HTML recibió un estilo visual:

```css
.cabeceraPrincipal, .menuPrincipal, .sliderPrincipal {
  background-color: blue;
  color: azure;
  width: 80%;
  margin: 0 auto;
}
```

- El **menú principal** (`.menuPrincipal`) se configuró con color rojo, centrado y con efecto `hover` para resaltar los enlaces al pasar el cursor:
```css
nav.menuPrincipal a:hover {
  background-color: #fff;
  color: red;
  border-bottom: blue 5px solid;
  transition: width 2s, height 4s, background-color 3s;
}
```

![Imagen de WhatsApp 2025-10-29 a las 12 05 01_ed0a944e](https://github.com/user-attachments/assets/b1991497-d4e9-41a8-9284-589bf97f3581)

---

### 4️⃣ Implementación del slider y las noticias
Se creó una sección `.sliderPrincipal` con un alto de `400px` y texto centrado, además de la sección `#noticias` con dos artículos (Noticia 1 y Noticia 2):

```css
section.sliderPrincipal {
  height: 400px;
  text-align: center;
}

#noticias {
  background-color: blue;
  color: white;
}
```

![Imagen de WhatsApp 2025-10-29 a las 12 06 18_1d69240a](https://github.com/user-attachments/assets/c9fc9899-4381-499c-b4b6-629953501ce6)

---
