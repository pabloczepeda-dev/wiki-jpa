# 6. Ciclo de Vida de una Entidad

Las entidades en JPA pasan por varios estados:

| Estado     | Descripción                                      |
|------------|--------------------------------------------------|
| New        | Objeto nuevo, aún no en la BD.                   |
| Managed    | Administrado por el `EntityManager`.             |
| Detached   | Fue persistido, pero ya no está gestionado.      |
| Removed    | Marcado para eliminación.                        |

### 🔁 Transiciones:
```text
New → persist() → Managed  
Managed → remove() → Removed  
Managed → detach() → Detached  
Detached → merge() → Managed
