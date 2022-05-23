# Niveles

En este módulo administrarás los permisos que tienen los usuarios sobre el bot. Estos niveles son usados como permisos para ejecutar determinados comandos y acciones que puedes tomar sobre otros usuarios.

Puedes utilizar tanto IDs de usuarios como de roles. Ten en mente que los permisos que se les den a un usuario prevalecen sobre las del rol. También hay que tener en cuenta de que las IDs deberán de estar entre comillas.

Aquí tienes un pequeño ejemplo de como sería una configuración sencilla. En este caso, puedes cambiar las IDs y niveles, o puedes añadir los niveles que quieras.

```yaml
levels:
  '459649180969730050': 150 # Owner ID
  '627156480595853322': 100 # Administrator Role
  '627241194753359931': 60  # Moderator Role
  '627241150817763380': 40  # Support Member Role
```

{% hint style="info" %}
Añadiendo comentarios (cualquier cosa escrita después del símbolo #) puedes mantener un archivo de configuración limpio y mucho más fácil de leer para todo el mundo.
{% endhint %}

