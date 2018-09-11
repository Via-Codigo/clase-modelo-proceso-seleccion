## HTML

### Elementos básicos

#### Titulares (Headings)

Son los encabezados o títulos que usaremos en nuestro documento existen del **h1** al **h6**, siendo el mas importante el **h1** y asi va bajando hasta el **h6** que es el menor importante.

```html
<h1>El título mas importante del documento</h1>
<h2>El título de un segundo nivel de importancia </h2>
...
<h6>El título menos importante</h6>
```

#### Párrafos (Paragraphs)

Cuando necesitamos escribir parrafos el texto lo colocamos dentro de la etiquetas `<p></p>`

```html
<p>Todo lo que necesitas para lograr tus objetivos ya está en ti.</p>
<p>
No vas a dominar el resto de tu vida en un día. Relájate.
Domina el día. Entonces sigue haciendo eso todos los días.
</p>
```

#### Listas

Las lista se utilizan cuando requieres mostras una secuencia de datos o elementos, pueden ser ordenadas o desordenadas.

##### Listas ordenadas

En ellas importa el orden de los elementos podrian ser los pasos para realizar un tramite.

```html
<ol>
	<li>Acudir al Banco de la Nación</li>
	<li>Pedir el concepto 1810</li>
	<li>Pagar S/ 98.50 por el pasaporte biométrico.</li>
	<li>Ingresar a www.migraciones.gob.pe</li>
	<li>Llenar el formulario </li>
	<li>Separar una cita.</li>
	<li>El pasaporte será entregado en las 14 sedes de Migraciones.
		Debe llevar su voucher y DNI, no es necesario una foto.</li>
</ol>
```

##### Listas no ordenadas

En ellas no es relevante el orden de los elementos y se pueden tener otras etiquetas incluso, como en el caso de un listado de enlaces:

```html
<ul>
	<li><a href="index.html">Inicio</a></li>
	<li><a href="servicios.html">Servicios</a></li>
	<li><a href="contacto.html">Contacto</a></li>
</ul>
```

## El elemento agrupador DIV

Se usa para agrupar otros elementos con fines de adaptar la disposición de estos al diseño de la interfaz, no aporta semántica. Se usa como elemento _comodín_. Por defecto se comporta como un elemento de tipo bloque.

```html
	<h2>Juntos como hermanos</h2>
	<div>
		<p>Juntos como hermanos <br>
		Miembros de una iglesia <br>
		Vamos caminando <br>
		Al encuentro del señor </p>

		<p>Un largo caminar <br>
		Por el desierto bajo el sol <br>
		No podemos avanzar <br>
		Sin la ayuda del señor</p>
	</div>
```

## CSS

### Propiedades de texto

Entre las propiedades para dar formato al texto tenemos:

#### Font-size

Esta propiedad sirve para indicar el tamaño que van a tener los textos dentro del documento,
pudiendo tener valores absolutos como 16px y relativos como: 1.2em o 120%.

```css
.header__title {
  font-size: 31px;
}
```

#### Text-decoration

Es la propiedad para añadir detalles decorativos al texto.

```css
.post__link {
  text-decoration: none; /* quita subrayado */
}

.post__price {
  text-decoration: line-through; /* agrega una línea horizontal
  a la mitad del texto  a modo de tachado */
}

.post__category {
  text-decoration: underline; /* subraya el texto */
}
```

### Otros

#### Content (contenido):

Contenido de la caja el cual podría tener un texto, una imagen, u otros elementos,
se le puede definir anchura con la propiedad **width** y altura con la propiedad **height**.

```css
.box {
  width: 800px; /* ancho de 800 pixeles */
  /* de preferencia es mejor no aplicar height y dejar que lo que 
	va dentro le de la altura con su propio volumen */
  height: 600px;
}
```

#### Padding (relleno):

Es la distancia del contenido de la caja hacia dentro del contenedor.

```css
.box {
  padding-right: 5px; /* distancia hacia el lado derecho. */
  padding-left: 5px; /* distancia hacia el lado izquierdo. */
  padding-top: 5px; /* distancia hacia arriba. */
  padding-botton: 5px; /* distancia hacia abajo. */
}
```

**TIP:** Si deseas ahorrar líneas de código puedes aplicar esto:

```css
.box {
  padding: 5px 10px; /* el primero es para el right y left, el segundo es para el top y bottom */
}
```

#### Margin (margen):

Es la distancia de la caja hacia afuera del contenedor.

```css
.box {
  margin-right: 5px; /* distancia hacia el lado derecho */
  margin-left: 5px; /* distancia hacia el lado izquierdo */
  margin-top: 5px; /* distancia hacia arriba */
  margin-bottom: 5px; /* distancia hacia abajo */
}
```

**TIP:** Si deseas centrar una caja horizontalmente puedes usar este pequeño truco.

```css
.box {
  width: 800px; /* aplicarle un ancho, también funciona con max-width */
  margin-left: auto; /* el valor auto para equilibrar el lado izquierdo */
  margin-right: auto; /* con el lado derecho  */
}
```

#### Border (borde):

Trazo o línea de contorno, podrías usar las propiedades:

```css
.box {
  border-style: solid; /* estilo de linea */
  border-color: black; /* color de borde */
  border-width: 10px; /* grosor del trazo */
  border-radius: 5px; /* radio del borde */
}
```

**TIP:** si deseas ahorrar escribiendo todas las declaraciones puedes usar este **shorthand**

```css
.box {
  border: solid 5px black; /* style width color */
}
```
