Cambio Funcional Propuesto: Implementación del Módulo de Reportes
Automáticos de Asistencia
1. Nombre del cambio funcional
“Módulo de Reportes Automáticos y Exportación de Datos”
2. Descripción del cambio y problema que resuelve
Actualmente, la aplicación de control de asistencia cumple adecuadamente con el
registro diario de entrada y salida de los usuarios. Sin embargo, presenta una limitación
significativa: no cuenta con un sistema de generación automática de reportes ni con la
posibilidad de exportar los datos a formatos estándar como PDF o Excel.
El cambio funcional propuesto consiste en el desarrollo e integración de un módulo de
reportes automáticos, capaz de generar informes personalizados filtrando por usuario,
rango de fechas y estado de asistencia (presente, ausente o tardanza). Además, permitirá
exportar los reportes generados en formatos PDF y Excel, facilitando la entrega de
información a las áreas administrativas y de control.
3. Implementación técnica del módulo
3.1 Análisis y diseño del módulo
Se identificarán los campos necesarios del registro de asistencia: nombre del usuario,
fecha, hora de entrada, hora de salida, estado de asistencia y observaciones.
Posteriormente, se diseñará una interfaz intuitiva con filtros configurables para que el
usuario seleccione los criterios del reporte.
3.2 Desarrollo de la funcionalidad
• Se creará una nueva sección en el menú principal denominado “Reportes”.
• Se implementará la generación dinámica de tablas en tiempo real a partir de
consultas SQL optimizadas.
• Se integrarán botones de exportación a PDF y Excel, utilizando librerías
específicas como iText para PDF y Apache POI para Excel.
• Los reportes generados se almacenarán en un historial interno, permitiendo su
consulta y descarga posterior.
3.3 Pruebas y validación
Se realizarán pruebas funcionales y de integración para verificar:
• La exactitud de los datos mostrados
• El correcto funcionamiento de los filtros
• La legibilidad de los reportes exportados
• La integridad del formato en ambos tipos de archivo
3.4 Actualización de la documentación
Se actualizará el manual de usuario para incluir instrucciones sobre el uso del nuevo
módulo. Además, se registrarán los cambios en la documentación técnica y en el
historial de versiones del sistema.
4. Mejora que corrige y beneficios esperados
• Reducción del tiempo de generación de reportes: los usuarios podrán obtener información en segundos, sin recurrir a procesos manuales.
• Eliminación de errores humanos: la automatización garantiza la exactitud de los
datos exportados.
• Mayor trazabilidad y control: los reportes históricos facilitan la revisión de
asistencia en periodos anteriores.
• Mayor productividad: los supervisores y responsables administrativos podrán
concentrarse en el análisis y la toma de decisiones, en lugar de recopilar datos
manualmente.
5. Impacto en la mantenibilidad y calidad del sistema
5.1 Mantenibilidad
El diseño del módulo se realizará bajo una arquitectura modular basada en el patrón
MVC (Modelo–Vista–Controlador), separando la lógica de negocio de la interfaz
gráfica. Esto permitirá realizar futuras actualizaciones o ajustes sin afectar las demás
partes del sistema. Además, al utilizar librerías estándar, se asegura compatibilidad y
facilidad de mantenimiento a largo plazo.
5.2 Calidad del sistema
El cambio funcional propuesto mejora la confiabilidad y la usabilidad del sistema,
brindando información más clara, accesible y verificable. También mejora la experiencia del usuario final al proporcionar un entorno más completo, funcional y
orientado a resultados. Asimismo, contribuye a la calidad interna del software, ya que el
código del nuevo módulo estará documentado, reutilizable y alineado con las buenas
prácticas de desarrollo.
