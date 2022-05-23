# Bienvenidas

Puedes crear tus propios mensajes para los nuevos usuarios que se unen a tu servidor.

```yaml
joins:
  enabled: true
  channels:
    - id: 'Channel ID 1'
      message: |-
        Hello {{member}}, welcome to {{server}}
      embed: true
      random:
        - 'Message 1'
        - 'Message 2'
      image: 'Image Link'
    - id: 'Channel ID 2'
      message: |-
        Hello {{member}}, welcome to my Server.
```

**Enabled:** define si el módulo está o no encendido.

**Channels:** esta es la lista de canales y mensajes. Cada uno está formado de la siguiente manera:

* **ID:** La ID del canal donde el mensaje se enviará.
* **Message:** el mensaje. Hay variables que puedes usar:
  * **\{{member\}}** - Menciona al nuevo usuario.
  * **\{{memberTag\}}** - Menciona el tag del nuevo usuario, así como: TutoPro#4702
  * **\{{memberCount\}}** - Muestra la cantidad de miembros que hay en el servidor.
  * **\{{server\}}** - Muestra el nombre del servidor.
* **Embed:** define si quieres usar un mensaje embed o no.
* **Random:** lista de mensajes que TutoPro elegirá al azar para enviarlo.
* **Image:** un enlace de una imagen o gif que se enviará junto al mensaje de bienvenida.

{% hint style="info" %}
Puedes añadir los canales que gustes.
{% endhint %}
