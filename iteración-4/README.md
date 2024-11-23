# Indice

- [Gestión de la iteración](#gestión-de-la-iteración)
  - [Definición del marco de trabajo](#definición-del-marco-de-trabajo)
  - [Planificación de la iteración](#planificación-de-la-iteración)
  - [Seguimiento de la iteración](#seguimiento-de-la-iteración)
  - [Inspección y adaptación del proceso](#inspección-y-adaptación-del-proceso)
- [Construir y validar posibles soluciones del MVP a través de prototipos.](#construir-y-validar-posibles-soluciones-del-mvp-a-través-de-prototipos)
  - [Prototipos finales](#prototipos-finales)

_<span style="color:red">[Existe la elaboración de un informe académico que resume los resultados y reflexiona sobre las lecciones aprendidas
sobre las prácticas de ingeniería de software ágil. El informe académico deberá ser implementado como un archivo de
markdown en el propio repositorio de github.]</span>

# Informe académico

## Descripción del proyecto

El proyecto consiste en desarrollar una aplicación móvil para que restaurantes puedan gestionar sus reservas.
Los clientes podrán ver las recomendaciones de restaurantes cerca de su ubicación, ver sus reseñas y evaluar, tipos de comida, ver disponibilidad y realizar reservas.
Los gerentes de restaurantes podrán gestionar las reservas y las mesas disponibles.

## Resumen de los resultados

Se completaron todas las funcionalidades prioritarias para los perfiles de cliente, gerente y administrador, destacando:
- Login, registro y edición de usuarios.
- Creación y cancelación de reservas.
- Gestión de notificaciones y restaurantes.
- Configuración de promociones y respuesta a comentarios para gerentes.

#### Prototipos en Figma:
Se desarrollaron prototipos interactivos que simulan flujos clave de la aplicación, desde el registro hasta la reserva y gestión de restaurantes. Estos prototipos fueron revisados y validados con usuarios finales, identificando oportunidades de mejora en la estética y usabilidad.

#### Validación y ajustes:
Las pruebas de usabilidad destacaron la claridad en la navegación, pero también identificaron áreas para optimizar, como:
- Hacer la interfaz más moderna y atractiva.
- Implementar filtros avanzados en la búsqueda de restaurantes.
- Mejorar los mensajes de confirmación visual y la gestión de notificaciones.

#### Resultados finales:
Cumplimos con los objetivos de cada iteración, logrando una velocidad promedio de 24 puntos de historia por sprint.
Se establecieron bases sólidas para continuar con el desarrollo del producto, priorizando funcionalidades como un sistema de recompensas y personalización avanzada.

## Reflexiones sobre las prácticas de ingeniería de software ágil
Utilizamos el marco de trabajo SCRUM para desarrollar el prototipo de una aplicación de restaurantes, siguiendo roles, eventos y artefactos definidos.

#### Adaptación de roles y eventos:
Los roles de Product Owner, Scrum Master y Development Team estuvieron bien definidos, con responsabilidades claras que facilitaron la organización y ejecución de tareas.
Las ceremonias SCRUM fueron adecuadas para el ritmo y complejidad del proyecto. Las reuniones se realizaron algunas presencialmente y otras mediante Discord, lo que permitió flexibilidad y una buena colaboración del equipo.

#### Gestión del trabajo y uso de herramientas:
Azure DevOps fue esencial para el seguimiento del progreso, principalmente el uso del product backlog y el sprint backlog y también las burndown charts que permitieron una visualización clara del desempeño en cada iteración.
La priorización mediante puntos de historia y categorías ayudó a enfocar los esfuerzos en las tareas mas importantes.

#### Retrospectiva:
Las retrospectivas proporcionaron un espacio valioso para reflexionar sobre el proceso y aplicar ajustes. Por ejemplo, se identificaron problemas de coordinación en el uso de Figma, lo que impulsó una revisión para evitar duplicidades en los prototipos.

#### Incorporación de feedback del usuario:
Los comentarios de usuarios finales fueron incorporados para ajustar la interfaz y las funcionalidades del prototipo, alineándolo mejor con las expectativas de los usuarios.

# Gestión de la iteración

## Definición del marco de trabajo

### Artefactos principales
**Eventos SCRUM**
- **Sprint Planning:** Se realizaron de manera presencial en la facultad o en discord, donde se definieron los objetivos del sprint y las tareas más prioritarias y sus story points.
- **Daily Scrum:** Se llevaron a cabo principalmente de manera presencial en la facultad, por WhatsApp o Discord. No fue necesario realizar daily meetings todos los días, y en algunos casos se implementaron mediante breves llamadas a través de Discord.
- **Sprint Review:** Se realizó al final de cada sprint para presentar el incremento del producto a los interesados clave.
- **Sprint Retrospective:** Esta ceremonia se llevó a cabo al final de cada sprint para discutir mejoras en los procesos y reflexionar sobre lo que funcionó y lo que puede optimizarse en los siguientes sprints.

#### Justificación de las adaptaciones principales del marco de trabajo al contexto del proyecto
Adaptamos la frecuencia de las daily scrums a la necesidad del equipo, realizándolas solo cuando era necesario.
A veces se realizaban en la facultad, otras veces por WhatsApp o Discord.

#### Definición del calendario de eventos con justificación de su adaptación al contexto de la iteración.
Seguimos el calendario planteado originalmente, respetando las fechas finales de las iteraciones y las ceremonias SCRUM.


#### Roles y responsabilidades definidos para cada integrante del equipo.
**Roles y responsabilidades del equipo**
- **Product Owner:** Magdalena Arza
  - Prioriza el Product Backlog y asegura que el equipo trabaje en las historias de mayor valor para el proyecto.
- **SCRUM Master:** Martín Salaberry
  - Facilita las ceremonias SCRUM, elimina obstáculos y asegura que se respeten las buenas prácticas del marco.
- **Development Team:** Joaquín Struyas, Martin Salaberry, Magdalena Arza
  - Encargados de desarrollar las historias de usuario planificadas en cada sprint, garantizando que el incremento del producto esté listo al finalizar la iteración.

## Políticas de trabajo del equipo:
### Definition of Done.
1. La historia cumple con todos los criterios de aceptación definidos al inicio.
2. El diseño visual y de interacción ha sido completado en Figma, con todos los elementos y componentes alineados a las guidelines establecidas.
3. La historia ha sido integrada en el prototipo de Figma de manera que el flujo se pueda navegar de forma intuitiva y sin errores.
4. El Product Owner ha revisado y aprobado el diseño final en Figma.

### Definition of Ready.
1. La historia cuenta con especificaciones visuales y de diseño claras, incluyendo cualquier guideline de estilo.
2. Cada historia tiene criterios de aceptación específicos que describen cómo debe funcionar y visualizarse el componente o flujo en Figma.
3. El Product Owner priorizó la historia como esencial para el sprint actual.



## Planificación de la iteración


#### Minuta de la sprint planning con su agenda, actividades y resultados.
Como resultado del sprint planning obtuvimos los objetivos de la iteración. 

#### Objetivos de la iteración
Para esta iteración, la última del release, se planificó realizar el informe y la presentación final del proyecto. 

- Como el objetivo de la iteración es realizar el informe y la presentación final del proyecto, no se planificaron historias de usuario ni tareas asociadas.
Por lo tanto, no planificamos en base a la capacidad del equipo ni utilizamos el backlog.


## Seguimiento de la iteración

### Minuta de daily scrum describiendo la coordinación del trabajo de cada integrante del equipo.
<span style="color:red">[TODO]</span>
Fecha: 21/11/2024
Hora: 15:00

#### Organización para la grabación del video:
**Magdalena Arza:** Explicará las funcionalidades relacionadas con el gerente y realizará la edición de los videos.
**Martín Salaberry:** Presentará las características del perfil del cliente.
**Joaquín Struyas:** Explicará las funcionalidades del perfil del administrador, como la creación de restaurantes y registro de gerentes.

#### Errores y partes faltantes del prototipo:
Ajustar los márgenes y espaciado en las pantallas del perfil del gerente.
Corregir los colores de los botones para que sean consistentes en toda la aplicación.
Añadir una confirmación visual al realizar acciones como agregar favoritos o cancelar reservas.
Incorporar una pantalla faltante para la gestión de comentarios por parte del administrador.


La reunion duró aproximadamente 1 hora


### Registro y reporte de horas de cada integrante del equipo con sus actividades principales.

### Iteracion 1
**Equipo** 
- Historias de usuario y sprint backlog: 2 horas 
- Sprint retrospective: 15 min

**Arza**
- Estudio de competidores: 1 hora 

**Arza y Struyas** 
- Story Map: 30 min 

**Salaberry** 
- Epicas: 1 hora


### Iteracion 2
**Arza**
- 22/10 : 1 hora
- 24/10 : 3 horas

**Salaberry**
- 22/10 : 1 hora
- 23/10 : 3 horas

**Struyas**
- 22/10 : 1 hora
- 23/10 : 2 horas
- 24/10 : 1 hora

### Iteracion 3
**Arza**
- Historias de usuario del gerente 2 horas
- Documentación 2 horas

**Salaberry**
- Historias de usuario del cliente 3 horas

**Struyas**
- Historias de usuario del administrador 3 horas
- Documentación 1 hora

### Iteracion 4
  **Arza**
- Video presentación 2 horas
- Documentación 1 hora

**Salaberry**
- Video presentación 2 horas
- Documentacion 1 hora

**Struyas**
- Video presentación 2 horas
- Documentación 1 hora

#### Seguimiento visual de la iteración con burndown y/o burnup charts
No hay seguimiento ya que no definimos tareas ni historias de usuario, tampoco usamos el backlog.

## Inspección y adaptación del proceso

_<span style="color:red">[Existe evidencia sobre la inspección del proceso con aprendizajes principales y acciones de mejora implementadas durante el desarrollo del proyecto.]_

### Artefactos principales

- Minuta de la retrospectiva con la dinámica utilizada y sus principales resultados. [TODO]
- Planificación y seguimiento de las acciones de mejora.

# Construir y validar posibles soluciones del MVP a través de prototipos

## Prototipos finales

_<span style="color:red">[Se evidencian los prototipos finales con las validaciones de los usuarios. Los prototipos deberán ser exportados en algún formato de imagen (como png o jpg) a efectos de poder ser visualizados fácilmente dentro del propio repo de github.]_


### Artefactos principales

## Prototipos interactivos finales con el feedback de las validaciones.
[Prototipo perfil administrador](https://www.figma.com/proto/BYvhnvacIuyWrmaI2aCwkn/Obligatorio-ISA?node-id=287-2646&node-type=canvas&t=IEOOjdqoqMzFfxcY-1&scaling=scale-down&content-scaling=fixed&page-id=287%3A2605&starting-point-node-id=287%3A2646)
[Prototipo perfil cliente](https://www.figma.com/proto/BYvhnvacIuyWrmaI2aCwkn/Obligatorio-ISA?node-id=165-1170&node-type=canvas&t=ZMpFgfFfSGATHKbQ-1&scaling=scale-down&content-scaling=fixed&page-id=5%3A4&starting-point-node-id=165%3A1170&show-proto-sidebar=1)
[Prototipo perfil gerente](https://www.figma.com/proto/BYvhnvacIuyWrmaI2aCwkn/Obligatorio-ISA?node-id=494-2010&node-type=canvas&t=jsyroM8cRIr85dXH-1&scaling=scale-down&content-scaling=fixed&page-id=136%3A897&starting-point-node-id=494%3A2010)

## Prototipos asociados como bocetos a las historias de usuario. [TODO]

## Lista de mejoras sugeridas de las validaciones con usuarios finales [TODO]
  - <span style="color:red">Se explicita que mejoras fueron implementadas en los prototipos y cuáles quedaron fuera del alcance del proyecto.
