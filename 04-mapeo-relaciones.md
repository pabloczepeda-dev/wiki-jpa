
---

### 📄 `04-mapeo-relaciones.md`

```markdown
# 4. Mapeo de Relaciones

JPA permite definir relaciones entre entidades como en una base de datos relacional.

### 🔹 Tipos de relaciones:
- `@OneToOne`: Uno a uno
- `@OneToMany`: Uno a muchos
- `@ManyToOne`: Muchos a uno
- `@ManyToMany`: Muchos a muchos

### 📘 Ejemplo `@OneToMany`:
```java
@Entity
public class Autor {
    @Id
    private Long id;
    private String nombre;

    @OneToMany(mappedBy = "autor")
    private List<Libro> libros;
}
