# Gimnasio

## Miembros del grupo L3-ABS-2

1. Gallego Cal, Guillermo
1. Sanchez Gonzalez, Alejandro
1. Khattabi El Inani, Ilias
1. Ruiz Ojeda, Jose Manuel

## 1. Introducción al problema

### 1.1. Contexto y situación actual

Hoy en día, el mundo del gimnasio y el deporte de fuerza ha crecido muchísimo, ya que cada vez más gente busca entrenar en serio y cuidar su físico. Sin embargo, al analizar el sector nos encontramos con que hay muchísima competencia, pero casi toda cae en uno de estos dos extremos:

* **Los gimnasios comerciales o *low-cost*:** Compiten tirando los precios, pero a cambio están siempre masificados en hora punta, les falta maquinaria específica para entrenar pesado de verdad y apenas hay seguimiento por parte de los monitores.
* **Los centros pequeños o especializados (boxes o gimnasios de barrio):** Aunque a veces tienen buen material para una disciplina concreta, se quedan cortos si buscas variedad y, sobre todo, suelen llevar toda la gestión a la antigua (con fichas de papel, hojas de Excel sueltas o grupos de WhatsApp), lo que acaba siendo un caos tanto para el dueño como para el que va a entrenar.

Viendo este problema, nuestro proyecto consiste en abrir **Legion Gym**, con el objetivo de montar el centro deportivo más completo de la zona y desmarcarnos de la competencia. La idea es juntar en una misma instalación, bien dividida por salas y zonas específicas, las cuatro grandes ramas del entrenamiento actual:

1. **Zona de Culturismo y Musculación:** Equipada con máquinas seleccionadas por su biomecánica y peso libre para trabajar de forma completa todos los grupos musculares (pecho, espalda, pierna y brazo).
2. **Zona de *Powerlifting*:** Preparada para el entrenamiento de fuerza con jaulas de potencia (*racks*), plataformas de peso muerto, bancos reglamentarios y discos calibrados.
3. **Zona de Calistenia y *Street Workout*:** Una estructura completa con barras de dominadas, paralelas y anillas pensada tanto para básicos y repeticiones como para ejercicios de tensión y lastre.
4. **Box de *CrossFit* y Entrenamiento Funcional:** Salas amplias orientadas a entrenamientos de alta intensidad y clases colectivas dirigidas por entrenadores.

<img width="1200" height="675" alt="foto gym" src="https://github.com/user-attachments/assets/d1e63ce4-f145-4db0-8282-0c4c64b955a2" />

Para que un gimnasio tan grande y con tantas disciplinas funcione sin volverse un descontrol, no basta con tener las mejores instalaciones físicas; necesitamos acompañarlo desde el primer día de un Sistema de Información propio que automatice toda la gestión.

### 1.2. Problemas que queremos resolver

Cuando un centro deportivo ofrece tantas opciones (clases dirigidas, distintas salas, entrenadores especializados y varios tipos de cuotas), intentar llevar el control de forma manual o con programas básicos que no están conectados entre sí genera problemas diarios muy claros:

* **Salas llenas y falta de espacio (*Overbooking*):** En disciplinas como *CrossFit*, calistenia o entrenamientos guiados de fuerza, el espacio y el material (barras, jaulas, máquinas) son limitados. Si no se controla automáticamente cuánta gente reserva en función de la capacidad máxima de cada sala, se juntan demasiadas personas a la vez, se entrena mal y se pierde calidad frente a la competencia.
* **Descontrol con las matrículas y los pagos:** Al manejar distintos planes de membresía de forma manual, es muy fácil que se pasen por alto matrículas que ya han caducado, que no quede claro quién tiene pagos pendientes o que por error administrativo se le duplique la matrícula activa a un mismo socio.
* **Descoordinación en horarios y entrenadores:** Cuadrar a mano qué entrenador da cada clase según su especialidad, en qué sala y a qué hora suele provocar solapamientos. Además, los entrenadores llegan a dar su clase a ciegas, sin saber cuánta gente se ha apuntado hasta que entran por la puerta.
* **Pérdida de tiempo para el socio en recepción:** Tener que ir al mostrador o preguntar en recepción solo para saber cuándo te caduca el mes, ver los horarios de las clases o reservar plaza hace que se formen colas innecesarias y da una imagen anticuada del gimnasio.

