Llega el momento de trabajar con animaciones y transiciones. Estas son de gran utilidad a la hora de crear movimientos y cambios en nuestros botones, contenedores u otros elementos…

## ¿Qué es una transición y una animación?

Una transición ocurre cuando un elemento pasa de un estado a otro a partir de un evento, como puede ser un :hover en un elemento del menú de navegación. Teniendo entonces 2 estados, un estado inicial y un estado final. En cambio, una animación puede tener un número ilimitado de estados.

### Transiciones

Al tener únicamente 2 estados no tienen tanta flexibilidad como las animaciones pero resulta más fácil trabajar con ellas. 

```css
/* Transiciones */
transition: margin-right 4s ease-in-out 1s; /* property name | duration | easing function | delay */

/* Las 4 propiedades de transición */
transition-property: margin-right; /* propiedad que queremos animar */
transition-duration: 2s; /* duracción de la transición */
transition-timing-function: linear; /* curva de movimiento de la transición */
transition-delay: 1s; /* retardo hasta que se inicia la transición */
```

Vamos a probar estas propiedades

```
<div class="box box-a"></div>
<div class="box box-b"></div>
<div class="box box-c"></div>
<div class="box box-d"></div>
```

A la hora de trabajar con CSS, tenemos que tener en cuenta que las animaciones nos dan un mayor rango de personalización, al tener ‘n’ estados y por lo tanto teniendo un mayor control.

```css
/* Animaciones */
animation: 3s ease-in 1s 2 reverse both paused slidein; /* @keyframes duration | easing-function | delay |
iteration-count | direction | fill-mode | play-state | name */

/* Las propiedades de animación */
animation-duration: 3s; /* duración de la animación*/
animation-timing-function: ease-in; /* curva de velocidad de la animación */
animation-delay: 1s; /* retraso inicio animación */
animation-iteration-count: 2 /* número de veces que se repite la animación */
animation-direction: reverse; /* animación de inicio a fin o al revés */
animation-fill-mode: both; /* si termina con los valores iniciales o finales */
animation-play-state: paused; /* si permite reiniciar la animación */
animation-name: slidein; /* nombre de la animación */
```

 

Ejemplo:

```html
<div class="box"></div>
```

 

```css
.box {
    width: 300px;
    height: 300px;
    background-color: blue;
    animation-name: ejemplo;
    animation-duration: 4s;
    animation-timing-function: linear;
    animation-delay: 2s;
    animation-iteration-count: 2;
    animation-direction: normal;
    animation-fill-mode: both;
    animation-play-state: paused;
}
  
@keyframes ejemplo {
10% {background-color: blueviolet;}
25% {background-color: violet;}
50% {background-color: yellow;}
100% {background-color: orange;}
}
```

 

Librería interesante de animaciones:

> https://daneden.github.io/animate.css/
