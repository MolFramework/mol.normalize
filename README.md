# Mol Normalize
Para normalizar los estilos que vienen definidos por defecto en cada navegador web y darle un poco de estilo.

v3.0.0


## Uso e instalación
Para utilizar el normalize en tu proyecto, puedes installarlo con [npm](https://www.npmjs.com/)
```sh
npm install https://github.com/mol-project/mol.normalize.git
```
importa el archivo principal
```sh
@import '~mol.normalize/scss/_normalize.scss';
```
y crea un archivo que contenga las mismas variables que las que se encuentran en
el archivo de `~mol.normalize/scss/_vars.scss`

ó si no tienes tiempo, importa el archivo minificado en tu hoja de estilos principal
```sh
@import '~mol.normalize/dist/normalize.min.css';
```

## Dev
Clona el repositorio
```sh
git clone https://github.com/mol-project/mol.normalize.git
cd mol.normalize/
npm install
```
Edita los archivos dentro de la carpeta de **scss**

#### Scripts
- `npm run dist` Actualiza los archivos minificados de la carpeta de distribución **dist**
- `npm run docs` Levanta un servidor local que se autorefresca con los cambios que se ejecuten en los archivos **scss** y actualiza los archivos de **docs**

#### Archivos
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

#### Variables
```text
@import url('https://fonts.googleapis.com/css?family=Josefin+Sans|Open+Sans|PT+Serif');

$m-font-family: 'Open Sans', sans-serif;
$m-font-size: 16px;
$m-font-weight: 400;
$m-letter-spacing: normal;
$m-line-height: 1.5em;

$m-code-family: monospace;

$m-em-family: 'PT Serif', serif;

$m-h-family: 'Josefin Sans', sans-serif;
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

## Problemas conocidos

(//▽//) El input type search por el momento funciona como un input type text, para mantener el estilo general de los inputs, espero puedan agregar la funcionalidad con js.
