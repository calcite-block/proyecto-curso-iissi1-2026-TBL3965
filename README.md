# Gimnasio

## Miembros del grupo L3-ABS-2

1. Gallego Cal, Guillermo
1. Sanchez Gonzalez, Alejandro
1. Khattabi El Inani, Ilias
1. Apellidos, Nombre

## 1. Introducción al problema

### 1.1. Contexto y situación actual

Hoy en día, el mundo del gimnasio y el deporte de fuerza ha crecido muchísimo, ya que cada vez más gente busca entrenar en serio y cuidar su físico. Sin embargo, al analizar el sector nos encontramos con que hay muchísima competencia, pero casi toda cae en uno de estos dos extremos:

* **Los gimnasios comerciales o *low-cost*:** Compiten tirando los precios, pero a cambio están siempre masificados en hora punta, les falta maquinaria específica para entrenar pesado de verdad y apenas hay seguimiento por parte de los monitores.
* **Los centros pequeños o especializados (boxes o gimnasios de barrio):** Aunque a veces tienen buen material para una disciplina concreta, se quedan cortos si buscas variedad y, sobre todo, suelen llevar toda la gestión a la antigua (con fichas de papel, hojas de Excel sueltas o grupos de WhatsApp), lo que acaba siendo un caos tanto para el dueño como para el que va a entrenar.

Viendo este problema, nuestro proyecto consiste en abrir **[NOMBRE DEL GIMNASIO]**, con el objetivo de montar el centro deportivo más completo de la zona y desmarcarnos de la competencia. La idea es juntar en una misma instalación, bien dividida por salas y zonas específicas, las cuatro grandes ramas del entrenamiento actual:

1. **Zona de Culturismo y Musculación:** Equipada con máquinas seleccionadas por su biomecánica y peso libre para trabajar de forma completa todos los grupos musculares (pecho, espalda, pierna y brazo).
2. **Zona de *Powerlifting*:** Preparada para el entrenamiento de fuerza con jaulas de potencia (*racks*), plataformas de peso muerto, bancos reglamentarios y discos calibrados.
3. **Zona de Calistenia y *Street Workout*:** Una estructura completa con barras de dominadas, paralelas y anillas pensada tanto para básicos y repeticiones como para ejercicios de tensión y lastre.
4. **Box de *CrossFit* y Entrenamiento Funcional:** Salas amplias orientadas a entrenamientos de alta intensidad y clases colectivas dirigidas por entrenadores.

<img src="maquinas.webp" alt="Instalaciones y máquinas del gimnasio" width="350">

Para que un gimnasio tan grande y con tantas disciplinas funcione sin volverse un descontrol, no basta con tener las mejores instalaciones físicas; necesitamos acompañarlo desde el primer día de un Sistema de Información propio que automatice toda la gestión.

### 1.2. Problemas que queremos resolver

Cuando un centro deportivo ofrece tantas opciones (clases dirigidas, distintas salas, entrenadores especializados y varios tipos de cuotas), intentar llevar el control de forma manual o con programas básicos que no están conectados entre sí genera problemas diarios muy claros:

* **Salas llenas y falta de espacio (*Overbooking*):** En disciplinas como *CrossFit*, calistenia o entrenamientos guiados de fuerza, el espacio y el material (barras, jaulas, máquinas) son limitados. Si no se controla automáticamente cuánta gente reserva en función de la capacidad máxima de cada sala, se juntan demasiadas personas a la vez, se entrena mal y se pierde calidad frente a la competencia.
* **Descontrol con las matrículas y los pagos:** Al manejar distintos planes de membresía de forma manual, es muy fácil que se pasen por alto matrículas que ya han caducado, que no quede claro quién tiene pagos pendientes o que por error administrativo se le duplique la matrícula activa a un mismo socio.
* **Descoordinación en horarios y entrenadores:** Cuadrar a mano qué entrenador da cada clase según su especialidad, en qué sala y a qué hora suele provocar solapamientos. Además, los entrenadores llegan a dar su clase a ciegas, sin saber cuánta gente se ha apuntado hasta que entran por la puerta.
* **Pérdida de tiempo para el socio en recepción:** Tener que ir al mostrador o preguntar en recepción solo para saber cuándo te caduca el mes, ver los horarios de las clases o reservar plaza hace que se formen colas innecesarias y da una imagen anticuada del gimnasio.

<img src="horario.avif" alt="Organización de horarios del gimnasio" width="300">

### 1.3. Clientes y usuarios en el contexto del proyecto

Dentro del contexto de nuestro proyecto, diferenciamos entre quién encarga el sistema y quiénes lo van a usar en el día a día del gimnasio (cuyas funciones detalladas dentro de la aplicación se especificarán más adelante en el documento):

* **El Cliente:** Es la **Dirección o Gerencia de [NOMBRE DEL GIMNASIO]**. Son los propietarios que invierten en el proyecto y ponen las reglas del negocio. Lo que buscan con este software es llevar las cuentas claras, evitar que entre gente con la cuota vencida, aprovechar al máximo las salas y conseguir que el gimnasio destaque por encima de cualquier competidor.
* **Los Usuarios:** Son las personas que van a interactuar con el sistema en el gimnasio:
  * **El personal de administración:** Los encargados de llevar el control general del centro (altas de socios, configuración de planes, matrículas, cobros y organización de salas, clases y horarios).
  * **Los entrenadores:** Los profesionales de cada área deportiva, que necesitan tener clara su agenda de clases, en qué sala les toca y qué volumen de reservas tienen para organizar la sesión.
  * **Los socios:** Los deportistas inscritos en el gimnasio, que buscan poder gestionar sus reservas a las clases y consultar el estado de su matrícula y sus pagos de forma rápida y sin complicaciones.

