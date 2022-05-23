---
description: Keep those raiders away!
---

# Antiraid

Este módulo le ayudará a mantener su servidor seguro. Si este módulo está habilitado, expulsará a los usuarios que lo activaron.

```yaml
antiraid:
  new_users_amount: 50
  interval: 10 # Seconds
```

Veamos para qué sirve cada propiedad:

**New Users Amount:** cantidad de usuarios que tienen que entrar en el intervalo seleccionado.

**Interval:** segundos en los que la cantidad especificada de usuarios debe unirse.

{% hint style="danger" %}
Este módulo no está probado oficialmente porque no podemos recrear un raid. Informa sobre cualquier error que encuentras.
{% endhint %}
