# Salidas

El módulo de salidas funciona de la misma manera que el de bienvenidas, pero se activa cuando alguien abandona el servidor.

```yaml
leaves:
  enabled: true
  channels:
    - id: 'Channel ID 1'
      message: |-
        See you {{member}}, welcome to {{server}}
```

**Enabled:** define si el módulo está o no encendido.

**Channels:** esta es la lista de canales y mensajes. Cada uno está formado de la siguiente manera:

* **ID:** La ID del canal donde el mensaje se enviará.
* **Message:** el mensaje. Hay variables que puedes usar:
  * **\{{member\}}** - Menciona al usuario que abandonó.
  * **\{{memberTag\}}** - Menciona el tag del usuario que abandonó, así como: TutoPro#4702
  * **\{{memberCount\}}** - Muestra la cantidad de miembros que hay en el servidor.
  * **\{{server\}}** - Muestra el nombre del servidor.
* **Embed:** define si quieres usar un mensaje embed o no.
* **Random:** lista de mensajes que TutoPro elegirá al azar para enviarlo.
