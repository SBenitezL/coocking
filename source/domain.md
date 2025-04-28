<a id="readme-top"></a>

# COOCKING

<details>
<summary>Tabla de contenidos</summary>

1. <a href='#introducción'>**Introducción**</a>
2. <a href='#objetivo-del-documento'>**Objetivo del Documento**</a>
3. <a href='#alcance'>**Alcance**</a>
4. <a href='#lenguaje-oblicuo'>**Lenguaje Oblicuo**</a>
   - 4.1 <a href='#definiciones-principales'>Definiciones principales</a>
   - 4.2 <a href='#términos-secundarios'>Términos secundarios</a>
5. <a href='#reglas-de-negocio'>**Reglas de Negocio**</a>
   - 5.1 <a href='#gestión-de-usuarios'>Gestión de Usuarios</a>
   - 5.2 <a href='#publicación-de-recetas'>Publicación de Recetas</a>
   - 5.3 <a href='#procesamiento-y-asignación-de-estado-de-ánimo'>Procesamiento y Asignación de Estado de Ánimo</a>
   - 5.4 <a href='#búsqueda-y-filtrado-de-recetas'>Búsqueda y Filtrado de Recetas</a>
   - 5.5 <a href='#moderación-de-contenido'>Moderación de Contenido</a>
6. <a href=''>**Consideraciones Especiales**</a>
   - 6.1 <a href='#asignación-de-estado-de-ánimo-basado-en-ia'> Asignación de Estado de Ánimo Basado en IA
     </a>
   - 6.2 <a href='#tolerancia-a-ingredientes-parciales'>Tolerancia a Ingredientes Parciales </a>
   - 6.3 <a href='#multiplataforma'>Multiplataforma</a>
   - 6.4 <a href='#personalización-y-recomendaciones'>Personalización y Recomendaciones</a>
   - 6.5 <a href='#escalabilidad-del-sistema'>Escalabilidad del Sistema</a>
7. <a href=''>**Glosario**</a>
8. <a href=''>**Anexos**</a>
</details>

## Introducción

El presente documento define el lenguaje oblicuo y las reglas de negocio de la aplicación de recetas denominada **Cooking**. El propósito es establecer un marco común de comunicación entre los usuarios, desarrolladores y equipos de negocio, garantizando la coherencia y claridad en la interpretación de los conceptos y comportamientos del sistema.

La aplicación permitirá a los usuarios crear, compartir y descubrir recetas, asociándolas automáticamente a estados de ánimo basados en los ingredientes y pasos de preparación. Además, ofrecerá filtros inteligentes para buscar recetas según los ingredientes disponibles o el estado emocional deseado.

El lenguaje oblicuo proporciona una serie de términos clave que serán utilizados de manera consistente en toda la documentación y durante el desarrollo. Las reglas de negocio definen las condiciones, restricciones y procedimientos que rigen el comportamiento de la aplicación, asegurando el cumplimiento de los objetivos funcionales y una experiencia de usuario coherente.

Este documento servirá como referencia viva durante todo el ciclo de vida del proyecto, desde la fase de análisis hasta su implementación y mantenimiento.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

## Objetivo del documento

El objetivo de este documento es definir de manera precisa el lenguaje oblicuo y las reglas de negocio que rigen el funcionamiento de la aplicación de recetas.

Busca establecer un marco común para todos los participantes del proyecto —usuarios, analistas, diseñadores, desarrolladores y testers— garantizando una interpretación consistente de los conceptos y una implementación alineada con los requerimientos de negocio.

Concretamente, este documento pretende:

Formalizar los términos clave que serán utilizados en toda la comunicación y documentación del sistema.

Definir las reglas que determinarán el comportamiento de las funcionalidades principales, incluyendo la publicación, clasificación y búsqueda de recetas.

Servir como referencia durante las fases de análisis, diseño, desarrollo, pruebas y mantenimiento de la aplicación.

Reducir ambigüedades y malentendidos en las decisiones de diseño y construcción del producto.

El uso de este documento contribuye a asegurar que la aplicación cumpla con los objetivos de negocio, brinde una experiencia de usuario coherente, y permita su evolución futura de manera controlada.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

## Alcance

Este documento abarca la definición de los términos clave (lenguaje oblicuo) y las reglas de negocio que estructuran el funcionamiento de la aplicación de recetas **COOCKING**.

El alcance incluye:

La gestión de usuarios que podrán registrarse, iniciar sesión y administrar sus recetas.

La creación, edición y eliminación de recetas por parte de los usuarios, especificando ingredientes y pasos de preparación.

El procesamiento automático de las recetas para asociarlas a uno o varios estados de ánimo relevantes.

