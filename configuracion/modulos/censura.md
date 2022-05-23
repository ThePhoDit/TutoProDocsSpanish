# Censura

El módulo de censura permite controlar si un usuario hace cualquier tipo de spam o usa una palabra prohibida. Miraremos cada propiedad después de ver un ejemplo, como de costumbre:

Cuando alguien activa este módulo, su mensaje será borrado y lo enviará en el canal de registros de la etiqueta `CENSOR`.

```yaml
censor:
  whitelist_level: 40

  filter_invites: true
  invites_codes_whitelist:
    - 'minecraft'
    - 'aUNhdFD'
  invites_guilds_whitelist:
    - 'Guild ID 1'
  invites_channels_whitelist: []
  invites_roles_whitelist: []
  invites_users_whitelist: []
  invites_categories_whitelist: []

  filter_links: true
  links_domains_whitelist:
    - 'google.com'
    - 'twitch.tv'
  links_channels_whitelist:
    - 'Channel ID 1'
    - 'Channel ID 2'
  links_roles_whitelist: []
  links_users_whitelist: []
  links_categories_whitelist: []

  filter_tokens: true
  tokens_blacklist:
    - 'Token 1'
    - 'Token 2'
  tokens_channels_whitelist:
    - 'Channel ID 1'
    - 'Channel ID 2'
    - 'Channel ID 3'
  tokens_roles_whitelist: []
  tokens_users_whitelist: []
  tokens_categories_whitelist: []

  filter_words: true
  words_blacklist:
    - 'Word 1'
    - 'Word 2'
  words_channels_whitelist: []
  words_roles_whitelist: []
  words_users_whitelist: []
  words_categories_whitelist: []
```

**Level Whitelist:** aquí configurarás el nivel a partir el cual no le afectará este módulo. Si el usuario tiene el [nivel](niveles.md) 50 y la censura está configurada al 40, el usuario no activara el filtro. El filtro solo se activará si el usuario tiene el mismo nivel o menor.

{% tabs %}
{% tab title="Invites" %}
**Filter Invites:** censura las invitaciones de Discord `true` o no `false` .

**Invites Codes Whitelist:** lista de invitaciones específicas que no se borrarán. Asegurate de colocar la código de invitación.

**Invites Guilds Whitelist:** lista de servidores a los cuales ninguna invitación será borrada, eso significa que si X servidor está en la lista, ninguna nueva invitación será censurada.

**Invites Channels Whitelist:** lista de canales donde el módulo está desactivado. Todas las invitaciones son permitidas.

**Invites Roles Whitelist:** lista de roles que serán ignorados.

**Invites Users Whitelist:** lista de usuarios que serán ignorados.

**Invites Categories Whitelist:** categorías que serán ignoradas.
{% endtab %}

{% tab title="Links" %}
**Filter Links:**  si está en `true` censurará todos los enlaces menos las invitaciones. En `false` no estará activado.

**Links Domains Whitelist:** lista de dominios que TutoPro ignorará.

**Links Channels Whitelist:** lista de canales que el bot ignorará y no censurará.

**Links Roles Whitelist:** lista de roles que el bot no censurará.

**Links Users Whitelist:** lista de usuario que el bot no censurará.

**Links Categories Whitelist:** lista de categorías en los que el bot no censurará.
{% endtab %}

{% tab title="Words" %}
**Filter Words:** si está en `true` las palabras de la lista serán censuradas. En `false` no.

**Words Blacklist:** lista de palabras que el bot censurará.

**Words Channels Whitelist:** lista de canales que el bot ignorará y no censurará.

**Words Roles Whitelist:** lista de roles que el bot no censurará.

**Words Users Whitelist:** lista de usuario que el bot no censurará.

**Words Categories Whitelist:** lista de categorías en los que el bot no censurará.
{% endtab %}

{% tab title="Tokens" %}
**Filter Tokens:** si está en `true` las palabras claves de la lista serán censuradas. En `false` no.

**Tokens Blacklist:** lista de palabras clave que el bot censurará.

**Tokens Channels Whitelist:** lista de canales que el bot ignorará y no censurará.

**Tokens Roles Whitelist:** lista de roles que el bot no censurará.

**Tokens Users Whitelist:** lista de usuario que el bot no censurará.

**Tokens Categories Whitelist:** lista de categorías en los que el bot no censurará.
{% endtab %}
{% endtabs %}

{% hint style="info" %}
## ¿Cuál es la diferencia entre palabras y palabras clave?

Si es tu primera vez un bot como este, entendemos tu confusión y por eso te vamos a ayudar.

### Palabras

Las palabras siempre están **separadas por un espacio** entre sus lados. Si `Hola` estuviera en la lista:

Hola soy Aris -> Esto sería borrado.

Hola**,** soy Aris -> Esto no sería borrado.

### Palabras clave

Las palabras clave pueden están juntas en una palabra. Si `Hola` estuviera en la lista:

Hola soy Aris -> Esto sería borrado.

Hola, soy Aris -> Esto sería borrado.

Me gusta decircosasenunamismapalabra**Hola**lol -> Esto sería borrado.
{% endhint %}

{% hint style="warning" %}
Recuerde que las palabras y las palabras clave no distinguen entre mayúsculas y minúsculas.&#x20;
{% endhint %}
