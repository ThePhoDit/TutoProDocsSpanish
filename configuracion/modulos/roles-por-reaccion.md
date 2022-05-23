# Roles por reacción

Haz que los usuarios seleccionen qué roles quieren tener.

```yaml
reaction_roles:
  - message: 'Message ID'
    emoji: '👺' # For default emojis.
    roles:
      - id: 'Role ID 1'
        type: 'ADD'
      - id: 'Role ID 2'
        type: 'REMOVE'
  - message: 'Message ID'
    emoji: 'tester:714804405806956685' # For custom emojis (name:id)
    roles:
      - id: 'Role ID 3'
```

La configuración de los roles por reacción es una lista con los diferentes objetos que quieres. Cada objeto corresponde a un mensaje y un emoji:

**Message:** la ID del mensaje donde estará el rol de reacción.

**Emoji:** el emoji al que los usuarios tienen que reaccionar. Pega el emoji Unicode si es uno predeterminado o usa el nombre de formato `nombre:id` para los personalizados.

**Roles:** lista de roles que serán añadidos o eliminados al reaccionar:

* **ID:** la ID del rol.
* **Type:** `ADD` (añade) o `REMOVE` (elimina). Por defecto está en `ADD`.

{% hint style="info" %}
Recuerda que tienes que añadir manualmente la reacción al mensaje.
{% endhint %}