<img width="617" height="348" alt="overbooking gym" src="https://github.com/user-attachments/assets/b076c899-2454-449a-9ed2-6d6ab458753e" />

### 1.3. Clientes y usuarios en el contexto del proyecto

Dentro del contexto de nuestro proyecto, diferenciamos entre quién encarga el sistema y quiénes lo van a usar en el día a día del gimnasio (cuyas funciones detalladas dentro de la aplicación se especificarán más adelante en el documento):

* **El Cliente:** Es la **Dirección o Gerencia de Legion Gym**. Son los propietarios que invierten en el proyecto y ponen las reglas del negocio. Lo que buscan con este software es llevar las cuentas claras, evitar que entre gente con la cuota vencida, aprovechar al máximo las salas y conseguir que el gimnasio destaque por encima de cualquier competidor.
* **Los Usuarios:** Son las personas que van a interactuar con el sistema en el gimnasio:
  * **El personal de administración:** Los encargados de llevar el control general del centro (altas de socios, configuración de planes, matrículas, cobros y organización de salas, clases y horarios).
  * **Los entrenadores:** Los profesionales de cada área deportiva, que necesitan tener clara su agenda de clases, en qué sala les toca y qué volumen de reservas tienen para organizar la sesión.
  * **Los socios:** Los deportistas inscritos en el gimnasio, que buscan poder gestionar sus reservas a las clases y consultar el estado de su matrícula y sus pagos de forma rápida y sin complicaciones.

<img width="137" height="296" alt="plan gym" src="https://github.com/user-attachments/assets/f8160ddd-f9e7-4c55-863d-e4f11b510ff3" />

### 1.4. Expectativas y objetivos

Con la puesta en marcha de este sistema de gestión, nuestras expectativas son:

1. **Centralizar toda la información del gimnasio:** Dejar atrás el papel y las hojas de cálculo sueltas para tener todos los datos de socios, matrículas, planes, pagos, entrenadores, salas, horarios y reservas guardados de forma segura y ordenada en un único sitio.
2. **Asegurar que se cumplan las normas del centro automáticamente:** Que sea el propio programa el que impida errores habituales, como que alguien reserve con la matrícula caducada, que se supere el aforo máximo de una sala o que se intente reservar una clase que ya ha empezado.
3. **Mejorar la experiencia diaria en el gimnasio:** Conseguir que tanto la administración como los entrenadores y los socios ahorren tiempo en gestiones, logrando que **Legion Gym** sea referente no solo por sus zonas de culturismo, *powerlifting*, calistenia y *CrossFit*, sino también por lo cómodo y bien organizado que está.

## 2. Glosario de términos

### A

Actividad deportiva: Ejercicio o práctica física que se realiza para mejorar la condición física, desarrollar habilidades o mantener un estilo de vida saludable. En el gimnasio, puede realizarse de forma individual o mediante clases dirigidas.

### C

Clase dirigida: Actividad deportiva organizada e impartida por un entrenador, con una duración, un horario y una capacidad máxima determinados.

Capacidad máxima: Número máximo de personas que pueden utilizar una sala o participar en una clase de forma simultánea, según los límites establecidos.

### E

Entrenador: Profesional encargado de dirigir actividades deportivas, orientar a los socios durante el ejercicio y supervisar el desarrollo de las clases que tiene asignadas.

<img src="images.jpg" alt="Entrenador" width="200">

Estado: Situación actual de un elemento del sistema, como una matrícula, una reserva, un pago o una máquina. Permite identificar su condición en un momento determinado.

### G

Gimnasio: Instalación destinada a la práctica de ejercicio físico y actividades deportivas que dispone de espacios, equipamiento y profesionales para atender a sus usuarios.

### H

Horario: Intervalo de tiempo establecido para determinar cuándo comienza y termina una clase o actividad deportiva.

<img src="horario.avif" alt="Horario" width="200">

### M

Mantenimiento de la matrícula: Control de la vigencia de la inscripción de un socio en el gimnasio, teniendo en cuenta sus fechas de inicio y finalización y su estado.

Matrícula: Registro que vincula a un socio con un plan de membresía durante un periodo determinado y establece las condiciones de su inscripción en el gimnasio.

