![LarnU](../_src/assets/00-PrimerosPasos/logo_LarnU.png)

## Etiquetas de Formularios

HTML5 proporciona una serie de etiquetas interesantes para utilizar en formularios (además de las ya existentes en versiones anteriores). Los formularios son una forma sencilla de establecer mecanismos para que el usuario pueda introducir información en una página web de forma sencilla e intuitiva, y el sitio web sea capaz de procesarla correctamente y añadirla en una base de datos de la página, enviarla por email o procesarla para mostrar información final al usuario.

Nuestros objetivos al crear un formulario HTML5 deben ser los siguientes:

- Hacer lo más sencillo posible el proceso de inserción de datos por parte del usuario.
- Intentar que la experiencia de usuario sea lo más agradable posible.
- Intentar que los datos introducidos estén en un formato predecible y esperado.
- Reducir los errores al introducir datos en la medida de lo posible.
- Comunicar claramente si ocurren errores al introducir datos.

### Contenedor de formulario 

Para comenzar con la creación de un formulario, el primer paso es indicar una etiqueta contenedora \<form>, que incluirá toda la información que se quiere recoger en ese formulario:

```
<form></form>
```

De esta forma, se puede incluso crear varias etiquetas `<form>` por página, pudiendo así crear varios formularios diferentes, como por ejemplo, uno para realizar una búsqueda en la página, otro para dejar un comentario y otro para enviar un email al autor.

La etiqueta `<form>` dispone de varios atributos para utilizar:

- `action`	-> URL	-> Dirección URL del back-end donde se enviará la información del formulario.
- `method`	-> get | post	-> Método HTTP de envío. GET a través de URL, POST para envío extenso.
- `name`	-> nombre	-> Nombre del formulario. Útil para procesar posteriormente.
- `target`	-> destino	-> Nombre del lugar donde se abrirá el formulario. \\_blank para nueva pestaña.
- `enctype`	-> tipo	-> Codificación para el envío del formulario. Importante para envío de archivos.
- `accept-charset`	-> codificación	-> Fuerza a utilizar una codificación en los parámetros de texto del formulario.
- `autocomplete`	-> on | off	-> Activa o desactiva el autocompletado para todos los campos del formulario.
- `novalidate`	-> Boolean ->	Con este atributo presente, el formulario obvia la validación HTML5.

### Campos de entrada 

Una de las etiquetas que más utilizaremos para obtener información a modo de campo de entrada de datos en un formulario es la etiqueta \<input>. Su funcionalidad más utilizada es la de servir como campo de texto:

### La etiqueta "input"

La etiqueta `<input>` tiene una gran cantidad de atributos (algunos dependiendo del valor de type, que mostraremos más adelante). Estos son los atributos que podemos utilizar de forma general para prácticamente cualquier campo de entrada de datos con la etiqueta `<input>`:

- `type`	-> tipo de campo	-> Indica el tipo de campo del que se trata.
- `name`	-> nombre del campo	-> Indica el nombre del campo para hacer referencia más tarde.
- `value`	-> valor por defecto	-> Indica el valor inicial que tendrá ese campo de datos.
- `form` -> nombre del formulario	-> Asocia este campo de datos con un formulario específico.
- `placeholder`	-> sugerencia	-> Indica una sugerencia al usuario antes de escribir.
- `size`	-> número	-> Tamaño visual (número de carácteres) del campo de datos.
- `autocomplete`	-> on | off	-> Activa o desactiva el autocompletado para este campo.
- `autofocus`	->	Establece el foco (coloca el cursor) en este campo al cargar la página.

El atributo type nos permitirá indicar que tipo de campo de dato mostrará en el navegador (text, number, date... los veremos más adelante). Mediante el atributo name le daremos un nombre al campo de texto, así cuando enviemos la información del formulario, podremos manejarla desde javascript o desde el back-end haciendo referencia a dicho nombre.

### Campos de texto

La etiqueta HTML `<input>` puede tomar varios valores diferentes en su atributo type para permitir al usuario introducir información de texto, además de otra etiqueta denominada `<textarea>` para cantidades de texto más grandes como varios párrafos.

