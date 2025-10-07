
---

### 📄 `02-entidades.md`

```markdown
# 2. Entidades en JPA

Una entidad es una clase que representa una tabla en la base de datos.

### 🧱 Ejemplo:
```java
@Entity
public class Estudiante {
    @Id
    @GeneratedValue
    private Long id;
    private String nombre;
    private int edad;
}