Máquina de musculación: Equipamiento deportivo diseñado para realizar ejercicios de fuerza y trabajar uno o varios grupos musculares.

<img src="maquinas.webp" alt="Máquinas de musculación" width="200">

Músculo: Tejido del cuerpo humano que permite producir movimiento mediante su contracción. En el ámbito del entrenamiento, los músculos se agrupan según las zonas del cuerpo que se trabajan durante los ejercicios: pierna, brazo, pecho y espalda.

<img src="download.jpg" alt="Músculos" width="200">

### P

Pago: Operación económica mediante la cual un socio abona una cantidad correspondiente a los servicios o a la membresía del gimnasio.

Plan de membresía: Modalidad de inscripción que establece las condiciones económicas y temporales de acceso a los servicios del gimnasio, como su precio y duración.

### R

Reserva: Registro mediante el cual un socio solicita una plaza para participar en una clase dirigida. Su gestión permite controlar las plazas disponibles y la asistencia prevista.

### S

Sala: Espacio físico del gimnasio destinado a la realización de actividades deportivas o a la ubicación de equipamiento de entrenamiento.

Socio: Persona inscrita en el gimnasio que dispone de una matrícula asociada a un plan de membresía.

## 3. Visión general del sistema

Legion Gym contará con un Sistema de Información diseñado para centralizar y automatizar las principales tareas administrativas y deportivas del gimnasio. El sistema permitirá gestionar los socios, las matrículas, los planes de membresía, los pagos, los entrenadores, las salas, las clases dirigidas y las reservas.

La aplicación estará orientada a tres tipos de usuarios: el personal de administración, los entrenadores y los socios. Cada perfil dispondrá de unas funcionalidades específicas según sus responsabilidades y necesidades dentro del centro.

El objetivo principal del sistema será mejorar la organización interna de Legion Gym, reducir los errores administrativos y facilitar el acceso a la información. Para ello, se establecerán controles automáticos que permitan comprobar la vigencia de las matrículas, gestionar las plazas disponibles en las clases y evitar conflictos en la asignación de entrenadores, salas y horarios.

Además, el sistema deberá mantener la información centralizada y actualizada para que los distintos usuarios puedan consultar los datos que necesiten según sus permisos.

### 3.1. Requisitos generales

Los requisitos generales definen las funcionalidades y condiciones básicas que deberá cumplir el Sistema de Información de Legion Gym para satisfacer las necesidades del gimnasio.

#### 3.1.1. Gestión de socios

El sistema deberá permitir al personal de administración registrar nuevos socios, consultar sus datos, modificarlos y gestionar su baja cuando corresponda. Para cada socio se almacenará la información necesaria para su identificación y contacto, así como los datos relacionados con su matrícula y su historial de pagos.

Cada socio deberá disponer de un identificador único que permita distinguirlo del resto de usuarios y relacionar correctamente toda su información dentro del sistema.

En relación a los socios, además, la aplicación permitirá crear y gestionar diferentes planes de membresía, estableciendo sus precios, duración y condiciones de acceso a las instalaciones y actividades del gimnasio.

El sistema deberá registrar las matrículas de los socios, incluyendo sus fechas de inicio y finalización y su estado actual. También deberá controlar su vigencia para impedir que los socios con una matrícula caducada o inactiva puedan realizar reservas que requieran una inscripción válida.

Asimismo, se deberán evitar registros duplicados de matrículas activas cuando no estén permitidos por las normas del gimnasio.

#### 3.1.2. Gestión de pagos

El sistema deberá permitir registrar y consultar los pagos asociados a las matrículas de los socios. Para cada operación se almacenarán datos como el importe, la fecha, el concepto y el estado del pago.

El personal de administración podrá comprobar qué socios tienen pagos pendientes y consultar el historial de operaciones económicas. El sistema deberá mantener diferenciados los pagos realizados, pendientes y rechazados, cuando corresponda.

#### 3.1.3. Gestión de entrenadores

La aplicación permitirá registrar y actualizar la información de los entrenadores, incluyendo sus datos identificativos, sus especialidades deportivas y las clases que tienen asignadas.