Según nuestras necesidades, tendremos varias opciones:

- Texto alfanumérico libre (texto corto)	-> `<input type="text">`	-> <input type="text">
- Texto para búsquedas	-> `<input type="search">`	-> <input type="search">
- Número de teléfono o móvil	-> `<input type="tel">`	-> <input type="tel">
- Dirección URL	-> `<input type="url">` -> <input type="url">	
- Dirección de correo email	-> `<input type="email">`	-> <input type="email">
manz@emezeta.com
- Clave o contraseña	-> `<input type="password">`	-> <input type="password">
- Campo oculto (no mostrar al usuario) ->	`<input type="hidden">`	
- Texto alfanumérico libre (extenso)	-> `<textarea>`	-> <textarea>	</textarea>

### Campos numéricos

La primera de ellas es number, un tipo con el que podremos utilizar un campo de texto donde el usuario sólo puede escribir números (o carácteres como +, - o el número e, entre otros). La diferencia respecto a otros campos es que al mover el ratón sobre él, nos aparecen dos flechas que nos permiten aumentar o disminuir la cantidad numérica del campo.

- Número o cantidad numérica	-> `<input type="number">`	-> <input type="number">
- Rango numérico	-> `<input type="range">`	-> <input type="range">

Por otro lado, tenemos la etiqueta `<input type="range">`, que en lugar de mostrarnos un campo de texto que podemos modificar introduciendo directamente el número, podemos hacerlo mediante un «slider» o barra de desplazamiento que representa un número entre un rango numérico específico.


### Campos de fecha y hora

En HTML5.1, además, se incluyeron nuevos campos que también permiten obtener fecha y hora (en un mismo campo), un mes específico o el número de semana del año, este último algo que se utiliza bastante en EEUU, aunque no demasiado en España.

- Fecha	-> `<input type="date">`	-> <input type="date">	
- Hora	-> `<input type="time">`	-> <input type="time">	
- Fecha y hora local	-> `<input type="datetime-local">`	-> <input type="datetime-local">	
- Mes	-> `<input type="month">`	-> <input type="month">	
- Semana	-> `<input type="week">`	-> <input type="week">	

### Campos de casillas y botones

Si queremos definir opciones que el usuario debe elegir o escoger, en muchos casos lo más apropiado suele ser utilizar casillas de verificación o botones de opción (botones de radio). La diferencia principal entre estos dos tipos de botones es la siguiente:

Las casillas de verificación se marcan para establecer una opción como activada (verdadero). Los botones de radio se marcan para elegir sólo una opción de varias posibles.

- Casilla de verificación (activado o desactivado)	-> `<input type="checkbox">` -> <input type="checkbox">	 
- Botón radio (casilla de opción única)	-> `<input type="radio">` -> <input type="radio">

### Casillas de verificación

Las casillas de verificación permiten mostrar al usuario la posibilidad de marcar una opción como activada, verdadera o afirmativa, o dejarla sin marcar, lo que representa una opción desactivada, falsa o negativa.

Se puede añadir el atributo checked para forzar que esa casilla esté activada inicialmente.

### Botones de radio

Los botones de radio se suelen utilizar cuando el usuario debe elegir sólo una opción específica de varias disponibles. Si las opciones son demasiadas, se suele optar por una lista de selección.

Para tener varios botones radio en un mismo grupo, y que sólo se active uno de ellos, el truco está en colocarle el mismo nombre en el atributo name a cada opción. Luego, en el atributo value le colocamos el valor que habrá seleccionado el usuario de haber marcado esa opción.

Si las casillas de verificación se nos quedan cortas o necesitamos mostrar una lista más extensa de datos, quizás sería conveniente utilizar una lista de selección, también llamada frecuentemente combo o lista desplegable. Estas listas nos permiten mostrar al usuario varias opciones disponibles para que se decanten por una.

Hay un tipo de lista seleccionable:

- Lista (cerrada) de opciones	-> `<select> y <option>`	-> <select> <option>Opción 1</option></select>

### Organización de campos

