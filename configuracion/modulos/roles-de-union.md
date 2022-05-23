# Roles de unión

Puedes asignar roles a los miembros recién unidos al servidor. Sigue este ejemplo para hacerlo:

```yaml
on_join_roles: ['630576778271784964', 'Otra ID de un rol']
```

Otra manera de hacerlo es de esta manera:

```yaml
on_join_roles:
  - '630576778271784964'
  - 'Otra ID de un rol'
```

Puedes añadir los roles que quieras.

{% hint style="info" %}
Como puedes ver, hay dos maneras de configurar una lista. Personalmente preferimos la segunda manera porque es mucho más limpia.&#x20;
{% endhint %}

{% hint style="info" %}
En las próximas páginas de la guía podrás utilizar una de las dos maneras de hacerlo, pero nosotros lo escribiremos solo de la segunda forma.
{% endhint %}