Cada entrenador podrá consultar su agenda para conocer las actividades que debe impartir, los horarios correspondientes, las salas asignadas y el número de reservas registradas en cada clase.

El sistema deberá impedir que un mismo entrenador tenga asignadas dos clases incompatibles en el mismo intervalo horario.

#### 3.1.4. Gestión de salas y actividades deportivas

El sistema permitirá registrar las salas disponibles en Legion Gym y definir sus características principales, como su nombre, su tipo de actividad y su capacidad máxima.

Se podrán organizar actividades relacionadas con las diferentes disciplinas del gimnasio, como musculación, powerlifting, calistenia, CrossFit y entrenamiento funcional.

La aplicación deberá controlar la disponibilidad de las salas y evitar que se programen actividades simultáneas incompatibles en un mismo espacio. También deberá impedir que una clase supere la capacidad máxima establecida.

En relación con la gestión de salas, el sistema deberá permitir crear, modificar y consultar las clases dirigidas, indicando su actividad, entrenador responsable, sala, fecha, hora de inicio, hora de finalización y número máximo de participantes.

Antes de confirmar una nueva clase o modificar una existente, se deberán comprobar los posibles conflictos de horario y la disponibilidad de los recursos necesarios.

Los socios podrán consultar la programación de las clases para conocer qué actividades se ofrecen y cuándo se realizan.

#### 3.1.5. Gestión de reservas

La aplicación permitirá a los socios reservar plazas en las clases dirigidas que tengan disponibles.

Antes de confirmar una reserva, el sistema deberá comprobar que el socio dispone de una matrícula válida, que la clase admite nuevas reservas, que todavía quedan plazas libres y que la actividad no ha comenzado.

También se deberá impedir que un mismo socio tenga varias reservas para una misma sesión cuando estas sean incompatibles con las normas del gimnasio.

El personal autorizado podrá consultar el listado de participantes de cada clase y gestionar las reservas cuando sea necesario.

#### 3.1.6. Control de acceso según el tipo de usuario

El sistema deberá distinguir entre el personal de administración, los entrenadores y los socios mediante un mecanismo de identificación y control de permisos.

- **Administración:** podrá gestionar los socios, las matrículas, los planes de membresía, los pagos, los entrenadores, las salas, las actividades, los horarios y las reservas.
- **Entrenadores:** podrán consultar sus horarios, las clases asignadas y los participantes inscritos en sus sesiones.
- **Socios:** podrán consultar su información personal, el estado de su matrícula, sus pagos y la programación de clases, además de realizar y cancelar reservas conforme a las normas establecidas.

Cada usuario únicamente podrá acceder a las funciones y los datos autorizados para su perfil.

#### 3.1.7. Consulta de información y disponibilidad

El sistema deberá facilitar la consulta de información actualizada sobre las clases, sus horarios, las salas disponibles y las plazas libres.

También deberá permitir consultar los datos relacionados con los socios, las matrículas, los pagos y las actividades, según los permisos de cada usuario.

La información deberá presentarse de forma clara y organizada para facilitar las tareas administrativas y mejorar la experiencia de los socios y entrenadores.

#### 3.1.8. Seguridad e integridad de los datos

La aplicación deberá proteger la información almacenada mediante controles de acceso y validaciones que eviten operaciones incorrectas.

Los datos de los socios, las matrículas, los pagos, los entrenadores y las reservas deberán mantenerse relacionados de forma coherente. Además, el sistema deberá evitar la pérdida de información y contemplar mecanismos de copia de seguridad y recuperación de los datos.

Por último, las operaciones que modifiquen información importante deberán realizarse de forma controlada para mantener la integridad de la información del gimnasio.

### 3.2. Usuarios del sistema

Los usuarios del sistema son aquellas personas las cuales van a utilizar la aplicación y realizar operaciones con ella. En nuestro sistema de gestión del  Gimnasio, tenemos tres usuarios posibles, que son el administrador del gimnasio, el socio y el entrenador. Cada uno tendrá diferentes responsabilidades y funcionalidades según su papel dentro del gimnasio.

El administrador del gimnasio es quien gestiona la información general del gimnasio. Tendrá acceso a las funciones de gestión de socios, planes de membresía, matrículas, entrenadores, clases, salas, horarios y pagos. Su función principal será garantizar el correcto funcionamiento y la organización de las actividades del gimnasio.

