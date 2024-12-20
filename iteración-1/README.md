# Indice

- [Gestión de la iteración](#gestión-de-la-iteración)
  - [Definición del marco de trabajo](#definición-del-marco-de-trabajo)
- [Planificación de la iteración](#planificación-de-la-iteración)
  - [Seguimiento de la iteración](#seguimiento-de-la-iteración)
- [Identificar y definir el problema a resolver](#identificar-y-definir-el-problema-a-resolver)
  - [Identificación del problema a resolver](#identificación-del-problema-a-resolver)
  - [Definición del problema/solución](#definición-del-problema/solución)
- [Product Backlog](#product-backlog)
  - [Epicas](#epicas)
  - [Definition of Ready](#definition-of-ready-dor)
  - [Definition of Done](#definition-of-done-dod)
  - [Historias de usuario](#historias-de-usuario)
  - [Story map](#story-map)

# Gestión de la iteración

## Definición del marco de trabajo
**Roles y responsabilidades del equipo**
- Product Owner: Magdalena Arza
	- Prioriza el Product Backlog y asegura que el equipo trabaje en las historias de mayor valor para el proyecto.
- SCRUM Master: Martín Salaberry
	- Facilita las ceremonias SCRUM, elimina obstáculos y asegura que se respeten las buenas prácticas del marco.
- Development Team: Joaquín Struyas
	- Encargado de desarrollar las historias de usuario planificadas en cada sprint, garantizando que el incremento del producto esté listo al finalizar la iteración.

**Eventos SCRUM**
- Sprint Planning: Se realizó de manera presencial en la facultad, donde se definieron los objetivos del sprint y las tareas más prioritarias y sus story points.
- Daily Scrum: Se llevaron a cabo principalmente de manera presencial en la facultad. Sin embargo, al ser un sprint relativamente corto, no fue necesario realizar daily meetings todos los días, y en algunos casos se implementaron mediante breves llamadas a través de Discord.
- Sprint Review: Se realizó al final de cada sprint para presentar el incremento del producto a los interesados clave.
- Sprint Retrospective: Esta ceremonia se llevó a cabo para discutir mejoras en los procesos y reflexionar sobre lo que funcionó y lo que puede optimizarse en los siguientes sprints.
  
# Planificación de la iteración

### Seguimiento de horas
- Equipo - 2 hs - Historias de usuario y sprint backlog
- Arza - 1 h - Estudio de competidores
- Arza y Struyas - 30 min - Story map
- Salaberry - 1 h - Epicas
- Equipo - 15 min - Sprint retrospective 

### Sprint retrospective

Al finalizar la iteración, nos reunimos para hacer la sprit retrospective, utilizamos la extensión retorspective en azure devops.

![Restrospective](./imagenes/retrospective.png)

### Acciones de mejora

- Decidir si agregar historias de usuario a partir del estudio de competidores.

## Identificación del problema a resolver
**Problema del negocio**
El proyecto busca resolver la falta de una plataforma eficiente para reservar y evaluar restaurantes, especialmente para personas que prefieren gestionar todo desde una aplicación móvil. Actualmente, no hay soluciones que integren de manera óptima la gestión de reservas, evaluaciones de usuarios y una comunicación directa con los restaurantes.

**Usuarios y escenarios principales**
- Clientes: Usuarios que buscan restaurantes, realizan reservas y dejan reseñas.
  Valor: Comodidad para encontrar, reservar y evaluar restaurantes desde una sola aplicación.
- Gerentes de restaurantes: Administran reservas, reciben feedback y gestionan la reputación del restaurante.
  Valor: Mejora en la gestión de reservas y visibilidad del restaurante mediante las reseñas de clientes.
- Administradores del sistema: Supervisan la plataforma, verifican las reseñas y resuelven incidencias.
  Valor: Control de calidad y mejora continua del servicio.

### Interesados (Stakeholders)

#### Clientes:
Personas que usan la aplicación para buscar, reservar y evaluar restaurantes.

**Necesidades:**
- Poder registrarse e iniciar sesión.
- Marcar restaurantes como favoritos.
- Reservar mesas en restaurantes.
- Configurar notificaciones de promociones y recomendaciones.
- Visualizar las puntuaciones y comentarios de restaurantes.

#### Gerentes:
Encargados de gestionar restaurantes dentro de la aplicación.

**Necesidades:**
- Confirmar y gestionar reservas.
- Modificar detalles del restaurante.
- Gestionar promociones y recibir notificaciones sobre reservas solicitadas.
- Apelar puntuaciones o comentarios recibidos.

#### Administradores:
Personal que gestiona los gerentes y los restaurantes registrados.

**Necesidades:**
- Dar de alta y modificar gerentes.
- Dar de alta restaurantes.
- Moderar y administrar comentarios y puntuaciones de restaurantes.
- Análisis y estudio de competidores.

### Estudio de competidores
#### Meitre
Es una plataforma de pedidos y reservas de restaurantes que buscan mayor control sobre sus reservas y la experiencia del cliente. 

“La plataforma de la compañía aprovecha la tecnología para reservar tablas basadas en las tendencias de la demanda, rotar tablas de manera eficiente, introducir técnicas de precios y organizar eventos, lo que permite a los clientes eliminar no-shows, reducir las tasas de cancelación y asignar la demanda de manera eficiente.”

A partir de las funcionalidades que detallan en su página web, se nos ocurre que podríamos incluir algunas de ellas que creemos tienen sentido en nuestra aplicación. 

- Alertas por Whatsapp y SMS automáticas.
- Confirmaciones por email y evaluaciones.
- Prevención de no-show (clientes que no asisten sin cancelar) con tarjeta de crédito.
- Lista de espera automática para sustituir cancelaciones.
- Rastreador de redes sociales.

#### TheFork
TheFork es una plataforma líder en reservas de restaurantes en línea, que conecta a los usuarios con más de 55,000 restaurantes en Europa y Australia. 
Los usuarios pueden hacer reservas en tiempo real, con confirmaciones instantáneas las 24 horas del día, y acceder a ofertas especiales. Además, TheFork ofrece millones de reseñas verificadas, ayudando a los comensales a elegir los mejores restaurantes basándose en opiniones confiables.

De las funcionalidades que ofrecen, tomamos como más adaptables a nuestro negocio las siguientes:
- Posibilidad de agregar promociones a los restaurantes.
- Información sobre el precio promedio de una comida en ese restaurante.
- Menú del restaurante.

#### OpenTable
“OpenTable es una aplicación de reserva de restaurantes que proporciona una solución de servicio completa para cualquier restaurante. Trae un fuerte motor de marketing y herramientas de gestión de invitados que puede utilizar para comprender más a los clientes y proporcionar experiencias de clase alta a los clientes.“

“OpenTable también es un libro de registro de reservas electrónico que tiene funciones de pantalla táctil para simplificar el trabajo para sus gerentes.“

- OpenTable ofrece un sistema de fidelización con puntos para obtener recompensas.
- Opciones para reservas de eventos especiales.

En resumen, el análisis de Meitre, TheFork y OpenTable nos muestra que cada plataforma ofrece características únicas para optimizar la experiencia de reservas en restaurantes. Meitre se centra en la eficiencia de reservas y la reducción de no-shows, mientras que TheFork proporciona acceso a reseñas verificadas y promociones para atraer a los comensales. Por último, OpenTable se destaca por su motor de marketing y un sistema de fidelización que recompensa a los usuarios. Integrar las mejores funcionalidades de estas plataformas en nuestra aplicación nos permitirá crear una solución competitiva y adaptada a las necesidades del mercado.

# Product Backlog

Realizamos el backlog en Azure DevOps: [link](https://dev.azure.com/JS292128/Obligatorio%20ISA1)

## Epicas
- Gestión de cuentas de usuario: facilitar acceso a la plataforma a los clientes mediante creación y gestión de sus cuentas.
- Gestión de reservas: los clientes deben poder realizar y gestionar sus reservas de manera eficiente.
- Personalizar experiencia de usuario: los usuarios deberán disponer de funciones que mejoren su experiencia a través de la personalización de su entorno, como favoritos y notificaciones.
- Gestión de restaurantes: los gerentes deben disponer de herramientas para gestionar la información y disponibilidad de los restaurantes bajo su control.
- Gestión de comentarios y valoraciones: permitir a usuarios valorar y comentar sobre sus experiencias en los negocios, y a los gerentes responder y visualizar este feedback.
- Integración de promociones y descuentos: se deben implementar con el objetivo de atraer clientes, facilitando su descubrimiento son filtros y notificaciones.

## Definition of Ready (DoR)

- La historia de usuario está claramente descrita y entendida por el equipo de diseño.
- Los criterios de aceptación están definidos y son claros.
- Las dependencias están identificadas y gestionadas.
- Los requisitos no funcionales están especificados.
- La historia de usuario está priorizada.

## Definition of Done (DoD)

- La funcionalidad cumple con los criterios de aceptación, sin errores y con tiempos de respuesta aceptables.
- Se validan correctamente los campos requeridos y se muestran mensajes de error descriptivos cuando corresponda.
- El acceso está restringido a usuarios autenticados y autorizados, siguiendo los lineamientos de seguridad.
- La interfaz es intuitiva, amigable y accesible.
- La funcionalidad es consistente en todos los navegadores y plataformas soportadas.
- El prototipo ha sido revisado, aprobado y probado con usuarios. Ha sido aceptado por el Product Owner y está listo para pruebas o desarrollo.

## Historias de usuario

### H1) 
Prioridad Alta - 2 story points
- Como: Usuario
- Quiero: Registrar una cuenta e iniciar sesión con nombre de usuario y contraseña o con google
- Para: Acceder a la aplicación, guardar mis reservas y promociones. 

#### Criterios de Aceptación:
- **Dado que** un usuario quiere registrarse
- **Cuando** el usuario complete los campos de email, nombre de usuario y contraseña
- **Entonces** el usuario debería poder registrarse con éxito o ver un mensaje de error si los datos son inválidos.

- **Dado que** un usuario quiere iniciar sesión
- **Cuando** el usuario ingrese su nombre de usuario y contraseña
- **Entonces** el usuario debería poder acceder a la aplicación

### H2)
Prioridad Media - 1 story point
- Como: Usuario
- Quiero: Poder recuperar mi contraseña
- Para: Poder acceder a mi cuenta si me olvido de la contraseña.

#### Criterios de Aceptación:
- **Dado que** un usuario ha olvidado su contraseña
- **Cuando** el usuario haga clic en "Recuperar contraseña"
- **Entonces** el sistema debería enviar un correo electrónico para restablecer la contraseña.

### H3)
Prioridad Alta - 1 story points
- Como: Usuario
- Quiero: Cerrar sesión 
- Para: Que otros usuarios no accedan a mi información

#### Criterios de Aceptación:
- **Dado que** un usuario ha iniciado sesión
- **Cuando** el usuario haga clic en "Cerrar sesión"
- **Entonces** el sistema debería cerrar la sesión y redirigir al usuario a la página de inicio.

### H4)
Prioridad Baja - 1 story points
- Como: Usuario
- Quiero: Poder modificar la información de mi cuenta
- Para: Poder actualizar mi información si esta cambia.

#### Criterios de Aceptación:
- **Dado que** un usuario ha iniciado sesión
- **Cuando** el usuario modifique la información de su cuenta (nombre, contraseña, etc.)
- **Entonces** los cambios deberían ser guardados correctamente.

### H5)
Prioridad Baja - 1 story points
- Como: Usuario
- Quiero: Seleccionar un avatar
- Para: Que la experiencia sea más personalizada?

#### Criterios de Aceptación:
- **Dado que** un usuario está creando o editando su perfil
- **Cuando** el usuario elija un avatar entre las opciones disponibles
- **Entonces** el avatar debería ser visible en su perfil.

### H6)
Prioridad Media - 3 story points
- Como: Usuario
- Quiero: Guardar mis restaurantes favoritos por zona
- Para: Seleccionar una zona y ver a dónde puedo ir

#### Criterios de Aceptación:
- **Dado que** un usuario está explorando restaurantes
- **Cuando** el usuario marque un restaurante como favorito
- **Entonces** el restaurante debería guardarse en su lista de favoritos.

### H7)
Prioridad Baja - 2 story points
- Como: Usuario
- Quiero: Configurar notificaciones de promociones en restaurantes favoritos
- Para: Enterarme de las promociones.

#### Criterios de Aceptación:
- **Dado que** un usuario ha guardado restaurantes favoritos
- **Cuando** el usuario configure las notificaciones de promociones
- **Entonces** el usuario debería recibir alertas cuando haya promociones en esos restaurantes.

### H8)
Prioridad Media - 2 story points
- Como: Usuario
- Quiero: Configurar notificaciones de reservas
- Para: Obtener la información de mis reservas

#### Criterios de Aceptación:
- **Dado que** un usuario tiene una reserva activa
- **Cuando** el usuario habilite las notificaciones de reservas
- **Entonces** el sistema debería notificar al usuario sobre el estado de sus reservas.

### H9)
Prioridad Media - 2 story points
- Como: Usuario 
- Quiero: Configurar notificaciones basadas en historial de reservas y valoraciones de otros usuarios
- Para: Encontrar nuevos restaurantes que sean similares a mis favoritos y que tengan buenas valoraciones.

#### Criterios de Aceptación:
- **Dado que** un usuario tiene historial de reservas
- **Cuando** el usuario habilite las recomendaciones basadas en el historial
- **Entonces** el sistema debería enviar sugerencias personalizadas de restaurantes.

### H10)
Prioridad Alta - 2 story points
- Como: Usuario
- Quiero: Tener un perfil con nombre de usuario, avatar, restaurantes favoritos, recomendaciones realizadas de restaurantes, historial de visitas a restaurantes.
- Para: Poder ver toda mi información en un solo lugar.

#### Criterios de Aceptación:
- **Dado que** un usuario ha iniciado sesión
- **Cuando** el usuario acceda a su perfil
- **Entonces** el perfil debería mostrar el nombre de usuario, avatar, restaurantes favoritos, recomendaciones y historial de visitas.

### H11)
Prioridad Alta - 2 story points
- Como: Usuario
- Quiero: Poder hacer una reserva en un restaurante o bar
- Para: Tener una mesa libre asegurada

#### Criterios de Aceptación:
- **Dado que** un usuario quiere reservar una mesa
- **Cuando** el usuario seleccione el restaurante, la fecha y la cantidad de personas
- **Entonces** el sistema debería confirmar la reserva y notificar al usuario.

### H12)
Prioridad Alta - 1 story point
- Como: Usuario
- Quiero: Poder cancelar una reserva previamente hecha
- Para: Ceder la mesa a otro cliente

#### Criterios de Aceptación:
- **Dado que** un usuario tiene una reserva activa
- **Cuando** el usuario cancele la reserva
- **Entonces** el sistema debería liberar la mesa y notificar al usuario.

### H13)
Prioridad Media - 1 story point
- Como: Usuario
- Quiero: Poder ver el estatus de mi reserva
- Para: Asegurarme de que haya sido confirmada

#### Criterios de Aceptación:
- **Dado que** un usuario tiene una reserva
- **Cuando** el usuario consulte el estado de su reserva
- **Entonces** el sistema debería mostrar si la reserva ha sido confirmada, pendiente o cancelada.

### H14)
Prioridad Baja - 1 story point
- Como: Usuario
- Quiero: Poder ver las calificaciones y comentarios de un restaurante
- Para: Poder ver si el restaurante es un buen lugar para visitar

#### Criterios de Aceptación:
- **Dado que** un usuario está explorando restaurantes
- **Cuando** el usuario seleccione un restaurante
- **Entonces** debería poder ver la puntuación y los comentarios de otros usuarios.

### H15)
Prioridad Alta - 1 story points
- Como: Usuario
- Quiero: Visualizar los restaurantes disponibles en mi zona
- Para: Ver las opciones de restaurantes cercanas a las que puedo ir

#### Criterios de Aceptación:
- **Dado que** un usuario está explorando restaurantes
- **Cuando** el usuario filtre por zona
- **Entonces** el sistema debería mostrar una lista de restaurantes cercanos.

### H16)
Prioridad Baja - 2 story points
- Como: Usuario
- Quiero: Poder recibir notificaciones de confirmación sobre mi reserva 
- Para: Tener una forma más cómoda de ver el estado de mi reserva

#### Criterios de Aceptación:
- **Dado que** un usuario ha realizado una reserva en un restaurante
- **Cuando** la reserva sea confirmada o cancelada por el restaurante
- **Entonces** el sistema debería enviar una notificación al usuario con el estado actualizado de la reserva.

### H17)
Prioridad Alta - 1 story points
- Como: Usuario
- Quiero: Poder seleccionar la cantidad de comensales
- Para: Que en la mesa que reserve haya lugar para todos.

#### Criterios de Aceptación:
- **Dado que** un usuario quiere hacer una reserva
- **Cuando** el usuario seleccione la cantidad de comensales
- **Entonces** el sistema debería permitir la reserva para esa cantidad de personas.

### H18)
Prioridad Media - 1 story point
- Como: Usuario
- Quiero: Poder filtrar por tipo de comida
- Para: Encontrar restaurantes que sirvan comida que me guste.

#### Criterios de Aceptación:
- **Dado que** un usuario está explorando un restaurante
- **Cuando** el restaurante ofrezca descuentos con tarjetas
- **Entonces**

### H19)
Prioridad Baja - 1 story points
- Como: Usuario
- Quiero: Que un restaurante me muestre si tiene descuentos con tarjetas
- Para: Saber qué beneficios puedo aprovechar.

#### Criterios de Aceptación:
- **Dado que** un usuario está explorando un restaurante
- **Cuando** el restaurante ofrezca descuentos con tarjetas
- **Entonces** el sistema debería mostrar los detalles de los descuentos disponibles.

### H20)
Prioridad Alta - 2 story points
- Como: Gerente.
- Quiero: Poder confirmar reserva para el restaurante que gerencio.
- Para: Gestionar las mesas disponibles en horarios y días definidos. Optimizando rendimiento y predicción.

#### Criterios de Aceptación:
- **Dado que** un gerente ha recibido una solicitud de reserva
- **Cuando** el gerente confirme la reserva
- **Entonces** el sistema debería notificar al cliente y actualizar la disponibilidad de mesas.

### H21)
Prioridad Alta - 2 story points
- Como: Gerente.
- Quiero: Poder modificar horarios disponibles y tipos de comida del restaurante que gerencio.
- Para: Informar correctamente a los clientes acerca de los servicios ofrecidos, lugares disponibles para ser reservados y nuestras horas de cierre/apertura.

#### Criterios de Aceptación:
- **Dado que** un gerente está gestionando un restaurante
- **Cuando** el gerente modifique los horarios o los tipos de comida
- **Entonces** el sistema debería reflejar los cambios y notificar a los clientes si es necesario.

### H22)
Prioridad Baja - 2 story points
- Como: Gerente.
- Quiero: Poder apelar a comentarios y puntuaciones que recibe mi restaurante.
- Para: Identificar mejoras posibles y obtener feedback directo de los clientes.

#### Criterios de Aceptación:
- **Dado que** un restaurante ha recibido un comentario o puntuación negativa
- **Cuando** el gerente quiera apelar el comentario
- **Entonces** el sistema debería permitirle enviar una solicitud de revisión.

### H23)
Prioridad Media - 2 story points
- Como: Gerente
- Quiero: Recibir notificaciones de reservas solicitadas para mi restaurante.
- Para: Poder confirmar/denegar las mismas a mis clientes cuanto antes.

#### Criterios de Aceptación:
- **Dado que** un cliente ha solicitado una reserva en un restaurante
- **Cuando** el cliente finalice el proceso de reserva
- **Entonces** el gerente debería recibir una notificación con los detalles de la reserva solicitada.

### H24)
Prioridad Alta - 2 story points
- Como: Administrador
- Quiero: Dar de alta un restaurante
- Para: Que pueda aparecer en la aplicación

#### Criterios de Aceptación:
- **Dado que** un administrador accede al panel de gestión
- **Cuando** el administrador introduce los detalles del restaurante (nombre, dirección, tipo de comida, horarios)
- **Entonces** el restaurante debería guardarse en la base de datos y estar disponible en la lista de restaurantes de la aplicación.

### H25)
Prioridad Alta - 2 story points
- -Como: Administrador
- Quiero: Poder dar de alta y modificar gerentes por restaurante 
- Para: Que gestione el restaurante asignado

#### Criterios de Aceptación:
- **Dado que** un administrador accede al panel de gestión
- **Cuando** el administrador introduce los datos de un gerente
- **Entonces** el gerente debería poder ser dado de alta o modificado correctamente y asignado a un restaurante específico.

### H26)
Prioridad Alta - 2 story points
- Como: Administrador
- Quiero: Indicar los restaurantes disponibles para reservar
- Para: Que los clientes sepan en cuales pueden realizar reservas

#### Criterios de Aceptación:
- **Dado que** un administrador accede al panel de gestión de restaurantes
- **Cuando** el administrador marque un restaurante como disponible para reservas
- **Entonces** los clientes deberían poder ver ese restaurante en la lista de restaurantes disponibles para reservar.

### H27)
Prioridad Baja - 2 story points
- Como: Administrador
- Quiero: Administrar comentarios y puntuaciones de restaurantes
- Para: Editar comentarios/modificar puntuaciones de un restaurante

#### Criterios de Aceptación:
- **Dado que** un administrador ha accedido a la sección de administración de comentarios y puntuaciones
- **Cuando** el administrador decida editar o eliminar un comentario o modificar una puntuación
- **Entonces** el sistema debería reflejar los cambios en la interfaz de los usuarios, actualizando las puntuaciones y comentarios.

### H28)
Prioridad Media - 2 story points
- Como: Gerente.
- Quiero: Poder agregar promociones en el restaurante que gerencio.
- Para: Recibir más clientes o premiar clientes recurrentes.

#### Criterios de Aceptación:
- **Dado que** un gerente ha creado una promocion
- **Cuando** el gerente confirme la promocion
- **Entonces** el sistema debería notificar a los clientes y actualizar las promociones del restaurante.


## Story map ##

![Story Map](./imagenes/storymap.png)
