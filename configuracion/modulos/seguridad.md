---
description: Característica Premium
---

# Seguridad

Este módulo permite proteger tu servidor. Esto puede ser usado como verificación, pero lo puedes usar para cualquier cosa que te imagines.

Esta configuración es super simple:

```yaml
security:
  ignored_users: []
  access:
    - password: 'Password 1'
      roles:
        - 'Role ID 1'
        - 'Role ID 2'
    - password: 'Password 2'
      roles:
        - 'Role ID 3'
```

**Ignored Users:** lista de usuario que no pueden utilizar el módulo.

**Access:** lista de contraseñas y roles. Puedes añadir la cantidad que quieras. Esta es la estructura:

* **Password:** el código secreto que se debe usar en el comando.
* **Roles:** lista de roles que se añadirán si el usuario utiliza la contraseña correcta.
