
---

### 📄 `03-persistencia.md`

```markdown
# 3. Persistencia

Persistir significa guardar el estado de un objeto en una base de datos.

### 🔹 Ejemplo:
```java
Estudiante est = new Estudiante();
est.setNombre("Laura");
est.setEdad(22);
entityManager.persist(est);