La funcionalidad de búsqueda y filtrado de recetas, basada en los ingredientes disponibles del usuario y/o en el estado de ánimo deseado.

La visualización de recetas con su detalle completo, incluyendo sus ingredientes, pasos y estado emocional asociado.

La gestión administrativa de contenidos para mantener la calidad y adecuación de las recetas publicadas.

La definición de los estados de ánimo predefinidos y la forma en que el sistema los asigna a cada receta.

Este documento no contempla aspectos técnicos de implementación detallada (como tecnologías específicas, arquitectura de sistemas o diseño de base de datos), ni procesos de marketing o comercialización de la aplicación.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

## Lenguaje oblicuo

El lenguaje oblicuo define los términos específicos que serán utilizados de forma consistente a lo largo del desarrollo, implementación y documentación de la aplicación.

Estos términos representan conceptos del negocio y ayudan a alinear la comunicación entre los equipos técnicos y no técnicos, evitando malentendidos y ambigüedades.

A continuación, se presentan las definiciones de los términos principales y secundarios:

### Definiciones principales

| Término                | Definición                                                                                                                                                                  |
| ---------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Usuario                | Persona que se registra en la aplicación para crear, gestionar, buscar o interactuar con recetas.                                                                           |
| Receta                 | Conjunto de instrucciones y lista de ingredientes que describen cómo preparar un platillo o bebida. Incluye título, imagen (opcional), ingredientes y pasos de preparación. |
| Ingrediente            | Elemento o producto alimenticio que forma parte de la preparación de una receta.                                                                                            |
| Paso de Preparación    | Instrucción específica que describe una acción que el usuario debe realizar durante la elaboración de la receta.                                                            |
| Estado de Ánimo        | Categoría emocional (por ejemplo: feliz, nostálgico, relajado) que se asigna a una receta según sus ingredientes, pasos y contexto general.                                 |
| Ingrediente Disponible | Ingrediente que el usuario indica que tiene en su posesión y que puede ser utilizado para preparar recetas.                                                                 |
| Filtro                 | Herramienta de búsqueda que permite al usuario restringir las recetas mostradas según criterios como ingredientes disponibles o estado de ánimo.                            |

### Términos secundarios

| Término         | Definición                                                                                                          |
| --------------- | ------------------------------------------------------------------------------------------------------------------- |
| Receta Favorita | Receta que un usuario ha marcado para guardar en su lista personal de favoritas.                                    |
| Comentario      | Opinión o retroalimentación que un usuario deja en una receta publicada.                                            |
| Valoración      | Calificación que un usuario asigna a una receta, generalmente en forma de estrellas o puntaje.                      |
| Moderación      | Proceso de revisión de recetas y comentarios para asegurar que cumplan con las políticas y normas de la aplicación. |

<p align="right">(<a href="#readme-top">back to top</a>)</p>

## Reglas de negocio

Las reglas de negocio definen los principios, restricciones y comportamientos que deben cumplirse en la aplicación para garantizar su correcto funcionamiento, de acuerdo con los objetivos planteados.

### Gestión de usuarios

- Registro Obligatorio: Todo usuario debe registrarse para crear, editar, eliminar o guardar recetas.

- Datos mínimos requeridos: Para registrarse, el usuario debe proporcionar un correo electrónico válido, un nombre de usuario y una contraseña segura.

- Roles de usuario: Existen al menos dos roles: Usuario Común y Administrador.

  - El Usuario Común puede gestionar sus propias recetas, buscar y guardar recetas de otros.

  - El Administrador puede gestionar usuarios, recetas públicas y estados de ánimo.

### Publicación de recetas

- Creación de receta: Toda receta debe contener al menos un título, una lista de ingredientes y un mínimo de un paso de preparación.

- Imagen opcional: Las recetas pueden tener una imagen asociada, pero no es obligatoria para su publicación.

- Propiedad de receta: Cada receta está asociada al usuario que la creó y solo él puede editarla o eliminarla (excepto el administrador).

- Contenido adecuado: Las recetas no deben contener contenido ofensivo o inapropiado; de detectarse, serán eliminadas por un administrador.

### Procesamiento y asignación de estado de ánimo

- Asignación automática: Al crear una receta, el sistema analizará los ingredientes y pasos para sugerir uno o más estados de ánimo asociados.

- Corrección manual: El usuario podrá proponer un estado de ánimo diferente si lo considera necesario, sujeto a validación automática del sistema (opcional).

- Múltiples estados: Una receta puede estar asociada a más de un estado de ánimo.

### Búsqueda y filtrado de recetas

