#  Sistema de Gestión Integral - Gimnasio Forza Entrenamientos

##  1. Propuesta de Proyecto – Descripción y Objetivo
La propuesta consiste en desarrollar un **sistema de gestión integral** para el gimnasio **Forza Entrenamientos**.  

El **objetivo principal** es centralizar y digitalizar los procesos administrativos y operativos del gimnasio, logrando mayor eficiencia y control tanto para el **dueño** como para los **profesores**.  

Esto permitirá:  
- Gestionar inscripciones de alumnos.  
- Controlar pagos.  
- Administrar turnos fijos por días y horarios.  
- Asignar rutinas a los alumnos.  
- Brindar a los usuarios acceso a su información personal y estado de pagos.  

---

##  2. Alcance (Inclusiones, Exclusiones, Supuestos y Restricciones)

###  Inclusiones
- ABM (alta, baja, modificación) de alumnos.  
- ABM de turnos y horarios.  
- Asignación de turnos a alumnos por parte de los profesores.  
- Gestión de pagos.  
- Login de usuarios.  
- Visualización de horarios y estado de pagos por parte de los alumnos.  
- Carga de datos personales y apto médico.  
- Registro y asignación de rutinas por parte de los profesores.  

###  Exclusiones
- No se incluye pasarela de pago online en esta primera versión (los pagos se registran de manera manual).  
- No se incluye aplicación móvil nativa (el acceso será vía web responsive).  
- No se contempla integración con sistemas contables externos.  

###  Supuestos
- Los alumnos mantienen un día y horario fijo (no hay sistema de reservas dinámicas).  
- El gimnasio cuenta con un número limitado de profesores que gestionarán los turnos.  
- Todos los usuarios cuentan con acceso a internet para ingresar al sistema.  

###  Restricciones
- El sistema deberá estar disponible vía web.  
- Se priorizará la usabilidad y la facilidad de uso sobre la complejidad de funcionalidades.  
- El desarrollo deberá completarse en un plazo acotado (ej: 3-4 meses).  

---

##  3. Interesados y su Impacto
- **Dueño del gimnasio** → Impacto **alto**, tendrá control total de la administración y reportes.  
- **Profesores** → Impacto **medio/alto**, asignan turnos, rutinas y verifican pagos.  
- **Alumnos** → Impacto **medio**, acceso a perfil, turnos y estado de pagos.  
- **Equipo de desarrollo** → Impacto **alto**, responsables del diseño, implementación y mantenimiento.  

---

##  4. Criterios de Aceptación Verificables

###  ABM de Alumnos
- El sistema debe permitir registrar un nuevo alumno con nombre, apellido, DNI, contacto y apto médico digitalizado.  
- El sistema debe permitir modificar y eliminar un alumno existente.  
- El sistema debe listar a los alumnos activos e inactivos.  

###  Gestión de Turnos
- El sistema debe permitir crear turnos con día, horario y capacidad máxima.  
- El sistema debe permitir asignar alumnos a turnos de acuerdo con su plan contratado.  
- El sistema debe impedir sobrepasar la capacidad máxima de un turno.  

###  Registro de Pagos
- El sistema debe permitir registrar el pago mensual de un alumno indicando fecha y monto.  
- El alumno debe poder visualizar en su perfil el estado de su pago (**al día** / **atrasado**).  
- El sistema debe emitir una alerta al profesor/dueño en caso de alumno con pago vencido.  

---
