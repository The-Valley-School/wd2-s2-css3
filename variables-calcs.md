## CUSTOM PROPERTIES

Podemos entender las custom properties como una especie de variables en CSS que nos van a permitir utilizar ese valor específico a lo largo del documento css (un color, una medida…).

La sintaxis es la siguiente:

 

```css
/* declaración */

elemento {
	--custom-property: green;
}

/* uso */

elemento {
	color: var(--custom-property);
}
```

  

Ejemplo:

 

```html
<div class="contenedor-a">
  <h1 class="titulo">Primer título </h1>
	<h1 class="titulo segundo">Segundo título </h1>
</div>
<div class="contenedor-b">
	<h1 class="titulo ">Tercer título </h1>
<div>
```

 

```css
.contenedor-a{
	--font-color: green;
}

.segundo{
	--font-color: yellow;
}

.titulo{
	color: var(--font-color,red);
}
```

  

## CÁLCULOS

En CSS tenemos la función calc() que nos permite realizar cálculos para determinar ciertos valores sobre propiedades CSS, por ejemplo tamaños, paddings, margins…

Esta función únicamente admite un parámetro, teniendo como resultado también un único valor.

Acepta los operadores: **suma (+), resta (-), división (/) y multiplicación (*)**

 

```css
.elemento {
    width: calc(100% - 200px);
}
```

 