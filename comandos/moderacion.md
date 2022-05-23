---
description: >-
  Aquí encontrarás todos los comandos de moderación que puedes usar con TutoPro.
  Si un comando tiene un alias, se mostrarán todas las formas de usarlo.
---

# Moderación

### Buscar infracciones de un usuario específico: (60)

```
;infractions {usuario}
---------
;infrs {usuario}
```

### Cambiar el motivo de una infracción: (60)

```
;reason {ID de infración} {nueva razón}
```

### Cambiar la duración de una infracción: (60)

```
;duration {ID de infración} {nueva duración}
```

### Eliminar una infracción: (60)

```
;delete {ID de infración}
```

> Solo funciona en infracciones temporales.&#x20;

### Advertir a alguien: (60)

```
;warn {usuario} [razón]
```

### Silenciar a alguien: (60)

```
;mute {usuario} [razón]
```

> El rol de silencio es requerido en el [módulo de infracción](../configuracion/modulos/infracciones.md).

### Silenciar temporalmente a alguien: (60)

```
;tempmute {usuario} {duración} [razón]
```

> El rol de silencio es requerido en el [módulo de infracción](../configuracion/modulos/infracciones.md).

### Quitar silencio a alguien: (60)

```
;unmute {usuario} [razón]
```

> El rol de silencio es requerido en el [módulo de infracción](../configuracion/modulos/infracciones.md).

### Expulsa a alguien del servidor: (60)

```
;kick {usuario} [razón]
```

### Veta a alguien del servidor: (60)

```
;ban {usuario} [razón]
```

### Veta temporalmente a alguien del servidor: (60)

```
;tempban {usuario} {duración} [razón]
```

### Quita el veto a alguien ya vetado: (60)

```
;unban {usuario} [razón]
```

### Borra mensajes: (60)

```
;clean {cantidad}
or
;clean {usuario} {cantidad}
```

### Veta varios usuarios: (60)

```
;mban {usuarios} [-r] [razón]
```

> Las IDs de los usuarios deben ser separados por un espacio. La etiqueta -r significa que la razón empieza desde allí.

### Expulsa a alguien del canal de voz: (60)

```
;voicekick {usuario}
```

### Obtén la lista de roles del servidor: (60)

```
;roles
```

### Cambiar el tiempo del modo lento del canal actual: (40)

```
;slowmode {tiempo en segundos}
```

### Bloquea un canal: (60)

```
;lock [roles]
```

> Los roles deben estar separados por un espacio. Si no se define, se usará everyone.

### Desbloquea un canal: (60)

```
;unlock [roles]
```

> Los roles deben estar separados por un espacio. Si no se define, se usará everyone.

{% hint style="info" %}
#### Mostrando el moderador&#x20;

Las notificaciones de infracciones mostrarán al moderador cuando notifique a un usuario según esté configurado en la [configuración de infracciones](../configuracion/modulos/infracciones.md).

Esto se puede anular introduciendo una palabra clave entre el usuario/duración y el motivo al ejecutar el comando. Las palabras clave disponibles son:

**DM** - Mostrará siempre quién dió la infracción.

Ejemplo: `;warn {usuario} DM [razón]`

**ADM** - No mostrará quién dió la infracción.

Example: `;warn {usuario} ADM [razón]`
{% endhint %}
