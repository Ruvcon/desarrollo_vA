# 🎓 Sistema de Gestión Académica para Posgrado · UTN FRLP

> Actividad Práctica · Desarrollo de Software · Metodología Ágil

---

# 📌 Product Backlog

# 👥 Actores del Sistema

| Actor | Descripción |
|---|---|
| Aspirante | Solicita inscripción y carga documentación |
| Estudiante | Realiza cursadas y seguimiento académico |
| Docente | Registra asistencia y calificaciones |
| Conducción / CPR | Supervisa, administra y genera reportes |

---

# 🧩 Épicas del Sistema

| ID | Épica |
|---|---|
| EP-01 | Gestión de Inscripciones |
| EP-02 | Legajo y Perfil Académico |
| EP-03 | Gestión Docente |
| EP-04 | Estadísticas y Reportes |
| EP-05 | Administración del Sistema |

---

# 📋 Product Backlog

| ID | Épica | Historia de Usuario | Criterios de Aceptación | SP | Prioridad | Sprint |
|---|---|---|---|---|---|---|
| US-01 | EP-01 | Como aspirante, quiero acceder a un formulario web, para inscribirme sin enviar correos. | **Dado** que ingresa al enlace, **cuando** completa los campos obligatorios, **entonces** el sistema guarda los datos.<br><br>**Dado** que finaliza la inscripción, **cuando** envía el formulario, **entonces** recibe una confirmación. | 5 | M | 1 |
| US-02 | EP-01 | Como aspirante, quiero adjuntar documentos PDF, para completar mi legajo digital. | **Dado** que selecciona archivos PDF, **cuando** los sube, **entonces** el sistema los valida.<br><br>**Dado** que los documentos son válidos, **cuando** finaliza la carga, **entonces** quedan almacenados en el legajo. | 3 | M | 1 |
| US-03 | EP-01 | Como conducción, quiero visualizar el estado del legajo, para verificar si está completo. | **Dado** que accede al panel, **cuando** revisa un aspirante, **entonces** observa un indicador visual.<br><br>**Dado** que faltan documentos, **cuando** visualiza el estado, **entonces** el sistema informa pendientes. | 3 | M | 2 |
| US-04 | EP-02 | Como conducción, quiero registrar asistencia y notas, para actualizar el estado académico del estudiante. | **Dado** que ingresa las notas, **cuando** confirma la carga, **entonces** el perfil académico se actualiza.<br><br>**Dado** que registra asistencia, **cuando** guarda los cambios, **entonces** el porcentaje se recalcula automáticamente. | 5 | M | 2 |
| US-05 | EP-03 | Como docente, quiero acceder mediante un enlace a mi planilla, para cargar asistencia sin usuario ni contraseña. | **Dado** que recibe el enlace, **cuando** lo abre, **entonces** accede a la planilla correspondiente.<br><br>**Dado** que el enlace es válido, **cuando** ingresa, **entonces** puede registrar asistencia y notas. | 3 | S | 3 |
| US-06 | EP-02 | Como conducción, quiero registrar tutorías y seguimiento del trabajo final, para monitorear el avance académico. | **Dado** que se registra una tutoría, **cuando** se guarda la información, **entonces** queda asociada al estudiante.<br><br>**Dado** que se consulta el perfil, **cuando** existen tutorías registradas, **entonces** se muestran cronológicamente. | 5 | S | 3 |
| US-07 | EP-02 | Como CPR, quiero cargar información de tesis o TFI, para mantener actualizado el estado del estudiante. | **Dado** que la carrera es maestría o doctorado, **cuando** se carga la tesis, **entonces** el sistema solicita director y resolución.<br><br>**Dado** que se completa la información, **cuando** se guarda, **entonces** queda registrada en el perfil académico. | 5 | M | 4 |
| US-08 | EP-02 | Como conducción, quiero visualizar un semáforo de avance académico, para conocer el estado del estudiante. | **Dado** que el estudiante posee materias aprobadas, **cuando** se consulta el perfil, **entonces** se muestra el estado de avance.<br><br>**Dado** que existen retrasos, **cuando** se visualiza el perfil, **entonces** el sistema genera alertas. | 3 | S | 4 |
| US-09 | EP-03 | Como docente, quiero descargar la planilla de cursada, para utilizarla en formato analógico. | **Dado** que accede a la planilla, **cuando** selecciona descargar, **entonces** obtiene el archivo correspondiente.<br><br>**Dado** que la descarga finaliza, **cuando** abre el archivo, **entonces** visualiza los datos de estudiantes. | 2 | C | 4 |
| US-10 | EP-03 | Como sistema, quiero enviar recordatorios automáticos a docentes, para evitar retrasos en la carga académica. | **Dado** que no se completó la carga, **cuando** vence el plazo establecido, **entonces** el sistema envía un correo automático.<br><br>**Dado** que el docente completa la carga, **cuando** se verifica el estado, **entonces** dejan de enviarse recordatorios. | 5 | S | 5 |
| US-11 | EP-04 | Como conducción, quiero generar estadísticas por cohorte, para analizar el estado de las carreras. | **Dado** que existen cohortes registradas, **cuando** se solicita un reporte, **entonces** el sistema genera estadísticas.<br><br>**Dado** que se selecciona una cohorte, **cuando** se consulta información, **entonces** se muestran indicadores académicos. | 5 | M | 5 |
| US-12 | EP-04 | Como conducción, quiero consultar niveles de desgranamiento y graduados, para evaluar el rendimiento académico. | **Dado** que existen datos académicos, **cuando** se genera el informe, **entonces** se calcula el nivel de desgranamiento.<br><br>**Dado** que se consulta el reporte, **cuando** existen graduados, **entonces** se visualiza la cantidad total. | 5 | S | 5 |
| US-13 | EP-05 | Como conducción, quiero abrir o cerrar períodos de inscripción, para controlar las convocatorias activas. | **Dado** que el administrador accede al panel, **cuando** modifica el estado de inscripción, **entonces** el sistema actualiza la disponibilidad.<br><br>**Dado** que la inscripción está cerrada, **cuando** un aspirante intenta ingresar, **entonces** el sistema informa que no está disponible. | 3 | M | 2 |
| US-14 | EP-05 | Como conducción, quiero buscar estudiantes por cohorte o nombre, para acceder rápidamente a su información. | **Dado** que existen estudiantes registrados, **cuando** se realiza una búsqueda, **entonces** el sistema devuelve coincidencias.<br><br>**Dado** que se selecciona un estudiante, **cuando** se abre su perfil, **entonces** se muestran todos sus datos académicos. | 3 | M | 3 |
| US-15 | EP-04 | Como conducción, quiero descargar reportes académicos, para compartir información institucional. | **Dado** que se genera un reporte, **cuando** selecciona exportar, **entonces** el sistema descarga el archivo.<br><br>**Dado** que el archivo es descargado, **cuando** se abre, **entonces** contiene la información solicitada. | 3 | C | 5 |

