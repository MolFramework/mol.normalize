# m.normalize
Mol Normalize es un archivo para normalizar los estilos que vienen definidos por defecto en cada navegador web. También permite resetear los estilos de un contenedor o de elementos independientes utilizando la funcionalidad de prefix, en el branch de prefix.


Puedes agregar el módulo MolNormalize corriendo la siguiente línea en la consola
```sh
npm install --save https://github.com/flkt-crnpio/m.normalize.git
```
___

### Personaliza el archivo normalize

Necesitas tener instalado [sass](https://sass-lang.com/install)

Puedes ver como se ven los tags abriendo el archivo `index.html` que utiliza el `normalize.css` para cargar los estilos.

En el archivo `_vars.scss` están una lista de variables para modificar el estilo general, como tipograría, color, fondo.

Mientras estes editando los estilos o variables, puedes correr la línea de abajo y refrescar tu navegador para ver los cambios.
```sh
sass --watch _normalize.scss:normalize.css --style expanded
```

Una vez que termines de editar corre la siguiente línea para obtener el archivo comprimido
```sh
sass _normalize.scss:normalize.min.css --style compressed
```


##### Variables especiales

Dentro del branch de 'prefix' se agrega un poco más de funcionalidad para proyectos más específicos. En general es para poder agregar estilos generales sin sobreescribir los que tenga la página, como por ejemplo para widgets.

1. `$m-prefix: nombre` crea una clase con el nombre del prefijo y todo lo que se encuentre dentro del contenedor que utilice la clase tendrá los estilos especificados en la hoja del normalize.

2. `$m-prefix-each: true` convierte todos los tag en clases y les agrega el nombre de prefijo al inicio de cada clase.


___

### Probado y funcionando en los siguientes navegadores
* Brave
* Chrome
* Firefox
* Opera
* Safari
___

### Problemas conocidos

`[type="search"]`

Σ(ﾟДﾟ； No me fué posible agregar estilos al `input type search` sin ocultarlo y redibujarlo primero, entonces, por el momento está funcionando como cualquier campo de texto perdiendo sus propiedades, lo siento. Pero siempre se puede agregar la funcionalidad con javascript, cierto?

-----------

( ﾟ▽ﾟ)/ Hi! [@MolFramework](https://twitter.com/MolFramework)