<img src="images.jpg" alt="Entrenador y socios" width="250">

### 1.4. Expectativas y objetivos

Con la puesta en marcha de este sistema de gestión, nuestras expectativas son:

1. **Centralizar toda la información del gimnasio:** Dejar atrás el papel y las hojas de cálculo sueltas para tener todos los datos de socios, matrículas, planes, pagos, entrenadores, salas, horarios y reservas guardados de forma segura y ordenada en un único sitio.
2. **Asegurar que se cumplan las normas del centro automáticamente:** Que sea el propio programa el que impida errores habituales, como que alguien reserve con la matrícula caducada, que se supere el aforo máximo de una sala o que se intente reservar una clase que ya ha empezado.
3. **Mejorar la experiencia diaria en el gimnasio:** Conseguir que tanto la administración como los entrenadores y los socios ahorren tiempo en gestiones, logrando que **[NOMBRE DEL GIMNASIO]** sea referente no solo por sus zonas de culturismo, *powerlifting*, calistenia y *CrossFit*, sino también por lo cómodo y bien organizado que está.

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

### 3.1. Requisitos generales

### 3.2. Usuarios del sistema

Los usuarios del sistema son aquellas personas las cuales van a utilizar la aplicación y realizar operaciones con ella. En nuestro sistema de gestión del  Gimnasio, tenemos tres usuarios posibles, que son el administrador del gimnasio, el socio y el entrenador. Cada uno tendrá diferentes responsabilidades y funcionalidades según su papel dentro del gimnasio.

El administrador del gimnasio es quien gestiona la información general del gimnasio. Tendrá acceso a las funciones de gestión de socios, planes de membresía, matrículas, entrenadores, clases, salas, horarios y pagos. Su función principal será garantizar el correcto funcionamiento y la organización de las actividades del gimnasio.

El socio será el usuario que esté inscrito en el gimnasio y utilice el sistema para consultar y gestionar su actividad. Podrá consultar el estado y la fecha de finalización de su matrícula, visualizar las clases disponibles y sus horarios, realizar o cancelar reservas y consultar la información de sus pagos.

El entrenador será el profesional encargado de impartir las clases y actividades del gimnasio. A través del sistema podrá consultar las clases que tiene asignadas, revisar sus horarios y las salas en las que se desarrollan, así como consultar las reservas de sus clases para conocer la asistencia prevista.

## 4. Catálogo de requisitos

### 4.1. Requisitos funcionales

#### R.F.01. Gestión de socios
-   Como administrador del gimnasio quiero registrar, modificar y consultar los datos de los socios para mantener actualizada su información personal.

#### R.F.02. Gestión de planes
-   Como administrador del gimnasio quiero crear, modificar y consultar los planes de membresía para gestionar las diferentes opciones disponibles para los socios.

#### R.F.03. Gestión de matrículas
-   Como administrador del gimnasio quiero registrar y gestionar las matrículas de los socios, indicando el plan, la fecha de inicio y la fecha de fin para
  controlar la vigencia de sus membresías.

#### R.F.04. Consulta del estado de la matrícula
-   Como socio quiero consultar el estado y la fecha de finalización de mi matrícula para saber si mi membresía está activa y cuándo caduca.

#### R.F.05. Gestión de entrenadores
-   Como administrador del gimnasio quiero registrar y gestionar los datos de los entrenadores y su especialidad para mantener actualizada la información del personal encargado de las clases.

#### R.F.06. Gestión de clases
-   Como administrador del gimnasio quiero crear y gestionar las clases, indicando su nombre, descripción, duración, capacidad máxima, y entrenador para organizar la oferta de actividades del gimnasio.

#### R.F.07. Gestión de salas
- Como administrador del gimnasio quiero registrar y gestionar las salas, indicando su capacidad y ubicación para organizar los espacios donde se realizan las clases.

#### R.F.08. Gestión de horarios
- Como administrador del gimnasio quiero establecer y consultar los horarios de las clases para organizar la programación de actividades del gimnasio.

#### R.F.09. Gestión de reservas
- Como socio quiero reservar y cancelar mi asistencia a las clases para poder organizar mi participación en las actividades del gimnasio.

#### R.F.10. Gestión de pagos
- Como administrador del gimnasio quiero registrar y consultar los pagos realizados por los socios, indicando el importe, la fecha, el método de pago y el estado para llevar un control de los pagos y de las matrículas.

**Prueba de aceptación**
- Descripción de la primera comprobación a realizar
- Descripción de la segunda comprobación a realizar
- Se debe aplicar la regla de negocio R.N.XX.
- ...

#### 4.1.1. Requisitos de información

##### R.I.01. Título requisito de información

Como [tipo de usuario]
quiero [servicio]
para [razón]

**Prueba de aceptación**
- Descripción de la primera comprobación a realizar
- Descripción de la segunda comprobación a realizar
- ...

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


