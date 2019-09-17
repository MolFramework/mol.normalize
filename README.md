# Mol Normalize #
Para normalizar los estilos que vienen definidos por defecto en cada navegador web y darle un poco de estilo. *This project if for normalize styles given by default for each web browser and it is for add a few custom style too.*

## Para usar la librería *How to use* ##
Instala la librería *Install the library*

```sh
npm install --save-dev https://github.com/mol-project/mol.normalize.git
```

Crea un archivo con las variables que las que se encuentran en el archivo de `~mol.normalize/scss/_vars.scss`[^1] para editar la tipografía, colores y media queries
*Create a var file that must have same vars like they are in the `~mol.normalize/scss/_vars.scss`[^1] file where you can edit general style aspects*

En el archivo general de SCSS de tu proyecto, importa el archivo de variables y el archivo principal de la librería *Import the vars and main files in to your project scss file*
```sh
@import '_vars.scss';
@import '~mol.normalize/scss/_normalize.scss';
```

Y compilalo con el resto de tu código, para evitar cargar tantos archivos. *Compile this with your code and avoid to load a lot of files*

## Archivo de distribución *Distribution File* ##
[mol.normalize](https://raw.githubusercontent.com/mol-project/mol.normalize/master/dist/normalize.min.css)


### [^1]: Variables ###
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
    "width": 100%,
    "minwidth": inherit,
    "maxwidth": inherit
  ),
  "tablet": (
    "since": 768px,
    "until": 1024px,
    "width": 100%,
    "minwidth": inherit,
    "maxwidth": inherit
  ),
  "laptop": (
    "since": 1025px,
    "until": 1599.99px,
    "width": 100%,
    "minwidth": inherit,
    "maxwidth": inherit
  ),
  "desktops": (
    "since": 1600px,
    "until": 99999px,
    "width": 100%,
    "minwidth": inherit,
    "maxwidth": inherit
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
