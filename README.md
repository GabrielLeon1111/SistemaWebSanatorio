# Sistema de Gestión

Sistema integral de gestión hospitalaria desarrollado en GeneXus V18, 
que digitaliza el flujo completo: desde la recepción del paciente 
hasta la atención médica y facturación.

## Capturas

<img width="1432" height="927" alt="image" src="https://github.com/user-attachments/assets/a59f612b-f077-4990-bff1-340212ee02b8" />
<img width="1365" height="945" alt="image" src="https://github.com/user-attachments/assets/115ac9de-2595-4758-b558-ef09debdc301" />
<img width="1681" height="422" alt="image" src="https://github.com/user-attachments/assets/4aa988e1-8872-4a33-aa29-2650e1a84cab" />
<img width="1488" height="912" alt="image" src="https://github.com/user-attachments/assets/5120e25a-ea59-4214-b9b7-01e54f48f974" />
<img width="1910" height="902" alt="image" src="https://github.com/user-attachments/assets/52d5fd9a-1a55-4e34-9cdb-700390022003" />

## Funcionalidades

**Recepción**
- Búsqueda de paciente por cédula con autocompletado
- Registro sin documento cuando es necesario
- Generación dinámica de horarios disponibles según médico: 
  calcula slots automáticamente (ej. cada 30 min) entre el 
  horario de inicio y fin de atención, y descarta los turnos 
  ya ocupados en tiempo real

**Enfermería**
- Registro de signos vitales y triaje
- Sincronización en tiempo real con el médico

**Médico**
Autenticación y permisos vía GeneXus Access Manager (GAM)
Gestión de estado del paciente:
Atendido: consulta finalizada
Ausente: el paciente no se presentó, se elimina de la lista del día
Pasar para después: si el paciente no llega a tiempo, no pierde el turno — pasa al final de la cola y es atendido más tarde ese mismo día, sin afectar a los demás pacientes

**Caja** *(en desarrollo)*
- Apertura y cierre de caja
- Facturación electrónica

## Stack tecnológico
- **Herramienta:** GeneXus V18
- **Backend:** Java (Apache Tomcat)
- **Base de datos:** SQL Server
- **Seguridad:** GAM

## Estado del proyecto
✅ Recepción, Enfermería y Médico — funcional
🔜 Módulo de Caja y reportes gerenciales — en desarrollo