El socio será el usuario que esté inscrito en el gimnasio y utilice el sistema para consultar y gestionar su actividad. Podrá consultar el estado y la fecha de finalización de su matrícula, visualizar las clases disponibles y sus horarios, realizar o cancelar reservas y consultar la información de sus pagos.

El entrenador será el profesional encargado de impartir las clases y actividades del gimnasio. A través del sistema podrá consultar las clases que tiene asignadas, revisar sus horarios y las salas en las que se desarrollan, así como consultar las reservas de sus clases para conocer la asistencia prevista.

## 4. Catálogo de requisitos

### 4.1. Requisitos funcionales

#### R.F.01. Consulta de socios
-   Como administrador del gimnasio quiero consultar los datos de los socios para mantener actualizada su información personal.

##### Prueba de aceptación

- Comprobar que el administrador puede registrar un socio introduciendo sus datos personales y que el sistema almacena correctamente la información.
  
- Comprobar que el administrador puede consultar los datos de un socio registrado y modificar su información, verificando que los cambios quedan guardados.
  
- Comprobar que el sistema impide registrar un socio cuando faltan datos obligatorios o cuando los datos introducidos no cumplen los formatos establecidos.
  
- Se debe aplicar la regla de negocio R.N.06.

#### R.F.02. Consulta de planes
-   Como administrador del gimnasio quiero consultar los planes de membresía para gestionar las diferentes opciones disponibles para los socios.

##### Prueba de aceptación

- Comprobar que el administrador puede crear un plan de membresía indicando sus características, duración y precio.
  
- Comprobar que el administrador puede consultar los planes registrados y modificar sus datos, verificando que los cambios se guardan correctamente.
  
- Comprobar que el sistema impide crear un plan con datos obligatorios incompletos, una duración no válida o un precio negativo.
  
- Se debe aplicar la regla de negocio R.N.06 y la regla de negocio R.N.11.

#### R.F.03. Consulta de matrículas
-   Como administrador del gimnasio quiero consultar las matrículas de los socios, indicando el plan, la fecha de inicio y la fecha de fin para
  controlar la vigencia de sus membresías.

##### Prueba de aceptación

- Comprobar que el administrador puede registrar una matrícula para un socio, asociándola a un plan e indicando las fechas de inicio y finalización.
  
- Comprobar que el sistema permite consultar las matrículas registradas y muestra correctamente el plan asociado y su periodo de vigencia.
  
- Comprobar que el sistema impide registrar una matrícula con una fecha de finalización anterior a la fecha de inicio.
  
- Comprobar que el sistema impide que un socio tenga más de una matrícula activa simultáneamente.
  
- Se debe aplicar la regla de negocio R.N.02 y la regla de negocio R.N.06.

#### R.F.04. Consulta del estado de la matrícula
-   Como socio quiero consultar el estado y la fecha de finalización de mi matrícula para saber si mi membresía está activa y cuándo caduca.

##### Prueba de aceptación

- Comprobar que un socio puede consultar su matrícula y visualizar su estado y su fecha de finalización.
  
- Comprobar que el sistema muestra la matrícula como activa cuando la fecha actual se encuentra dentro de su periodo de vigencia y como caducada cuando ha finalizado dicho periodo.
  
- Comprobar que un socio únicamente puede consultar la información de sus propias matrículas y no la de otros socios.
  
- Se debe aplicar la regla de negocio R.N.13.

#### R.F.05. Consulta de entrenadores
-   Como administrador del gimnasio quiero registrar y gestionar los datos de los entrenadores y su especialidad para mantener actualizada la información del personal encargado de las clases.
  
##### Prueba de aceptación

- Comprobar que el administrador puede registrar un entrenador indicando sus datos personales y su especialidad.
  
- Comprobar que el administrador puede consultar la información de un entrenador registrado y modificar sus datos, verificando que los cambios se guardan correctamente.
  
- Comprobar que el sistema impide registrar un entrenador cuando faltan datos obligatorios o la información introducida no cumple los formatos establecidos.
  
- Se debe aplicar la regla de negocio R.N.06.

