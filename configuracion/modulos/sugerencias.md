# Sugerencias

Las sugerencias son una parte esencial de TutoPro. Ellas permiten a los usuarios de la comunidad hacer saber a los administradores que les gustaría ver en sus servidores.

Veamos como se configura este módulo:

```yaml
suggestions:
  reviewing_channel: 'Channel ID 1'
  voting_channel: 'Channel ID 2'
  approved_channel: 'Channel ID 3'
  potential_channel: 'Channel ID 4'
  denied_channel: 'Channel ID 5'
```

**Reviewing Channel:** si esta propiedad tiene una id del canal, todas las nuevas sugerencias serán enviadas allí. La idea de la función es que el canal que se coloca aquí solo lo puedan ver los moderadores antes, para [revisar](sugerencias.md) el contenido.

**Voting Channel:** esta propiedad es necesaria para esto funcione. Las sugerencias son enviadas aquí si o son revisados o si `Reviewing Channel` no está configurado. Los usuarios pueden votar aquí.

**Approved Channel:** canal donde se envian las sugerencias [aprobadas](sugerencias.md). Si no está configurado, se editará la sugerencia en el canal de votación.

**Potential Channel:** canal donde se envian las sugerencias [potenciales](sugerencias.md). Si no está configurado, se editará la sugerencia en el canal de votación.

**Denied Channel:** canal donde se envian las sugerencias [denegadas](sugerencias.md). Si no está configurado, se editará la sugerencia en el canal de votación.
