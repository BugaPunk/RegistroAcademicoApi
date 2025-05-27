# Proyecto CRUD - Universidad

Este repositorio contiene la base del proyecto Universitario utilizando **Spring Boot**. Cada grupo debe trabajar en su propia rama según las instrucciones del docente.

---

## 🚀 Objetivo

El proyecto ya incluye un frontend básico con funcionalidades para crear y editar estudiantes; su tarea consiste en agregar la funcionalidad para eliminar registros mediante una baja lógica.

## 📝 Implementación de Baja Lógica de Estudiantes

Se ha implementado la funcionalidad de baja lógica para estudiantes en el frontend, aprovechando la API existente en el backend. Esta implementación permite dar de baja a un estudiante sin eliminarlo físicamente de la base de datos.

### Características implementadas:

- **Modal de baja lógica**: Se agregó un modal que solicita el motivo de baja del estudiante.
- **Validación de datos**: Se verifica que el motivo de baja no esté vacío antes de enviar la solicitud.
- **Registro completo**: Se envía al backend el motivo de baja, el usuario que realiza la operación y la fecha.
- **Feedback visual**: Se muestra un indicador de carga durante el proceso y mensajes de éxito o error.

### Detalles técnicos:

- Se modificó la función `deleteStudent()` para que abra el modal de baja lógica.
- Se implementó la función `confirmDeleteStudent()` que realiza la llamada al endpoint `/api/estudiantes/{id}/baja`.
- No fue necesario modificar el backend, ya que la API ya contaba con toda la funcionalidad requerida.
/github.com/LiaRos-ai/RegistroUniversitario.git