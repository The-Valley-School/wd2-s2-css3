 Vamos ahora a dar un repaso global a las unidades de medida que podemos utilizar a la hora de desarrollar nuestras páginas web.

Se agrupan en dos conjuntos:

- Unidades de longitud absoluta.
- Unidades de longitud relativa.

## **UNIDADES DE LONGITUD ABSOLUTA**

Unidades de medida no relativas a nada y que siempre tendrán el mismo tamaño:

| Unidad | Nombre | Equivale a |
| --- | --- | --- |
| cm | Centímetros | 1cm = 96px/2,54 |
| mm | Milímetros | 1mm = 1/10 de 1cm |
| Q | Cuartos de milímetros | 1Q = 1/40 de 1cm |
| in | Pulgadas | 1in = 2,54cm = 96px |
| pc | Picas | 1pc = 1/6 de 1in |
| pt | Puntos | 1pt = 1/72 de 1in |
| px |. Píxeles | 1px = 1/96 de 1in |

Casi siempre, estos valores los usaremos para trabajar temas de formato de impresión más allá del tema de pantalla.

El único del listado que usaremos a menudo es el pixel. Existen dos vertientes a cerca del píxel ya que algunos hablan de que se trata de una unidad relativa ya que depende de la resolución de pantalla del monitor.

## UNIDADES DE LONGITUD RELATIVA

El valor de estas unidades siempre estará referenciado por otro valor. Nos son de gran ayuda a la hora de trabajar con diferentes tamaños de pantalla.

| em | Tamaño de letra del elemento padre, en el caso de propiedades tipográficas como font-size, y tamaño de la fuente del propio elemento en el caso de otras propiedades, como width, padding, etc. |
| --- | --- |
| ex | Altura x de la fuente del elemento. |
| ch | La medida de avance (ancho) del glifo "0" de la letra del elemento. |
| rem | Tamaño de la letra del elemento raíz. |
| lh | Altura de la línea del elemento. |
| vw | 1% del ancho de la ventana gráfica. |
| vh | 1% de la altura de la ventana gráfica. |
| vmin | 1% de la dimensión más pequeña de la ventana gráfica. |
| vmax | 1% de la dimensión más grande de la ventana gráfica. |

### em

Tamaño relativo al tamaño de letra del elemento. Por ejemplo, si queremos que un título tenga un padding relativo al tamaño de letra quedaría de esta forma:

 

```html
<h1 class="title title-a">Título</h1>
<h1 class="title title-b">Título</h1>
```

  

```css
.title{
	display: inline-block;
	padding: 0.5em;
	background-color: lightcoral;
}

.title-a{
	font-size: 100px;
}

.title-b{
	font-size: 30px;
}
```

 

A lo largo del proyecto, podemos mezclar este tipo de unidades con píxeles, por ejemplo:

```css
body { 
	font-size: 10px; 
}

h1 { 
	font-size: 3em; 
}
```

### ex

Relativa a la altura de la letra **x minúscula.** Idéntico al funcionamiento de la medida **em.**

  

```css
.title{
	display: inline-block;
	padding: 1ex;
	background-color: lightcoral;
}
```

  

### vh y vw

Son medidas relativas al viewport.
