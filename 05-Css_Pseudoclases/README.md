![LarnU](../_src/assets/00-PrimerosPasos/logo_LarnU.png)

<br>
<br>

# Desafío: css_pseudoclases

## Instrucciones

Completa los siguientes desafíos, para que pueda funcionar de manera correcta los códigos css.

I. Establezca el color de fondo en rojo cuando pase el mouse sobre un enlace.

```
<style>
 tuCodigoAca {
  background-color: red;
}
</style>

<body>

<h1>This is a header.</h1>
<p>This is a paragraph.</p>
<a href="https://larnu.app/#/">This is a link.</a>

</body>
```

II. Establezca el color de fondo en rojo, cuando pase el mouse sobre elementos con la clase "maestro".

```
<style>
 tuCodigoAca {
  background-color: red;
}
</style>

<body>

<h1 class="master">This is a header.</h1>
<p class="master">This is a paragraph.</p>
<p>This is a paragraph.</p>

</body>
```

III. Establezca el color de fondo en rojo, de cualquier elemento `<p>` que sea el primer hijo de cualquier elemento.

```
<style>
 tuCodigoAca {
  background-color: red;
}
</style>

<body>

<p>This is a paragraph.</p>
<p>This is a paragraph.</p>

</body>
```

VI. Establezca el color de fondo en rojo, de cualquier elemento `<input>` que esté enfocado.

```
<style>
 tuCodigoAca {
  background-color: red;
}
</style>

<body>

<form>
  Name:
  <input type="text" name="fname">
  Age:
  <input type="text" name="age">
</form>

</body>
```

V. Establezca el color de fondo en rojo, de la primera línea del párrafo.

```
<head>
<style>
 tuCodigoAca {
  background-color: red;
}
</style>

<body>

<p class="intro">
In my younger and more vulnerable years
my father gave me some advice that I've
been turning over in my mind ever since.
'Whenever you feel like criticizing anyone,' he told me,
'just remember that all the people in this world
haven't had the advantages that you've had.'
</p>

</body>
```

VI. Establezca el color de fondo en rojo, para la primera letra del elemento `<p>`.

```
<style>
 tuCodigoAca {
  background-color: red;
}
</style>

<body>

<p class="intro">
In my younger and more vulnerable years
my father gave me some advice that I've
been turning over in my mind ever since.
'Whenever you feel like criticizing anyone,' he told me,
'just remember that all the people in this world
haven't had the advantages that you've had.'
</p>

</body>
```

VII. Inserte la imagen "smiley.gif" antes y después de cualquier elemento `<p>`, utilizando los pseudoelementos ::before y ::after.

```
<style>
tuCodigoAca {
  tuCodigoAca: url('smiley.gif');
}
tuCodigoAca {
  tuCodigoAca: url('smiley.gif');
}
</style>

<body>

<p>This is a paragraph.</p>
<p>This is a paragraph.</p>

</body>
```