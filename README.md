# Gimnasio

## Miembros del grupo L3-ABS-2

1. Gallego Cal, Guillermo
1. Sanchez Gonzalez, Alejandro
1. Khattabi El Inani, Ilias
1. Apellidos, Nombre

## 1. Introducción al problema

- Descripción del problema para poner en contexto el proyecto, incluyendo información sobre los clientes y usuarios, la situación actual, problemas, expectativas, etc. Se valorará la presencia de información multimedia (fotos, gráficos, documentos escaneados, etc.).

## 2. Glosario de términos

- Términos específicos del dominio del problema, ordenados alfabéticamente. Se valorará la presencia de información multimedia.

## 3. Visión general del sistema

### 3.1. Requisitos generales

### 3.2. Usuarios del sistema

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


