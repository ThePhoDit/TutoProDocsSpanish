# Registros

Este módulo permite hacer un registro de todo lo que está pasando en el servidor. \
Como siempre tienes un ejemplo aquí:

```yaml
logs:
  timezone: 'Europe/Madrid'
  ignored_roles: []
  ignored_channels: []
  ignored_users: []
  channels:
    - id: 'ID del canal'
      enabled: true
      include:
        - 'WARN'
        - 'KICK'
        - 'BAN_ADD'
        - 'TEMPBAN_ADD'
        - 'BAN_RMV'
        - 'MUTE_ADD'
        - 'MUTE_RMV'
        - 'TEMPMUTE_ADD'
        - 'GUILD_MEMBER_ADD'
        - 'GUILD_MEMBER_RMV'
        - 'VOICE_JOIN'
        - 'VOICE_MOVE'
        - 'VOICE_LEAVE'
        - 'MESSAGE_EDIT'
        - 'MESSAGE_DELETE'
        - 'CENSOR'
        - 'COMMAND_USED'
        - 'SPAM'
        - 'CHANNEL_CREATE'
        - 'CHANNEL_UPDATE'
        - 'CHANNEL_DELETE'
```

**Timezone:** región que el bot utilizará para colocar bien el tiempo. Puedes ver las zonas horarias [aquí](https://timezonedb.com/time-zones). \
( usa el nombre de la columna _Time Zone_ )

**Ignored Roles:** lista de las IDs de roles que no serán registradas. \
Si un usuario tiene un rol que está en la lista, el bot no registrará nada suyo.

**Ignored Channels:** lista de IDs de canales que no se registrarán.

**Ignored Users:** lista de IDs de usuarios en las que sus acciones no serán registradas.

**Channels:** recuerda que puedes añadir los que quieras.

* **ID:** ID del canal en las que se enviarán los registros.
* **Enabled:** `true` hará que los registros estén activos (registre) , mientras que `false` los desactivará (no registrará nada). Por defecto está en `false`.
* **Include:** lista de acciones que serán enviados a dicho canal. Los nombres describen lo que registra cada uno.

