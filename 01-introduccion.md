# 1. Introducción a JPA

**Java Persistence API (JPA)** es una especificación que facilita el manejo de datos persistentes en aplicaciones Java. Permite mapear clases Java a tablas de bases de datos relacionales.

### ✅ Ventajas:
- Reduce la necesidad de escribir SQL.
- Desacopla el acceso a datos de la lógica del negocio.
- Compatible con múltiples proveedores (Hibernate, EclipseLink, etc.)

### 📌 Ejemplo real:
Guardar un estudiante en la base de datos sin escribir SQL manual:
```java
entityManager.persist(estudiante);
