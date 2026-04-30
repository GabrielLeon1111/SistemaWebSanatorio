# Sistema de Gestión - Sanatorio Merssan

Sistema integral desarrollado en **GeneXus V18** para la digitalización de procesos hospitalarios, desde la recepción hasta el historial clínico.

### 🚀 Módulos y Flujos de Trabajo
Actualmente, el sistema cuenta con los siguientes pilares operativos detallados por rol y nivel de avance:

#### **Rol: Recepcionista (95%)**
Interfaz unificada para una admisión eficiente y gestión de agenda:
* **Admisión Inteligente y Flexible:** 
    * El sistema permite buscar al paciente por número de cédula para autocompletar datos automáticamente.
    * **Flexibilidad de registro:** En caso de que el paciente no cuente con documento, el sistema permite realizar el agendamiento utilizando únicamente el nombre, garantizando la atención en cualquier circunstancia.
* **Selección Guiada de Especialista:** El paciente indica la especialidad requerida y el sistema despliega los médicos disponibles. El recepcionista informa sobre los profesionales disponibles y sus respectivos días de atención.
* **Asignación de Turnos y Horarios:** 
    * Cálculo automático de fechas válidas según la configuración de cada médico.
    * Gestión de horarios: El sistema asigna un horario por defecto o permite al paciente elegir su bloque preferido según la disponibilidad.
    * Exclusión de bloques ocupados para evitar duplicidades.

#### **Rol: Lic. en Enfermería (95%)**
Módulo de triaje y preparación clínica:
* **Control de Pre-consulta:** Registro detallado de signos vitales (peso, presión arterial, síntomas).
* **Gestión de Datos:** Capacidad de insertar y modificar datos clínicos, con restricciones de eliminación para asegurar la trazabilidad.
* **Interoperabilidad:** Sincronización en tiempo real de los datos cargados para que el médico los visualice al iniciar la atención.

#### **Rol: Médico (70%)**
Gestión de consulta personalizada e integración con seguridad:
* **Seguridad con GAM:** Autenticación vía GeneXus Access Manager que vincula al usuario con su perfil profesional, restringiendo el acceso únicamente a sus pacientes y especialidad.
* **Gestión de Estados:** Work-with dinámico para marcar pacientes como ✅ Atendido, ❌ Ausente o 🔄 Pasar para después (reordenamiento automático de la cola).

### 🛠️ Stack Tecnológico
* **Herramienta:** GeneXus V18 (Upgrade 3+).
* **Generador:** Java (Despliegue en Apache Tomcat).
* **Base de Datos:** SQL Server.
* **Seguridad:** GAM (GeneXus Access Manager).

### 📈 Objetivos en Desarrollo (Próximas Implementaciones)

#### **Rol: Cajera**
* **Gestión de Apertura y Cierre de Caja:** Control del ciclo diario (monto inicial, ingresos automáticos y resumen de jornada auditado por responsable).
* **Control de Movimientos:** Registro detallado de flujo de efectivo, incluyendo retiros operativos con fecha, monto y motivo.
* **Facturación Electrónica:** Vinculación con el paciente para cobro de servicios mediante tarjeta de crédito, débito y medios electrónicos.

#### **Otros Módulos**
* **Triage Avanzado:** Clasificación de urgencias médicas según gravedad y tiempos de espera.
* **Reportes Gerenciales:** Estadísticas de turnos, movimientos de caja y pacientes atendidos.

---
*Nota: Este proyecto es un portafolio técnico que demuestra el uso de herramientas de alta productividad, seguridad avanzada (GAM) y modelado de bases de datos relacionales.*
