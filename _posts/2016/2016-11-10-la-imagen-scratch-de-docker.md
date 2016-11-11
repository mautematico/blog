---
layout: "post"
title: "La imagen \"scratch\" de docker"
date: "2016-11-10 17:25"
---

Hay una imagen mínima _reservada_ en Docker, de nombre scratch. Si quieres, puedes utilizar esta imagen mínima para crear tu propia imagen.

Pero hay una particularidad interesante respecto a scratch: No puedes descargarla vía pull, tampoco ejecutarla, y de hecho no puedes etiquetar ninguna imagen con el nombre scratch.

Lo que sí puedes es hacer referencia a scratch en tu Dockerfile. Por ejemplo, puedes crear una imagen mínima utilizando scratch de esta forma:

```
FROM scratch
ADD hello /
CMD ["/hello"]
```

Para los curiosos, esto resultaría en la imagen `hello-world` usada en los tutoriales de docker.

https://docs.docker.com/engine/userguide/eng-image/baseimages/#/creating-a-simple-base-image-using-scratch
