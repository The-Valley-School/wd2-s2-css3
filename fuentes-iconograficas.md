A la hora de trabajar sobre un proyecto web, se dará el caso en el que tengamos que trabajar con multitud de iconos, llegado el punto tenemos que intentar evitar usarlos como si fueran imágenes y trabajar con fuentes iconográficas.

A partir de ahí tenemos varias opciones:

### UTILIZAR FUENTES ICONOGRÁFICAS EXISTENTES

Existen infinidad de fuentes iconográficas gratuitas que podemos usar, a nosotros nos gusta especialmente **fontawesome**

> https://fontawesome.com/

Al registrarnos, podemos acceder a una fuente iconográfica gratuita que nos proporciona infinidad de iconos a usar. Basta con incluir dentro de nuestro proyecto el siguiente script:

```html
<script src="https://kit.fontawesome.com/7109d51c44.js" crossorigin="anonymous"></script>
```

A partir de aquí, podremos buscar el icono que queramos en la web e introducirlo en nuestro proyecto:

```html
<i class="fa-solid fa-house"></i>

<!-- A nosotros nos gusta más trabajar con span -->
<span class="fa-solid fa-house"></span>
```

### UTILIZAR FUENTES ICONOGRÁFICAS PROPIAS

Para proyectos propios está muy bien utilizar **fontawesome**, pero por lo general, el equipo de diseño nos proporcionará los iconos propios asociados a la imagen de marca del proyecto con los cuales tendremos que trabajar, para ello crearemos nuestras fuentes iconográficas propias.

Para ello, al no tener equipo de diseño en este video, usaremos un repositorio de iconos svg.

> https://www.svgrepo.com/

Tras descargar la selección que queramos usaremos icomoon para crear nuestra propia fuente:

> https://icomoon.io/app

Para utilizarlas bastará con copiar y pegar la clase :)