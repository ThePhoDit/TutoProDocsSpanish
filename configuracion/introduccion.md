# Introducción

Aquí encontrarás información sobre el funcionamiento del archivo de configuración y en las próximas páginas como configurarlo todo.

Antes de nada, el propietario del servidor o un administrador del mismo deberá de ejecutar el comando `tp//setup`. Si no eres un administrador y necesitas ejecutar el comando, contacta con un desarrollador en el [servidor de soporte](https://discord.gg/aUNhdFD).

Lo siguiente que tienes que tener en mente es cómo sacar el archivo YAML para trabajar en él. Para ello simplemente ejecuta el comando [export](../comandos/configuracion-1/export.md).

{% hint style="info" %}
Recomendamos la utilización de un editor de texto como Visual Studio Code o Notepad++ para poder abrir el archivo. De todas formas puedes utilizar el bloc de notas de tu PC.
{% endhint %}

Esto es lo que verás al abrir el archivo la primera vez:

{% code title="LaIDDeTuServidor.yaml" %}
```yaml
levels:
  '459649180969730050': 100 # ThePhoDit#1801 - Tu ID deberá de estar aquí. 

prefix: ';'
locale: 'en'
on_join_roles: []
local_blacklist: []
```
{% endcode %}

Estas propiedades que estás viendo, son necesarias para que el bot pueda funcionar, así que **NO LAS ELIMINES**.

Pasaremos por todos los módulos disponibles, en las próximas páginas.