#### R.F.06. Consulta de clases
-   Como administrador del gimnasio quiero consultar y gestionar las clases, indicando su nombre, descripción, duración, capacidad máxima, y entrenador para organizar la oferta de actividades del gimnasio.

##### Prueba de aceptación

- Comprobar que el administrador puede crear una clase indicando su nombre, descripción, duración, capacidad máxima, entrenador, sala y horario.
  
- Comprobar que el administrador puede consultar las clases registradas y modificar sus datos, verificando que los cambios se guardan correctamente.
  
- Comprobar que el sistema no permite crear una clase sin entrenador, sala u horario asignado.
  
- Comprobar que la capacidad máxima de una clase no supera la capacidad de la sala en la que se realiza.
  
- Comprobar que el sistema impide asignar a un entrenador una clase cuyo horario se solape con otra clase que tenga asignada.
  
- Se debe aplicar la regla de negocio R.N.03, la regla de negocio R.N.04 y las reglas de negocio R.N.14 y R.N.15.

#### R.F.07. Consulta de salas
- Como administrador del gimnasio quiero consultar y gestionar las salas, indicando su capacidad y ubicación para organizar los espacios donde se realizan las clases.

##### Prueba de aceptación

- Comprobar que el administrador puede registrar una sala indicando su capacidad y ubicación.
  
- Comprobar que el administrador puede consultar las salas registradas y modificar sus datos, verificando que los cambios se guardan correctamente.
  
- Comprobar que el sistema impide registrar una sala con una capacidad igual o inferior a cero o sin los datos obligatorios.
  
- Comprobar que el sistema impide asignar una misma sala a dos clases cuyos horarios se solapen.
  
- Se debe aplicar la regla de negocio R.N.06 y la regla de negocio R.N.15.

#### R.F.08. Consulta de horarios
- Como administrador del gimnasio quiero establecer y consultar los horarios de las clases para organizar la programación de actividades del gimnasio.

##### Prueba de aceptación

- Comprobar que el administrador puede establecer un horario para una clase indicando su fecha y hora de inicio y finalización.
  
- Comprobar que el administrador puede consultar los horarios de las clases y visualizar correctamente la fecha, la hora, la sala y el entrenador asignados.
  
- Comprobar que el sistema impide establecer un horario cuya hora de finalización sea anterior o igual a la hora de inicio.
  
- Comprobar que el sistema impide programar dos clases en la misma sala durante periodos que se solapen.
  
- Comprobar que el sistema impide asignar al mismo entrenador dos clases cuyos horarios se solapen.
  
- Se debe aplicar la regla de negocio R.N.03 y la regla de negocio R.N.15.

#### R.F.09. Consultar de reservas
- Como socio quiero  consultar mis reservas y cancelar mi asistencia a las clases para poder organizar mi participación en las actividades del gimnasio.

##### Prueba de aceptación

- Comprobar que un socio con una matrícula activa puede reservar una clase cuyo horario todavía no haya comenzado y que disponga de plazas libres.
 
- Comprobar que un socio puede cancelar una reserva realizada previamente y que la plaza queda disponible para otro socio.
  
- Comprobar que el sistema impide realizar una reserva cuando el socio no tiene una matrícula activa o su matrícula ha caducado.
  
- Comprobar que el sistema impide realizar una reserva cuando la clase ha comenzado o cuando se ha alcanzado la capacidad máxima permitida.
  
- Comprobar que el sistema impide que un socio realice varias reservas para una misma clase.
  
- Se debe aplicar la regla de negocio R.N.01, la regla de negocio R.N.04, la regla de negocio R.N.05 y la regla de negocio R.N.16.

#### R.F.10. Consulta de pagos
- Como administrador del gimnasio quiero registrar y consultar los pagos realizados por los socios, indicando el importe, la fecha, el método de pago y el estado para llevar un control de los pagos y de las matrículas.

##### Prueba de aceptación

- Comprobar que el administrador puede registrar un pago asociado a un socio, indicando el importe, la fecha, el método de pago y el estado.

- Comprobar que el administrador puede consultar los pagos registrados y visualizar correctamente la información de cada operación.
 
- Comprobar que el sistema impide registrar pagos con importes iguales o inferiores a cero o con datos obligatorios incompletos.
  