las siguientes etiquetas, que sirven para organizar mejor los elementos de un formulario, reagrupándolos por categorías o temáticas, mostrándolos de forma más ordenada o incluso para que visualmente sea más sencillo encontrar la información del formulario.

Las etiquetas que veremos son las siguientes:

- Agrupación visual o temática de campos de entrada ->	`<fieldset>`
- Leyenda para la etiqueta `<fieldset>`	-> `<legend>`
- Relación de campo y texto	`<label>`

### Envio de formularios

Por último, y no por ello menos importante, tenemos los botones de envío de formulario. Si un formulario carece de estos botones, el usuario sólo puede enviarlo si pulsa ENTER en el último campo del formulario. No obstante, siempre es aconsejable incluir un botón explícitamente para que el usuario pueda pulsarlo y enviar el formulario sin confusión y de forma clara.

Tenemos varios tipos de botones que actúan sobre el formulario:

- Botón de envío de formulario	-> `<input type="submit">` -> <input type="submit">	
- Botón de envío con imagen	-> `<input type="image">`	-> <input type="image">
- Botón de borrar formulario	-> `<input type="reset">`	-> <input type="reset">
- Botón sin funcionalidad	-> `<input type="button">` o `<button>` -> <button> boton

### Validaciones Html

Al crear un formulario en HTML, debemos ser conscientes de un detalle ineludible: los usuarios se equivocan al rellenar un formulario. Ya sea por equivocación del usuario, ambigüedad del formulario, o error del creador del formulario, el caso es que debemos estar preparados y anticiparnos a estos errores, para intentar que los datos lleguen correctamente a su destino y evitar cualquier tipo de moderación o revisión posterior.

### Atributos básicos

En nuestros campos de entrada de datos, se pueden utilizar ciertos atributos para realizar validaciones sencillas. Algunos de estos atributos ya lo hemos visto en apartados anteriores, sin embargo, vamos a comentarlos uno por uno:

- `minlength`	-> número	-> Campos de texto	-> Establece la longitud mínima del texto requerida.
- `maxlength`	-> número	-> Campos de texto	-> No permite escribir textos superiores a número carácteres.
- `min`
- - `número`	-> Campos numéricos	-> Establece el número mínimo permitido.
- - `fecha`	-> Campos de fecha	-> Establece la fecha mínima permitida.
- - `hora`	-> Campos de hora	-> Establece la hora mínima permitida.
- `max`	
- - `número`	-> Campos numéricos	-> Establece el número máximo permitido.
- - `fecha`	-> Campos de fecha	-> Establece la fecha máxima permitida.
- - `hora`	-> Campos de hora	-> Establece la hora máxima permitida.
- `step`
- - `número`	-> Campos numéricos	-> Establece el salto de números permitido. Por defecto, 1.
- - `fecha`	-> Campos de fecha	-> Establece el salto de días permitido. Por defecto, 1.
-  `hora`	-> Campos de hora	-> Establece el salto de segundos permitido. Por defecto, 1.
- `required`	->	Campos en general	-> Campo obligatorio. Se debe rellenar para enviar formulario.
- `disabled`	->	Campos en general	-> Campo desactivado. No se puede modificar. No se envía.
- `readonly`	->	Campos en general	-> Campo de sólo lectura. No se puede modificar. Se envía.

## Recursos adicionales

* [MDN official CSS documentation](https://developer.mozilla.org/es/docs/Learn/CSS/First_steps/How_CSS_works)
* [MDN official HTML documentation](https://developer.mozilla.org/es/docs/Web/HTML)

<br>
<br>

<table class="hide" width="100%" style='table-layout:fixed;'>
  <tr>
    <td>
      <img src="https://static.thenounproject.com/png/288029-200.png" width="50"/>
      <br>
      <a href="https://forms.gle/MY9PJuXbMnD17e548">
        Has click acá para dejar tu feedback sobre esta clase.
      </a>
    </td>
  </tr>
</table>

---

#### Si tienes dudas sobre este tema, puedes consultarlas en el canal **_Preguntas_** de Discord