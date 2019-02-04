# Mol Normalize
Para normalizar los estilos que vienen definidos por defecto en cada navegador web.

v1.0.0

( ﾟ▽ﾟ)/ Hi! [@MolFramework](https://twitter.com/MolFramework)


## Uso e instalación
Para utilizar el normalize en tu proyecto, puedes installarlo con [npm](https://www.npmjs.com/)
```sh
npm install --save https://github.com/MolFramework/mol.normalize.git
```
e importarlo en tu hoja de estilos principal
```sh
@import '~mol.normalize/dist/normalize.min.css';
```
o si prefieres utilizar tu propio archivo de variables, importa
```sh
@import '~mol.normalize/scss/_normalize.scss';
```
y crea un archivo que contenga las mismas variables que las que se encuentran en
el archivo de `~mol.normalize/scss/_vars.scss`


## Dev
Clona el repositorio
```sh
git clone https://github.com/MolFramework/mol.normalize.git
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

#### Variables específicas del normalize
```text
@import url('https://fonts.googleapis.com/css?family=Montserrat:400,600|Open+Sans:300,400,700');

$m-background:        #fff;
$m-color:             #222029;
$m-primary:           #ff2d39;
$m-secondary:         #2a21a5;
$m-accent:            #2ed7d1;

$m-actn-color:        $m-primary;
$m-actn-color-hover:  mix($m-primary, $m-accent, 90%);
$m-actn-font:         $m-background;
$m-actn-font-hover:   $m-background;

$m-font-family:       'Open Sans', sans-serif;
$m-font-size:         15px;
$m-font-weight:       400;
$m-letter-spacing:    normal;
$m-line-height:       1.5em;

$m-code-family:       monospace;

$m-h-family:          'Montserrat', sans-serif;
$m-h-size:            20px;
$m-h-height:          1em;
$m-h-spacing:         normal;
$m-h-weight:          600;
$m-h-style:           normal;
$m-h-transform:       normal;

$m-transition:        all 0.3s cubic-bezier(0.465, 0.240, 0.370, 0.825);
```

## Problemas conocidos

`[type="search"]`

Σ(ﾟДﾟ；El input type search por el momento funciona como un input type text, para mantener el estilo general de los inputs, esperamos puedan agregar la funcionalidad con js.