---

# 📊 Escala de Estimación

| Story Points | Complejidad |
|---|---|
| 1 | Muy simple |
| 2 | Simple |
| 3 | Moderada |
| 5 | Compleja |
| 8 | Muy compleja |
| 13 | Épica / subdividir |

---

# 🏷️ Prioridad MoSCoW

| Código | Significado |
|---|---|
| M | MUST — Imprescindible |
| S | SHOULD — Importante |
| C | COULD — Deseable |
| W | WON'T — No incluido |

---

# 🚀 Organización de Sprints

| Sprint | Objetivo |
|---|---|
| Sprint 1 | Inscripción y carga de documentación |
| Sprint 2 | Gestión académica y administración |
| Sprint 3 | Gestión docente y búsquedas |
| Sprint 4 | Seguimiento académico y tesis |
| Sprint 5 | Estadísticas, reportes y automatizaciones |

---

# 📚 Tecnologías Sugeridas

- Frontend: HTML, CSS, JavaScript
- Backend: Node.js / Java / PHP
- Base de Datos: MySQL / PostgreSQL
- Control de versiones: Git + GitHub

---

# 🏫 Universidad Tecnológica Nacional
## Facultad Regional La Plata

**Materia:** Desarrollo de Software  
**Trabajo Práctico:** Product Backlog  
**Metodología:** Scrum / Agile
****
