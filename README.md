<a name="readme-top"></a>

<!-- PROJECT SHIELDS -->

[![Contributors][contributors-shield]][contributors-url]
[![Forks][forks-shield]][forks-url]
[![Stargazers][stars-shield]][stars-url]
[![Issues][issues-shield]][issues-url]
[![MIT License][license-shield]][license-url]
[![LinkedIn][linkedin-shield]][linkedin-url]

<!-- TABLE OF CONTENTS -->
<details>
<summary>Tabla de contenidos</summary>
<ol>

</ol>
</details>

<br />
<div align="center">
  <a href="https://github.com/SBenitezL/coocking">
    <img src="source/logo.jpg" alt="Logo" width="80" height="80">
  </a>

<h3 align="center">Coocking</h3>

  <p align="center">
    He creado este proyecto para practicar y mejorar mis habilidades de desarrollo full-stack, combinando Java para el backend y Angular para el frontend. El objetivo es construir una aplicación completa, desde la lógica del dominio hasta la interfaz de usuario, para afianzar mis conocimientos en ambas tecnologías. Elegí un proyecto de gestión de recetas porque me permite practicar conceptos clave como la persistencia de datos, el manejo de peticiones HTTP y la creación de una interfaz de usuario intuitiva. Usaré Spring Boot para el backend, MySQL para la base de datos, y Angular para el frontend, lo que me permitirá explorar diferentes aspectos del desarrollo full-stack. Espero que este proyecto me ayude a fortalecer mis habilidades y a construir una aplicación funcional y eficiente.
    <br />
    <a href="https://github.com/SBenitezL/coocking"><strong>Explore the docs »</strong></a>
    <br />
    <br />
    <a href="https://github.com/SBenitezL/coocking">View Demo</a>
    ·
    <a href="https://github.com/SBenitezL/coocking/issues/new?labels=bug&template=bug-report---.md">Report Bug</a>
    ·
    <a href="https://github.com/SBenitezL/coocking/issues/new?labels=enhancement&template=feature-request---.md">Request Feature</a>

<a href="https://github.com/SBenitezL/coocking/blob/master/source/domain.md">Domain</a>

  </p>
</div>

<!-- ABOUT THE PROJECT -->

# Acerca del Proyecto

## Requisitos Funcionales

---

### Gestión de Usuarios

1. **Registro de usuarios**: El sistema debe permitir que nuevos usuarios se registren proporcionando correo electrónico, nombre y contraseña.
2. **Autenticación de usuarios**: El sistema debe permitir que los usuarios inicien sesión y cierren sesión de forma segura.

### Publicación de Recetas

1. **Creación de recetas**: El usuario podrá crear nuevas recetas incluyendo:
   - Título
   - Imagen (opcional)
   - Ingredientes (lista)
   - Pasos de preparación (paso a paso)
2. **Edición de recetas**: El usuario podrá editar sus recetas publicadas.
3. **Eliminación de recetas**: El usuario podrá eliminar sus propias recetas.

### Procesamiento de Recetas

1. **Análisis de contenido**: El sistema debe procesar la receta subida (ingredientes, pasos, título) para asociarla automáticamente a uno o más **estados de ánimo** (por ejemplo: feliz, nostálgico, energético, relajado).
2. **Asignación manual de estado de ánimo** (opcional): El usuario puede sugerir un estado de ánimo para su receta al publicarla.

### Búsqueda y Filtrado

1. **Búsqueda de recetas**: El sistema permitirá buscar recetas por:
   - Nombre de receta
   - Ingredientes disponibles
   - Estado de ánimo asociado
2. **Filtro por ingredientes**: El usuario podrá ingresar los ingredientes que tiene disponibles y ver recetas que pueda preparar con ellos.
3. **Filtro por estado de ánimo**: El usuario podrá filtrar recetas asociadas a un estado de ánimo específico.

### Visualización de Recetas

1. **Detalle de receta**: Al seleccionar una receta, el usuario podrá ver:
   - Nombre
   - Imagen
   - Ingredientes
   - Pasos detallados
   - Estado(s) de ánimo asociados
2. **Listado de recetas**: El sistema mostrará un listado de recetas destacadas, recientes o populares.

### Funcionalidades Sociales (opcional para una segunda versión)

1. **Valoraciones y comentarios**: Los usuarios podrán calificar y comentar recetas.
2. **Guardar recetas favoritas**: Los usuarios podrán guardar recetas en una lista de favoritos.

### Administración del Sistema

1. **Moderación de contenido**: Los administradores podrán revisar y eliminar recetas que infrinjan políticas de la aplicación.
2. **Gestión de estados de ánimo**: Los administradores podrán gestionar (crear/editar/eliminar) los estados de ánimo disponibles en el sistema.

---

<p align="right">(<a href="#readme-top">back to top</a>)</p>

## Habilidades puestas en práctica

- Creación de variables
- Operadores
- Sentencias condicionales
- Ciclos
- Funciones
<p align="right">(<a href="#readme-top">back to top</a>)</p>

## Tecnologias

- [![Java][Java-shield]][Java-link]

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->

[contributors-shield]: https://img.shields.io/github/contributors/SBenitezL/coocking.svg?style=for-the-badge
[contributors-url]: https://github.com/SBenitezL/coocking/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/SBenitezL/coocking.svg?style=for-the-badge
[forks-url]: https://github.com/SBenitezL/coocking/network/members
[stars-shield]: https://img.shields.io/github/stars/SBenitezL/coocking.svg?style=for-the-badge
[stars-url]: https://github.com/SBenitezL/coocking/stargazers
[issues-shield]: https://img.shields.io/github/issues/SBenitezL/coocking.svg?style=for-the-badge
[issues-url]: https://github.com/SBenitezL/coocking/issues
[license-shield]: https://img.shields.io/github/license/SBenitezL/coocking.svg?style=for-the-badge
[license-url]: https://github.com/SBenitezL/coocking/blob/master/LICENSE.txt
[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
[linkedin-url]: https://linkedin.com/in/santiago-benitez-lopez
[Java-shield]: https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white
[Java-link]: https://www.oracle.com/java/technologies/javase/jdk17-archive-downloads.html
