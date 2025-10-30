# Semana 03

## Ingeniería Web

**Fecha:** 21/10/2025  
**Estudiante:** Anthony Joel Romero Yaguana  
**Paralelo:** A  

## Instalación del entorno de desarrollo local (XAMPP)

Durante esta práctica se llevó a cabo la **instalación del entorno de desarrollo XAMPP**, una herramienta esencial que integra **Apache, MariaDB, PHP y Perl**. Este paquete permite crear un servidor local para el desarrollo y prueba de aplicaciones web dinámicas, sin depender de un hosting externo.

---

### Proceso de instalación

1. En primer lugar, se accedió al sitio oficial de **[Apache Friends](https://www.apachefriends.org/download.html)**, desde donde se seleccionó la versión más reciente de **XAMPP para Windows (8.1.25 / 64 bits)**.  
<img width="1280" height="799" alt="image" src="https://github.com/user-attachments/assets/7de2b8f0-1da9-4833-a84e-0f4bb7e96ddc" />

2. Posteriormente, la descarga fue redirigida a **SourceForge**, sitio que aloja los archivos oficiales de instalación. Desde allí se completó la descarga del instalador.  
<img width="1280" height="799" alt="image" src="https://github.com/user-attachments/assets/f2d4f524-711f-4bb7-86ec-1367752d03fa" />


3. Una vez descargado, se ejecutó el instalador y se siguieron los pasos guiados del asistente (VMware InstallBuilder). Durante el proceso, se seleccionaron los módulos principales:  
   - **Apache** (servidor web)  
   - **MySQL / MariaDB** (gestor de bases de datos)  
   - **PHP** (lenguaje de programación)  
   - **phpMyAdmin** (interfaz de administración de bases de datos)  

   <img width="1280" height="799" alt="image" src="https://github.com/user-attachments/assets/6d7e7868-aca4-48fb-be91-f147461781ce" />


4. Finalmente, tras la instalación, se verificó el correcto funcionamiento del entorno ingresando en el navegador a la dirección **[http://localhost/dashboard](http://localhost/dashboard)**, donde se desplegó el panel de bienvenida de XAMPP.  
 <img width="1280" height="799" alt="image" src="https://github.com/user-attachments/assets/8211c3f4-c4e3-4490-a07f-4478ed8c19f2" />
 

La instalación se completó satisfactoriamente, mostrando la página de inicio de XAMPP para Windows **versión 8.1.25**.  
Esto confirmó que los servicios de **Apache** y **MySQL** se encontraban activos, permitiendo iniciar la creación y prueba de aplicaciones dinámicas en un entorno controlado y seguro.  

<img width="1280" height="799" alt="image" src="https://github.com/user-attachments/assets/a4275151-99aa-4533-b996-5260f4d20640" />

## Configuración del CMS WordPress conectado a la base de datos

Una vez finalizada la instalación de **XAMPP** y comprobado el funcionamiento del servidor local, se procedió con la **configuración del gestor de contenidos WordPress**, utilizando una base de datos creada previamente en **MySQL Workbench**.

---

### Creación de la base de datos

El primer paso consistió en crear la base de datos que almacenará toda la información del sitio web: usuarios, entradas, configuraciones y comentarios.  
Para ello, se empleó **MySQL Workbench**, ejecutando la siguiente instrucción SQL:

```sql
CREATE DATABASE basePrueba;
```

La ejecución de este comando creó una base de datos vacía lista para ser enlazada con WordPress, lo que permitirá almacenar de forma estructurada la información del sitio.

<img width="1280" height="799" alt="image" src="https://github.com/user-attachments/assets/0d86fb85-c5a1-4094-bc2a-e79bf581f460" />


---

### Instalación y configuración inicial de WordPress

Con la base de datos lista, se descargó **WordPress** desde su sitio oficial y se colocó la carpeta dentro del directorio `htdocs` de **XAMPP**.  
Posteriormente, se accedió desde el navegador a la ruta **http://localhost/ingWeb/tia**, iniciando el asistente de instalación del CMS.

En esta etapa se configuró la información inicial del sitio, asignando el nombre **“Almacenes Tía”**, el usuario principal **anthonyJoel**, una contraseña segura y el correo institucional **ajromero12@utpl.edu.ec**.

<img width="1280" height="824" alt="image" src="https://github.com/user-attachments/assets/ba234dec-4af0-4804-b062-4c4001642c9f" />


Tras ingresar los datos y confirmar la conexión con la base de datos `basePrueba`, el sistema generó automáticamente las tablas necesarias (como `wp_users`, `wp_posts`, `wp_options`, entre otras).  
Finalmente, se mostró el mensaje de instalación completada, indicando que el CMS estaba listo para usarse.

<img width="1280" height="799" alt="image" src="https://github.com/user-attachments/assets/3d7957b8-bc16-4406-b67a-1de5e3dbf6ed" />

---

### Acceso al panel administrativo

Una vez instalada la plataforma, se accedió al **panel de administración (wp-admin)**, el entorno principal de trabajo de WordPress.  
Desde aquí es posible crear entradas, páginas, gestionar usuarios, añadir plugins y personalizar la apariencia del sitio.

<img width="1280" height="801" alt="image" src="https://github.com/user-attachments/assets/37d46063-2f75-4f53-897d-c062e105d161" />

---

### Visualización del sitio web

Al finalizar la configuración, se abrió el sitio principal en la dirección **http://localhost/ingWeb/tia/**, mostrando la página predeterminada con el mensaje **“¡Hola, mundo!”**.  
Esto confirmó que el entorno funcionaba correctamente y que la conexión entre **WordPress**, **Apache** y **MySQL/MariaDB** era estable y funcional.

<img width="1280" height="799" alt="image" src="https://github.com/user-attachments/assets/d1ca7bb5-dc3a-475f-a8d0-c213803ef2a3" />

# Personalización y uso de plugins en WordPress

## Implementación de temas y personalización del sitio

En esta parte del proyecto se trabajó en la **personalización visual del sitio web de prueba “Almacenes Tía”** utilizando las herramientas integradas de WordPress.  
Desde el panel administrativo, se accedió a la sección **Apariencia → Temas**, donde se activó el tema **Twenty Twenty-Four**, y posteriormente se exploraron otros temas disponibles como **Twenty Twenty-Five** y **Twenty Twenty-Three**, observando sus diferencias visuales y de estructura.

<img width="1280" height="799" alt="image" src="https://github.com/user-attachments/assets/8cc87cc6-6877-4fc7-acab-7885e2dfb373" />


---

## Creación de contenido y páginas

Para probar las funcionalidades del CMS, se creó una página llamada **“Misión y Visión”**, en la que se añadió un texto descriptivo y una imagen institucional de Almacenes Tía.  
Esta práctica permitió experimentar con el **editor de bloques de WordPress**, agregando encabezados, párrafos e imágenes de manera dinámica.

<img width="1280" height="799" alt="image" src="https://github.com/user-attachments/assets/a32574e6-9110-43da-9627-f468678d9e34" />


Al visualizar el sitio, se comprobó que la nueva página aparecía correctamente en el menú de navegación principal, junto con otras secciones del sitio.

<img width="1280" height="799" alt="image" src="https://github.com/user-attachments/assets/f0de092f-c817-4a42-a101-b1512fceb5e7" />

<img width="1280" height="799" alt="image" src="https://github.com/user-attachments/assets/bf070954-4cf5-479d-aa25-4a3fb47af82c" />


---

## Integración de plugins y herramientas de diseño

Para mejorar la funcionalidad del sitio, se instalaron **plugins de SiteOrigin**, incluyendo:

- **Page Builder by SiteOrigin:** para construir páginas con un sistema de arrastrar y soltar.  
- **SiteOrigin Widgets Bundle:** para añadir iconos, botones, encabezados y elementos visuales.  
- **SiteOrigin CSS:** para realizar ajustes visuales mediante hojas de estilo personalizadas.  

<img width="1280" height="799" alt="image" src="https://github.com/user-attachments/assets/d687f1dd-95c9-4d8d-af3b-52ae78699cfd" />


Una vez instalados los complementos, se configuró una **página de inicio personalizada**, agregando secciones visuales como encabezado, íconos circulares y bloques de texto con el constructor visual de SiteOrigin.

<img width="1280" height="799" alt="image" src="https://github.com/user-attachments/assets/1f022ba0-6c95-4b45-9d90-446c4e930bdf" />

---

## Creación de una tienda virtual de prueba

Como parte de la práctica, se integró un sistema de **tienda virtual** dentro del mismo sitio de WordPress, utilizando el plugin **WooCommerce**.  
Se añadieron productos de ejemplo con precios y etiquetas de oferta, para comprobar el funcionamiento del carrito de compras y la estructura de la tienda.

<img width="1280" height="799" alt="image" src="https://github.com/user-attachments/assets/52459808-b1c3-4800-a6ec-2044b36ee65e" />



Finalmente, se accedió a la sección **Tienda**, donde se visualizaron los productos creados.  
Esta experiencia permitió comprender el proceso de **integración de comercio electrónico** dentro de un CMS, observando cómo WordPress puede evolucionar de un simple blog a un sistema completo de gestión y ventas.

<img width="1280" height="799" alt="image" src="https://github.com/user-attachments/assets/85d33548-c9a2-44cb-bf7a-2e5a79eb11b1" />



---

### Bibliografía

- WooCommerce. (s. f.). *Extensión oficial para comercio electrónico en WordPress*. https://woocommerce.com/  
- WordPress. (s. f.). *WordPress.org – Herramienta de gestión de contenidos*. https://wordpress.org/  
- MySQL. (s. f.). *MySQL Workbench – Visual Database Design Tool*. https://www.mysql.com/products/workbench/  
- Apache Friends. (s. f.). *Download XAMPP*. https://www.apachefriends.org/download.html  

