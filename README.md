## Mol Normalize ##
Nueva versión en [mol-normalize](https://github.com/flkt-crnpio/mol-normalize)

.

.

.

___

### Para usar esta librería ###

```sh
npm install --save-dev https://github.com/mol-project/mol.normalize.git
```

Crea o copia el archivo de [variables](https://github.com/mol-project/mol.normalize/blob/master/scss/_vars.scss) para editar la tipografía, colores y media queries
*Create a var file like [this file](https://github.com/mol-project/mol.normalize/blob/master/scss/_vars.scss) where you can edit general style aspects*

En el archivo general de SCSS de tu proyecto, importa el archivo de variables y el archivo principal de la librería *Import the vars and main files in to your project scss file*
```sh
@import '_vars.scss';
@import '~mol.normalize/scss/_normalize.scss';
```

Y compilalo con el resto de tu código, para evitar cargar tantos archivos. 
*Compile this with your code and avoid to load a lot of files*

### Archivo de distribución ###
Descarga el archivo de distrubución y usalo en el head de tu proyecto. 
*Download the distribution file and added into your head project*
[mol.normalize](https://raw.githubusercontent.com/mol-project/mol.normalize/master/dist/normalize.min.css)
```text
<link rel="stylesheet" href="mol.normalize.css">
```

### Variables ###
```text
$m-font-family: sans-serif;
$m-font-size: 16px;
$m-font-weight: 400;
$m-letter-spacing: normal;
$m-line-height: 1.5em;

$m-code-family: monospace;

$m-em-family: serif;

$m-h-family: sans-serif;
$m-h-size: 23px;
$m-h-height: 1em;
$m-h-spacing: normal;
$m-h-weight: 600;
$m-h-style: normal;
$m-h-transform: none;

$m-colors: (
  "background": #0a0838,
  "font": #fff,
  "primary": #ff5252
);

$m-queries: (
  "phone": (
    "since": 320px,
    "until": 767px,
  ),
  "tablet": (
    "since": 768px,
    "until": 1024px,
  ),
  "laptop": (
    "since": 1025px,
    "until": 1599.99px,
  ),
  "desktops": (
    "since": 1600px,
    "until": 99999px,
  )
);
```

### Archivos ###
```text
mol.normalize/
├── dist/
│   ├── normalize.min.css
│   └── normalize.min.css.map
├── docs/
│   ├── index.html
│   ├── normalize.css
│   └── normalize.css.map
└── scss/
    ├── _normalize.scss
    ├── _vars.scss
    └── normalize.scss
```

## Problemas conocidos ##

(//▽//) El input type search por el momento funciona como un input type text, para mantener el estilo general de los inputs, espero puedan agregar la funcionalidad con js. *The input type search is working like a simple input text, in order to maintain coherence input design, sorry.*
