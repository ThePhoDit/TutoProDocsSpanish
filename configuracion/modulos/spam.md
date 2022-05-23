# Spam



El módulo de spam mantiene alejado a los usuarios que intentan "inundar" el chat con mensajes de spam. Puede filtrar por una cantidad de mensajes, una cantidad de mensajes duplicados o por la cantidad de líneas en un mensaje

Aquí tienes un ejemplo de cómo está configurado:

```yaml
spam:
  enabled: true
  level_whitelist: 40
  delete_messages: true
  tempmute_duration: 900
  channels_whitelist: []
  roles_whitelist: []
  users_whitelist: []
  categories_whitelist: []
  only_channels: []
  maximum_messages:
    enabled: true
    amount: 10
    interval: 5
    channels_whitelist: []
    roles_whitelist: []
    users_whitelist: []
    categories_whitelist: []
    only_channels: []
  duplicated_messages:
    enabled: true
    amount: 5
    interval: 5
    channels_whitelist: []
    roles_whitelist: []
    users_whitelist: []
    categories_whitelist: []
    only_channels: []
  maximum_lines:
    enabled: true
    amount: 5
    channels_whitelist: []
    roles_whitelist: []
    users_whitelist: []
    categories_whitelist: []
    only_channels: []
```

**Enabled:** si este módulo está encendido o apagado.

**Level Whitelist:** nivel que alguien necesita para ser ignorado. Cualquiera con un nivel superior no activará el filtro.

**Delete Messages:** si el bot borra los mensajes o no.

**Tempmute Duration:** tiempo en segundos del silencio aplicado. Ponle en 0 para deshabilitarlo.

**Roles Whitelist:** lista de roles ignorados generalmente.

**Channels Whitelist:** lista de canales ignorados generalmente.

**Users Whitelist:** lista de usuarios ignorados generalmente.

**Categories Whitelist:** lista de categorías ignoradas generalmente.

**Only Channels:** lista de únicos canales donde el módulo funcionará.

{% tabs %}
{% tab title="Maximum Messages" %}
**Enabled:** si esta sección está encendida o apagada.

**Amount:** cantidad de mensajes que activa el filtro.

**Interval:** tiempo en segundos para enviar la cantidad selecionada de mensajes.

**Roles Whitelist:** lista de roles ignorados.

**Channels Whitelist:** lista de canales ignorados.

**Users Whitelist:** lista de usuarios ignorados.

**Categories Whitelist:** lista de categorías ignoradas.

**Only Channels:** lista de únicos canales donde el módulo funcionará.
{% endtab %}

{% tab title="Duplicated Messages" %}
**Enabled:** si esta sección está encendida o apagada.

**Amount:** cantidad de mensajes duplicados que activa el filtro.

**Interval:** tiempo en segundos para enviar la cantidad selecionada de mensajes duplicados.

**Roles Whitelist:** lista de roles ignorados.

**Channels Whitelist:** lista de canales ignorados.

**Users Whitelist:** lista de usuarios ignorados.

**Categories Whitelist:** lista de categorías ignoradas.

**Only Channels:** lista de únicos canales donde el módulo funcionará.
{% endtab %}

{% tab title=" Maximum Lines" %}
**Enabled:** si esta sección está encendida o apagada.

**Amount:** cantidad de lineas en un mensaje que activa el filtro.

**Roles Whitelist:** lista de roles ignorados.

**Channels Whitelist:** lista de canales ignorados.

**Users Whitelist:** lista de usuarios ignorados.

**Categories Whitelist:** lista de categorías ignoradas.

**Only Channels:** lista de únicos canales donde el módulo funcionará.
{% endtab %}
{% endtabs %}

