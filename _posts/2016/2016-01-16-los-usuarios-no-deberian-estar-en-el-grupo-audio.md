---
layout: post
title: "Los usuarios no deberían estar en el grupo 'audio'"
date: '2016-01-16 11:34'
---

Mi novia y yo compartimos computadora (aka _PC_, _ordenador_), y de un tiempo a la fecha algo andaba mal con el sonido.

Detalles técnicos aparte, el origen del problema era una política del sistema y pulseaudio. Tal política ocasionaba el bloqueo de la tarjeta de sonido, de forma que sólo un usuario podía reproducir (o grabar) sonido a la vez.

Si te pasa que sólo un usuario puede reproducir sonido en **GNU/Linux**, esta podría ser la solución:

# Revisa la lista de usuarios que están en el grupo `audio`:

```
mautematico@flex:~$ fgrep -ie 'audio' /etc/group
audio:x:29:pulse,mautematico,mariana
```

En mi caso, había tres usuarios: `mautematico`, `mariana` y `pulse`. Los usuarios regulares no deberían estar en el grupo `audio`.

# Quita los usuarios regulares del grupo `audio`:

```
root@flex:~# deluser mautematico audio
root@flex:~# deluser mariana audio
```

# Ahora sólo debería estar `pulse` en el grupo `audio`:

```
root@flex:~# fgrep -ie 'audio' /etc/group
audio:x:29:pulse
```

# Reinicia:

```
root@flex:~# reboot
```

# Y prueba.
¡Suerte!