- Comprobar que el sistema permite identificar los pagos asociados a un socio y a la matrícula correspondiente.
 
- Comprobar que el sistema conserva el estado registrado de cada pago y permite consultar si se encuentra pendiente, realizado o rechazado, según los estados definidos por el sistema.
 
- Se debe aplicar la regla de negocio R.N.06 y la regla de negocio R.N.11.

#### 4.1.1. Requisitos de información

##### R.I.01.Consulta de la agenda y listado de participantes para entrenadores

Como entrenador quiero consultar mi agenda de clases y el listado de socios inscritos en cada sesión para conocer las actividades que debo impartir y la asistencia prevista.

**Prueba de aceptación**
- Comprobar que un entrenador puede visualizar su calendario de clases asignadas con sus respectivos horarios, salas y tipos de actividad.

- Comprobar que el entrenador puede acceder al listado actualizado de socios que han reservado plaza en una de sus clases.

- Comprobar que un entrenador únicamente puede visualizar la información correspondiente a sus propias clases y no las de otros compañeros.

- Se debe aplicar la regla de negocio R.N.03 y la regla de negocio R.N.13.

##### R.I.02. Consulta del historial de pagos y recibos para socios

Como socio quiero consultar mi historial de pagos realizados y pendientes para llevar un control de mis cuotas y comprobar el estado de mis transacciones.

**Prueba de aceptación**
- Comprobar que un socio puede acceder a una pantalla de resumen donde se listan todas sus operaciones económicas (pagos realizados, pendientes o rechazados).

- Comprobar que para cada pago se muestra correctamente la fecha, el importe, el concepto y el estado del mismo.

- Comprobar que un socio únicamente puede consultar sus propios datos de pago y nunca los de otros usuarios del gimnasio.

- Se debe aplicar la regla de negocio R.N.11 y la regla de negocio R.N.13.

#### R.I.03. Consulta general de la ocupación de salas y aforos para la administración

Como administrador del gimnasio quiero consultar el estado de ocupación actual y programada de las distintas salas para optimizar el espacio y evitar problemas de capacidad.

**Prueba de aceptación**

- Comprobar que el administrador puede ver un panel con el listado de salas, su capacidad máxima y las actividades o clases que se están realizando en tiempo real o en un horario determinado.

- Comprobar que el sistema muestra alertas visuales o indicadores cuando una sala se encuentra próxima a su límite de capacidad o experimenta solapamientos.

- Comprobar que la información se actualiza de manera coherente cada vez que se añade una nueva clase o se realiza una reserva.

- Se debe aplicar la regla de negocio R.N.04 y la regla de negocio R.N.15.

#### R.I.04. Consulta de la programación de clases dirigidas para los socios

Como socio quiero consultar la programación completa de clases dirigidas disponibles en el gimnasio filtrando por disciplina, horario o entrenador para planificar mis entrenamientos semanales.

**Prueba de aceptación**

- Comprobar que un socio puede visualizar la parrilla de clases semanales organizadas por zonas o disciplinas (CrossFit, calistenia, etc.).

- Comprobar que el sistema muestra el número de plazas libres restantes en cada clase antes de que el socio intente realizar su reserva.

- Comprobar que las clases que ya han comenzado o que no disponen de plazas libres se muestran claramente indicadas con su estado correspondiente.

- Se debe aplicar la regla de negocio R.N.01 y la regla de negocio R.N.05.

#### 4.1.2. Reglas de negocio

##### R.N.01. Matrícula activa para realizar reservas
-   Un socio debe tener una matrícula activa para poder realizar una reserva en una clase.

##### R.N.02. Una única matrícula activa
-   Un socio no puede tener más de una matrícula activa al mismo tiempo.

##### R.N.03. Asignación de clases
-   Cada clase debe estar asociada a un entrenador, una sala y un horario determinado.

##### R.N.04. Capacidad máxima de las clases
-   El número de reservas de una clase no puede superar la capacidad máxima de la sala donde se realiza.
  
##### R.N.05. Restricciones para realizar reservas
-   Un socio no puede reservar una clase cuyo horario ya haya comenzado ni realizar una reserva cuando su matrícula se encuentre caducada.