- Filtro de ingredientes: El usuario podrá ingresar una lista de ingredientes y el sistema mostrará recetas que puedan elaborarse con esos ingredientes (total o parcialmente).

- Filtro de estado de ánimo: El usuario podrá seleccionar uno o más estados de ánimo para filtrar recetas que correspondan a dichos estados.

- Combinación de filtros: El usuario podrá combinar filtros de ingredientes y estado de ánimo para obtener resultados más precisos.

### Moderación de contenido

- Revisión de reportes: Los usuarios podrán reportar recetas inapropiadas, las cuales deberán ser revisadas por un administrador.

- Eliminación justificada: Toda eliminación de contenido debe registrarse indicando el motivo para mantener un historial de acciones administrativas.

- Actualización de estados de ánimo: Los administradores pueden actualizar, agregar o eliminar estados de ánimo disponibles en la aplicación conforme evolucionen las necesidades del negocio.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

## Consideraciones especiales

Este apartado describe aspectos que, aunque no forman parte directamente de los requisitos funcionales o reglas básicas, son importantes para el correcto uso, crecimiento y mantenimiento de la aplicación.

### Asignación de estado de ánimo basado en IA

- La asignación de estados de ánimo puede mejorarse progresivamente mediante técnicas de inteligencia artificial o aprendizaje automático, basándose en análisis de texto de ingredientes y pasos de recetas.

- En las primeras versiones, el sistema utilizará reglas básicas (keywords, análisis de tono) para sugerir estados de ánimo.

- Las recetas con asignación automática podrán ser re-evaluadas conforme se mejoren los algoritmos del sistema.

### Tolerancia a ingredientes parciales

- El sistema debe permitir mostrar recetas en las cuales el usuario no tenga todos los ingredientes pero sí un porcentaje alto (por ejemplo, al menos el 70%), sugiriendo ingredientes faltantes para completar la receta.

- Esta tolerancia será configurable por parámetros de negocio.

### Multiplataforma

- La aplicación deberá diseñarse pensando en su disponibilidad tanto en formato web como móvil.

- La experiencia de usuario debe ser consistente entre plataformas, respetando sus particularidades.

### Personalización y recomendaciones

- En versiones futuras, se planea incluir un motor de recomendaciones basado en las preferencias de búsqueda, recetas favoritas y estados de ánimo más seleccionados por cada usuario.

- La privacidad de los datos deberá ser garantizada en todo momento, respetando normativas de protección de datos personales.

### Escalabilidad del sistema

- La aplicación deberá estructurarse de modo que soporte el crecimiento en el número de usuarios, recetas publicadas y consultas simultáneas.

- El diseño de bases de datos, servicios de búsqueda y procesamiento automático debe considerar opciones de escalabilidad horizontal.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

## Glosario

| Término                      | Definición                                                                                                                                              |
| ---------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Usuario                      | Persona registrada en la aplicación que puede crear, editar, buscar y guardar recetas.                                                                  |
| Administrador                | Usuario con permisos especiales para gestionar el contenido y moderar la plataforma.                                                                    |
| Receta                       | Documento creado por un usuario que contiene un título, imagen (opcional), lista de ingredientes y pasos detallados para preparar un platillo o bebida. |
| Ingrediente                  | Elemento alimenticio utilizado para elaborar una receta.                                                                                                |
| Ingrediente Disponible       | Ingrediente que el usuario declara tener a mano para buscar recetas que pueda cocinar.                                                                  |
| Paso de Preparación          | Acción específica que el usuario debe realizar para avanzar en la elaboración de una receta.                                                            |
| Estado de Ánimo              | Categoría emocional asignada a una receta para asociarla a una experiencia sensorial o emocional (por ejemplo, "feliz", "relajado", "nostálgico").      |
| Filtro                       | Herramienta que permite restringir la búsqueda de recetas según ingredientes disponibles, estado de ánimo, entre otros criterios.                       |
| Valoración                   | Calificación que un usuario asigna a una receta publicada, generalmente en forma de estrellas o puntaje.                                                |
| Comentario                   | Opinión escrita que un usuario deja en una receta para compartir su experiencia o sugerencias.                                                          |
| Moderación                   | Proceso de revisión de contenido publicado para asegurar que cumpla con las políticas de la aplicación.                                                 |
| IA (Inteligencia Artificial) | Tecnología utilizada para analizar el contenido de las recetas y asignar estados de ánimo de forma automatizada.                                        |
| Escalabilidad                | Capacidad del sistema para adaptarse y funcionar eficientemente al aumentar el volumen de usuarios y datos.                                             |

<p align="right">(<a href="#readme-top">back to top</a>)</p>

## Anexos

<p align="right">(<a href="#readme-top">back to top</a>)</p>
