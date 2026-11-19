# SGA-DO: Sistema de Gestión Académica (DiplomadosOnline.com)

Motor Core (Backend) desarrollado por consola para automatizar el registro académico, cálculo polimórfico de calificaciones y emisión de certificados mediante persistencia en archivos de texto plano (`.txt`).

## Problemática Resuelta
* **Integridad de Datos:** Eliminación de duplicados y errores manuales derivados del uso de hojas de cálculo.
* **Persistencia:** Almacenamiento seguro e inmediato en `alumnos.txt` y `profesores.txt`.
* **Automatización de Certificados:** Generación automática de reportes (`certificados_pendientes.txt`) mediante estructuras tipo Cola (FIFO).

## Arquitectura y Estructuras de Datos
* **POO:** Herencia (`Persona` -> `Alumno`, `Profesor`) y Polimorfismo (`ProgramaAcademico` -> `Curso`, `Diplomado`, `Bootcamp`).
* **Pila (LIFO):** Implementada para la función *Deshacer Último Registro de Nota* (`Ctrl + Z`).
* **Cola (FIFO):** Implementada para procesar en orden a los estudiantes aprobados.

## Contenido del Repositorio
* `/docs`: Análisis de negocio, requerimientos del MVP y Diagrama de Clases UML.
* `/python`: Código fuente en Python.
* `/java`: Código fuente en Java.
* `/cpp`: Código fuente en C++.
