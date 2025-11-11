# Caso 5: Aplicación de Control de Asistencia

## 1. Descripción del Caso
[cite_start]Sistema que registra la asistencia de estudiantes a clase[cite: 10, 12]. [cite_start]El sistema busca modernizar y simplificar el proceso de asistencia, reduciendo errores y proporcionando datos en tiempo real[cite: 15].

## 2. Objetivos
[cite_start]El objetivo es simplificar el proceso de control de asistencia, proporcionar datos precisos para el seguimiento del rendimiento estudiantil y mejorar la comunicación entre estudiantes, profesores y administradores[cite: 18].

## 3. Requerimientos
Se definieron requerimientos funcionales y no funcionales clave.

### Requerimientos Funcionales
* [cite_start]**RF-01: Registro de Asistencia:** Permitir a los estudiantes registrar su asistencia escaneando un código QR único[cite: 29].
* [cite_start]**RF-02: Generación de Reportes:** Permitir a los profesores generar reportes de asistencia por clase y estudiante (PDF/CSV)[cite: 32].
* [cite_start]**RF-03: Gestión de Usuarios:** Permitir a los administradores gestionar cuentas de estudiantes y profesores[cite: 35].
* [cite_start]**RF-04: Autenticación:** Requerir que todos los usuarios se autentiquen con nombre de usuario y contraseña[cite: 38].
* [cite_start]**RF-05: Notificaciones:** Enviar notificaciones automáticas a estudiantes sobre su historial de faltas[cite: 42].

### Requerimientos No Funcionales
* [cite_start]**RNF-01: Rendimiento:** El registro de asistencia debe tardar menos de 2 segundos[cite: 46].
* [cite_start]**RNF-02: Seguridad:** Garantizar la confidencialidad de los datos mediante encriptación[cite: 47].
* [cite_start]**RNF-03: Usabilidad:** La interfaz debe ser intuitiva y fácil de usar[cite: 49].

## 4. Tabla de Pruebas
[cite_start]Se diseñaron los siguientes casos de prueba para validar las funcionalidades clave:

| Caso de prueba | Requerimiento asociado | Datos de entrada | Resultado esperado |
| :--- | :--- | :--- | :--- |
| Registro válido QR | Registro de asistencia | Código QR válido, usuario estudiante, hora dentro del rango | [cite_start]Registro exitoso de asistencia con fecha y hora correctas [cite: 52] |
| Registro fuera de hora | Registro de asistencia | Código QR válido, usuario estudiante, hora fuera del rango | [cite_start]Error: registro no permitido fuera del horario [cite: 52] |
| Generación de reporte | Generación de reportes | Solicitud de reporte para una clase específica | [cite_start]Reporte PDF/CSV con lista completa y estado de asistencia [cite: 52] |
| Creación de usuario | Gestión de usuarios | Datos de nuevo usuario administrador | [cite_start]Usuario creado y disponible en el sistema [cite: 52] |
| Envío de notificación | Notificaciones | Historial de asistencia con faltas acumuladas | [cite_start]Estudiante recibe notificación con resumen [cite: 52] |

## 5. Tipo de Mantenimiento Propuesto
[cite_start]Se propone un **Mantenimiento Perfectivo**[cite: 240, 265].

[cite_start]**Nombre del cambio:** "Módulo de Reportes Automáticos y Exportación de Datos"[cite: 184].

[cite_start]**Problema que resuelve:** Actualmente, la aplicación registra la asistencia, pero no cuenta con un sistema de generación automática de reportes ni exportación a PDF o Excel[cite: 187].

**Descripción de la Propuesta:**
[cite_start]Se propone el desarrollo e integración de un módulo de reportes automáticos[cite: 188]. Este módulo permitirá a los profesores y administradores:
1.  [cite_start]Generar informes personalizados filtrando por usuario, rango de fechas y estado de asistencia (presente, ausente, tardanza)[cite: 188].
2.  [cite_start]Exportar dichos reportes en formatos PDF y Excel[cite: 189].

[cite_start]Este cambio mejora la eficiencia, reduce errores humanos y optimiza el tiempo de trabajo administrativo[cite: 212, 213, 215].

## 6. Reflexión sobre Control de Versiones (Git/GitHub)
El control de versiones es fundamental en la documentación técnica de un proyecto de software. Herramientas como Git y GitHub nos permiten mantener un historial de cada cambio realizado en los requerimientos, planes de prueba y manuales.

Esto es útil porque:
1.  **Trazabilidad:** Podemos ver exactamente *quién* cambió un requerimiento, *cuándo* lo hizo y *por qué* (a través de los mensajes de "commit").
2.  **Trabajo en Paralelo:** Permite que diferentes personas trabajen en diferentes documentos (como `DRS_v1` y `DRS_v2`) sin sobreescribir el trabajo del otro.
3.  **Recuperación:** Si una nueva versión de un documento introduce un error o elimina información importante, podemos "regresar en el tiempo" fácilmente a una versión anterior que funcionaba.

[cite_start]En este proyecto, usar control de versiones nos habría permitido gestionar la evolución del `DRS_v1` al `DRS_v2` [cite: 263] de manera ordenada, sabiendo qué requerimientos se agregaron en la segunda versión.