---
description: >-
  Las etiquetas como como comandos customizados, puedes usarlo para dar
  información.
---

# Etiquetas

Puedes elegir quién puede usar las etiquetas dentro del [módulo de comandos](../configuracion/modulos/comandos.md). Usa el mismo sintaxis `use_tags` como nombre de comando. Se vería algo así:

```yaml
use_tags:
  permission: 10
  enabled: true
  disabled_channels: []
```

Esto funciona exactamente igual a los demás comandos.

Ahora que sabes como controlar quién usa las etiquetas, veamos algunos comandos útiles:

### Obtener una lista de etiquetas:  (40)

```
;taglist
---------
;listtag
```

### Crea una etiqueta:  (100)

```
;createtag {nombre} {contenido}
---------
;addtag {nombre} {contenido}
```

### Edita una etiqueta: (100)

```
;changetag {nombre/id} {nuevo contenido}
---------
;edittag {nombre/id} {nuevo contenido}
```

### Borra una etiqueta:  (100)

```
;deletetag {nombre/id}
---------
;deltag {nombre/id}
```

### Obtener información sobre una etiqueta:   (40)

```
;infotag {nombre/id}
---------
;taginfo {nombre/id}
```
