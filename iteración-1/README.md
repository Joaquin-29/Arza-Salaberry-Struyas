# Indice

- [Gestión de la iteración](#gestión-de-la-iteración)
  - [Definición del marco de trabajo](#definición-del-marco-de-trabajo)
  - [Planificación de la iteración](#planificación-de-la-iteración)
  - [Seguimiento de la iteración](#seguimiento-de-la-iteración)
  - [Inspección y adaptación del proceso](#inspección-y-adaptación-del-proceso)
- [Identificar y definir el problema a resolver](#identificar-y-definir-el-problema-a-resolver)
  - [Identificación del problema a resolver](#identificación-del-problema-a-resolver)
  - [Definición del problema/solución](#definición-del-problema/solución)

# Gestión de la iteración

## Definición del marco de trabajo

_[Definición del marco de trabajo SCRUM con los acuerdos principales del equipo y evidencia de sus prácticas aplicadas en la iteración. Deben estar los roles definidos para cada integrante del equipo y la justificación de la adaptación del marco de trabajo al contexto de la iteración.]_

### Artefactos principales

- Definición del calendario de eventos con justificación de su adaptación al contexto de la iteración.
- Roles y responsabilidades definidos para cada integrante del equipo.
- Políticas de trabajo del equipo:
  - Definition of Done.
  - Definition of Ready.

## Planificación de la iteración

_[Sprint Backlog para cumplir con el objetivo de la iteración. Debe contener las historias de usuario priorizadas y las tareas planificadas basadas en la capacidad y velocidad disponible del equipo.]_

### Artefactos principales

- Minuta de la sprint planning con su agenda, actividades y resultados.
- Objetivos de la iteración.
- Sprint backlog con historias de usuarios y tareas asociadas.
- Planificación de acuerdo a la capacidad del equipo.
- Técnicas de priorización y estimación utilizadas.

## Seguimiento de la iteración

_[Existe evidencia sobre el registro de actividades y horas de cada integrante del equipo con el seguimiento general de cada iteración del proyecto sobre lo planificado inicialmente.]_

### Artefactos principales

- Minuta de daily scrum describiendo la coordinación del trabajo de cada integrante del equipo.
  - ¿Que logramos hacer?
  - ¿Qué planificamos hacer?
  - ¿Qué impedimentos tenemos?
- Registro y reporte de horas de cada integrante del equipo con sus actividades principales.
- Seguimiento visual de la iteración con burndown y/o burnup charts.

## Inspección y adaptación del proceso

_[Existe evidencia sobre la inspección del proceso con aprendizajes principales y acciones de mejora implementadas durante el desarrollo del proyecto.]_

### Artefactos principales

- Minuta de la retrospectiva con la dinámica utilizada y sus principales resultados.
- Planificación y seguimiento de las acciones de mejora.

# Identificar y definir el problema a resolver

## Identificación del problema a resolver

_[Entendimiento claro del problema del negocio a resolver con la identificación de los usuarios y escenarios principales con su valor de negocio asociado. Existe a su vez evidencia que se analiza y compara aplicaciones similares existentes del mercado.]_

## Artefactos principales

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

### Competidores

---

## Definición del problema/solución

_[Existe un Product Backlog definido con su jerarquía de épicas e historias de usuario con sus criterios de aceptación asociados. Existe una priorización de los prototipos principales que se buscarán idear, construir y validar como parte del ciclo de descubrimiento.]_

### Artefactos principales

- Product backlog con épicas e historias de usuario para prototipar.
- Historias de usuario cumpliendo el Definition of Ready con sus criterios de aceptación.
- Propuesta de valor diferenciadora de la competencia.
- Story map del roadmap inicial del proyecto.

# Product Backlog

## Login de usuario

El login de usuario deberá comprender:

- Login con nombre de usuario y contraseña.
- Login con usuario de Google.
- Recuperar contraseña.

### Criterios de aceptación

- El usuario debe poder iniciar sesión con su nombre de usuario y contraseña.
- El usuario debe poder iniciar sesión utilizando su cuenta de Google.
- El usuario debe poder recuperar su contraseña mediante un enlace enviado a su correo electrónico.

## Logout de usuario

Cerrar sesión.

### Criterios de aceptación

- El usuario debe poder cerrar sesión de su cuenta.
- Al cerrar sesión, el usuario debe ser redirigido a la página de inicio de sesión.
- La sesión del usuario debe ser invalidada en el servidor.

## Registrar restaurantes favoritos

En el registro, el cliente podrá registrar sus restaurantes favoritos en diferentes zonas.

### Criterios de aceptación

- El cliente debe poder añadir restaurantes a su lista de favoritos.
- El cliente debe poder organizar sus restaurantes favoritos por zonas.
- El cliente debe poder ver y gestionar su lista de restaurantes favoritos desde su perfil.

## Editar usuario

Poder modificar todo dato de usuario menos el email.

### Criterios de aceptación

- El cliente debe poder modificar su nombre, contraseña, dirección, y otros datos personales.
- El cliente no debe poder modificar su email.
- Los cambios deben ser guardados y reflejados en el perfil del cliente.

## Configurar notificaciones de promociones y confirmaciones de reserva

El usuario de perfil cliente podrá configurar si quiere ser notificado de promociones en los restaurantes que eligió como favoritos y de las confirmaciones de reserva.

### Criterios de aceptación

- El cliente debe poder activar o desactivar las notificaciones de promociones para los restaurantes favoritos.
- El cliente debe poder activar o desactivar las notificaciones de confirmaciones de reserva.
- Las configuraciones de notificaciones deben ser guardadas y reflejadas en el perfil del cliente.

## Solicitar reserva

El cliente podrá solicitar una reserva en alguno de los restaurantes o bares que estén dados de alta en la aplicación y que permitan reservas. Deberá seleccionar el restaurante, cantidad de personas y horario.

### Criterios de aceptación

- El cliente debe poder seleccionar un restaurante o bar que permita reservas.
- El cliente debe poder especificar la cantidad de personas para la reserva.
- El cliente debe poder seleccionar el horario de la reserva.
- La solicitud de reserva debe ser enviada y confirmada por el restaurante o bar.

## Usuario con perfil de cliente

El registro de cliente lo hace cada cliente utilizando su email, nombre de usuario, contraseña o haciendo el registro vía Google.

### Criterios de aceptación

- El cliente debe poder registrarse utilizando su email, nombre de usuario y contraseña.
- El cliente debe poder registrarse utilizando su cuenta de Google.
- Los datos de registro deben ser guardados y reflejados en el perfil del cliente.

## Cancelación de reserva

El cliente podrá cancelar una reserva.

### Criterios de aceptación

- El cliente debe poder ver una lista de sus reservas actuales.
- El cliente debe poder seleccionar una reserva y cancelarla.
- La cancelación de la reserva debe ser confirmada y reflejada en el perfil del cliente.

## Visualizar estatus de reserva

Visualización de estatus de una reserva.

### Criterios de aceptación

- El cliente debe poder ver el estatus de sus reservas actuales.
- El estatus de la reserva debe incluir información como confirmada, pendiente o cancelada.
- La información del estatus debe ser actualizada en tiempo real.

## Avatar de usuario

En el registro, el usuario puede seleccionar un avatar.

### Criterios de aceptación

- El usuario debe poder seleccionar un avatar durante el proceso de registro.
- El avatar seleccionado debe ser guardado y reflejado en el perfil del usuario.
- El usuario debe poder cambiar su avatar desde su perfil después del registro.

## Visualización de puntuación de restaurante y comentarios

El cliente podrá visualizar la puntuación de un restaurante y los comentarios.

### Criterios de aceptación

- El cliente debe poder ver la puntuación promedio de un restaurante.
- El cliente debe poder ver los comentarios dejados por otros clientes.
- La información de puntuación y comentarios debe ser actualizada en tiempo real.

## Configurar notificaciones de recomendaciones diarias

El cliente puede configurar si desea recibir notificaciones de recomendaciones del día basadas en el historial de reservas y valoraciones del usuario.

### Criterios de aceptación

- El cliente debe poder activar o desactivar las notificaciones de recomendaciones diarias.
- Las recomendaciones deben estar basadas en el historial de reservas y valoraciones del usuario.
- Las configuraciones de notificaciones deben ser guardadas y reflejadas en el perfil del usuario.

## Visualizar restaurantes disponibles

Visualizar restaurantes disponibles por zona (puede incluir mapa interactivo según su ubicación geográfica en tiempo real), rango de precios, y valoración (ranking).

### Criterios de aceptación

- El cliente debe poder ver una lista de restaurantes disponibles por zona.
- La visualización puede incluir un mapa interactivo basado en la ubicación geográfica en tiempo real del cliente.
- El cliente debe poder filtrar los restaurantes por rango de precios.
- El cliente debe poder ver la valoración (ranking) de los restaurantes.

## Usuario con perfil de gerenciador

Gerentes de restaurantes. Su registro lo realiza el administrador.

### Criterios de aceptación

- El administrador debe poder registrar a los gerentes de restaurantes.
- Los gerentes deben tener acceso a funcionalidades específicas para la gestión de sus restaurantes.
- Los datos de registro de los gerentes deben ser guardados y reflejados en el sistema.

## Perfil de cliente

El perfil del cliente deberá mostrar la siguiente información: Nombre de usuario, avatar, restaurantes favoritos, recomendaciones realizadas de restaurantes, historial de visitas a restaurantes.

### Criterios de aceptación

- El perfil del cliente debe mostrar el nombre de usuario.
- El perfil del cliente debe mostrar el avatar seleccionado.
- El perfil del cliente debe mostrar una lista de restaurantes favoritos.
- El perfil del cliente debe mostrar las recomendaciones realizadas de restaurantes.
- El perfil del cliente debe mostrar el historial de visitas a restaurantes.

## Recibir notificaciones

El cliente podrá recibir notificaciones de reserva confirmada.

### Criterios de aceptación

- El cliente debe recibir una notificación cuando una reserva sea confirmada.
- La notificación debe incluir detalles de la reserva confirmada.
- Las notificaciones deben ser enviadas en tiempo real.

## Administrador

Administrador capaz de registrar gerentes de restaurantes.

### Criterios de aceptación

- El administrador debe poder registrar a los gerentes de restaurantes.
- Los datos de registro de los gerentes deben ser guardados y reflejados en el sistema.
- El administrador debe tener acceso a funcionalidades específicas para la gestión de gerentes y restaurantes.

## Alta restaurantes

El administrador podrá dar de alta los restaurantes indicando dirección, tipo de comida y horarios.

### Criterios de aceptación

- El administrador debe poder registrar nuevos restaurantes.
- El administrador debe poder especificar la dirección del restaurante.
- El administrador debe poder especificar el tipo de comida del restaurante.
- El administrador debe poder especificar los horarios del restaurante.
- Los datos del restaurante deben ser guardados y reflejados en el sistema.

## Gerente confirma reservas

El gerente debe ser capaz de confirmar reservas para el restaurante que gerencia.

### Criterios de aceptación

- El gerente debe poder ver una lista de reservas pendientes para su restaurante.
- El gerente debe poder confirmar una reserva.
- La confirmación de la reserva debe ser reflejada en el sistema y notificar al cliente.

## Alta y modificación de gerenciadores

Dar de alta y modificar gerenciadores por restaurante.

### Criterios de aceptación

- El administrador debe poder registrar nuevos gerenciadores para los restaurantes.
- El administrador debe poder modificar los datos de los gerenciadores existentes.
- Los cambios deben ser guardados y reflejados en el sistema.

## Gerente modifica restaurante

El gerente debe ser capaz de modificar los horarios disponibles y los tipos de comida del restaurante que gerencia.

### Criterios de aceptación

- El gerente debe poder modificar los horarios disponibles del restaurante.
- El gerente debe poder modificar los tipos de comida del restaurante.
- Los cambios deben ser guardados y reflejados en el sistema.

## Restaurantes disponibles para reserva

El administrador podrá indicar restaurantes para los cuales se podrán realizar reservas.

### Criterios de aceptación

- El administrador debe poder seleccionar los restaurantes que permitirán reservas.
- Los cambios deben ser guardados y reflejados en el sistema.
- Los restaurantes seleccionados deben estar disponibles para que los clientes realicen reservas.

## Gerente apela a review

El gerente debe ser capaz de apelar a puntuaciones o comentarios que recibe el restaurante que gerencia.

### Criterios de aceptación

- El gerente debe poder ver las puntuaciones y comentarios recibidos por su restaurante.
- El gerente debe poder apelar a una puntuación o comentario específico.
- La apelación debe ser enviada al administrador para su revisión.
- Los cambios deben ser guardados y reflejados en el sistema.

## Administrar comentarios y puntuaciones de restaurantes

El administrador podrá administrar comentarios y puntuaciones de restaurantes.

### Criterios de aceptación

- El administrador debe poder ver todos los comentarios y puntuaciones de los restaurantes.
- El administrador debe poder editar o eliminar comentarios y puntuaciones inapropiados.
- Los cambios realizados por el administrador deben ser guardados y reflejados en el sistema.

## Gerente recibe notificaciones

El gerente debe recibir notificaciones de reservas solicitadas del restaurante que gerencia.

### Criterios de aceptación

- El gerente debe recibir una notificación cuando se solicite una reserva en su restaurante.
- La notificación debe incluir detalles de la reserva solicitada.
- Las notificaciones deben ser enviadas en tiempo real.

## Promociones

El gerente podrá crear promociones para sus restaurantes que serán visibles por los clientes.

### Criterios de aceptación

- El gerente debe poder crear nuevas promociones para sus restaurantes.
- Las promociones deben ser visibles para los clientes.
- Los detalles de las promociones deben ser guardados y reflejados en el sistema.


