# Infracciones

Aquí podrás configurar la parte moderativa del bot. Vamos a ver un ejemplo primero y para que sirve cada cosa.

```yaml
infractions:
  mute_role: 'ID del rol de Silencio'
  notify:
    - 'WARN'
    - 'MUTE'
    - 'TEMPMUTE'
    - 'UNMUTE'
    - 'KICK'
    - 'BAN'
    - 'TEMPBAN'
    - 'UNBAN'
  show_moderator: false
  delete_command: true
  messages:
    warn: |-
      You have been warned by {{moderator}} in {{server}} with the reason:
      {{reason}}.
    ban: |-
      You have been baned.
```

**Mute Role:** este es el rol que dará a los usuarios que serán silenciados por un moderador o el filtro de spam.

**Notify:** todas las acciones de esta lista será notificadas al usuario al momento de ser efectuadas. Si no quieres se notifiquen, simplemente elimina cualquier acción que no desees de aquí.

**Show Moderator:** mostrará `true` o no `false` los moderadores que efectuará la acción. \
Esto lo podrá anular un comando que veremos en la sección de moderación.&#x20;

**Delete Command:** eliminará `true` o no `false` el comando de infracción que ejecutarás sobre el usuario. (solo en comandos en infracción)

**Messages:** permite colocar un mensaje deseado para el envío de notificación de la sanción por MD. Puedes añadir uno para cada comando.