##### R.N.06. Restricciones para gestionar matrículas
-  La fecha de finalización de una matrícula debe ser posterior a su fecha de inicio. El estado de la matrícula debe determinarse a partir de su periodo de vigencia y de las condiciones de activación establecidas por el sistema.
  
##### R.N.07. Restricciones para definir planes de membresía
-  El precio de un plan de membresía no puede ser negativo y su duración debe ser un valor válido y superior a cero.

##### R.N.08. Restricciones para asignar capacidades a salas y clases
-  La capacidad de una sala debe ser un número entero positivo. Ninguna clase podrá tener una capacidad máxima superior a la capacidad de la sala asignada.

##### R.N.09. Restricciones para registrar pagos
-  El importe de un pago debe ser superior a cero. El sistema debe validar el importe y los datos obligatorios antes de registrar la operación.

##### R.N.10. Restricciones para consultar y gestionar información personal
-  Cada socio únicamente podrá consultar su propia información personal, sus matrículas y los datos relacionados con sus reservas y pagos. El administrador podrá consultar y gestionar la información de los socios de acuerdo con sus permisos.

##### R.N.11. Restricciones para asignar horarios a entrenadores
-  Un entrenador no puede tener asignadas dos clases cuyos horarios se solapen. El sistema debe comprobar la disponibilidad del entrenador antes de guardar o modificar la programación de una clase.

##### R.N.12. Restricciones para asignar horarios a salas
-  Una sala no puede estar asignada a dos clases cuyos horarios se solapen. El sistema debe comprobar la disponibilidad de la sala antes de guardar o modificar la programación de una clase.

##### R.N.13. Restricciones para registrar reservas de una misma clase
-  Un socio no puede mantener más de una reserva activa para una misma clase programada. Si ya dispone de una reserva activa, el sistema debe impedir que registre otra para esa misma sesión.
  
### 4.2. Mapa de historias de usuario (opcional)

### 4.3. Requisitos no funcionales (opcional)

**R.N.F. 01. Título requisito no funcional**
Como [tipo de usuario]
quiero [servicio]
para [razón]

-- fin entregable 1 --

## 5. Modelo conceptual

### 5.1. Diagramas de clases UML

- con restricciones.

### 5.2. Escenarios de prueba

- con descripción textual y diagrama de objetos UML.

## 6. Matrices de trazabilidad

- Matriz de trazabilidad entre los elementos del modelo conceptual y los requisitos.

|       | EntidadX   | AsociaciónX  | RestricciónX  | Entidad2 ...   | 
|:------|:-----------|:-----------|:-----------|:-----------|
| RI-1  | X          | X          | X          | X          |
| RI-2  |            | X          |            | X          |
| RF-1  |            | X          |            | X          |
| RF-2  | X          |            | X          | X          |
| RN-1  |            | X          |            |            |
| RN-2  | X          | X          | X          |            |
| ...   |            |            |            |            |

-- fin entregable 2 --

## 7. Modelo relacional en 3FN

- Relaciones obtenidas al aplicar la transformación del modelo conceptual.

### 7.1.  Justificación de la estrategia de transformación de jerarquías

- si se identificaron jerarquías en el MC.


### 8. Matriz de trazabilidad MC/SQL (opcional):

- Restricciones sobre el MC / Elementos del modelo tecnológico (SQL) (Triggers, checks, etc.)
- Incluir Reglas de negocio — Constraints/Triggers en las matrices de trazabilidad para el entregable 3

|       | EntidadX   | AsociaciónX  | RestricciónX  | Entidad2 ...   | 
|:-------|:-------|:-------|:-------|:-------|
| TABLA-1 |        |        |        |        |
| TABLA-2 |        |        |        |        |
| TABLA-3 |        |        |        |        |
| TABLA-4 |        |        |        |        |
| TRIG-1 |        |        |        |        |
| TRIG-2 | X      | X      |        | X      |
| TRIG-3 |        | X      |        | X      |
| TRIG-4 |        |        | X      |        |
| CONST-1 |        |        |        |        |
| CONST-2 | X      | X      |        | X      |
| CONST-3 |        | X      |        | X      |
| CONST-4 |        |        | X      |        |

Se consideran todo tipo de constraints declarativas (aquellas definidas durante el CREATE TABLE).
-- fin entregable 3 --

## Referencias


