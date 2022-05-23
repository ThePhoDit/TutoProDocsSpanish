# Comandos

Este módulo es muy importante. Te permitirá configurar meticulosamente cada comando, individualmente.

Tendrás las siguientes propiedades para todos los comandos:

```yaml
commands:
  ping:
    permission: 0
    enabled: true
    only_channels:
      - 'ID de un canal'
      - 'ID de otro canal'
    disabled_channels:
      - 'ID de un canal'
      - 'ID de otro canal'
  warn:
    permission: 50
    enabled: true
    only_channels: []
    disabled_channels: []
```

**Permission:** nivel requerido para ejecutar el comando. Si un usuario tiene el mismo nivel o más alto en el [módulo de niveles](niveles.md), podrán ejecutar el comando. Si quieres que todo el mundo pueda utilizar el comando, ajusta el nivel con `0`. \
Por defecto el bot usa el nivel asociado a este comando. Comprueba la sección [Niveles de poder](../../comandos/niveles-de-poder.md) para más información.

**Enabled:** puede ser `true` o `false`. Si está en `false`, el comando estará desactivado. \
`True` está colocado por defecto.

**Only Channels:** lista de canales en el que el bot trabajará (solo funcionará en los canales descritos). \
Esto anula `disabled_channels`.

**Disabled Channels:** lista de canales donde los comandos no funcionarán. \
De forma predeterminada, ninguno de ellos está allí.

### Analizando el ejemplo anterior

En el ejemplo anterior hemos configurado como se comportará el comando `warn`:

* Solo los usuarios de nivel 50 o mayor pueden usarlo.
* El comando está activado, así que se puede utilizar.
* No hay restricción en ningún canal porque no hemos rellenado ninguna lista.

{% hint style="warning" %}
Recuerda que si un comando no está configurado en el módulo, se utilizarán los permisos predeterminados.
{% endhint %}
