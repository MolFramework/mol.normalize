# mol.normalize

Librería para normalizar las etiquetas de HTML. Los títulos se muestran en diferente tamaño para celulares o escritorio. Agrega tu tipografía favorita mediante variables. Edita el color de fondo, del texto y de acción en el archivo de variables.


Por si no quieres editar nada, aqui esta el archivo de distrubucion de
[mol.normalize](https://github.com/mol-project/mol.normalize/blob/master/dist/), puedes descargarlo y agregarlo en la cabecera de tu proyecto
```text
<link rel="stylesheet" href="mol.normalize.css">
```

## instalación

### 1. Guarda el modulo en tu entorno de desarrollo
```sh
npm install --save-dev https://github.com/mol-project/mol.normalize.git
```

### 2. Crea tu carpeta de estilos
```sh
mkdir -p src/scss
```

### 3.(a) Copia el archivo de [variables](https://github.com/mol-project/mol.normalize/blob/master/scss/_vars.scss) para editar la tipografía, colores y media queries
```sh
cp node_modules/mol.normalize/scss/_vars.scss src/scss
```


### 3.(b) ó crea un archivo nuevo y agrega las variables requeridas

```sh
touch src/scss/_vars.scss
```

Variables requeridas:
```text
$m-font-family: sans-serif;
$m-font-size: 16px;
$m-font-weight: 400;
$m-letter-spacing: normal;
$m-line-height: 1.5em;

$m-code-family: monospace;

$m-em-family: serif;

$m-h-family: sans-serif;
$m-h-mobile-size: 14px;
$m-h-size: 23px;
$m-h-height: 1em;
$m-h-spacing: normal;
$m-h-weight: 600;
$m-h-style: normal;
$m-h-transform: none;

$m-colors: (
  "background": #fff,
  "font": #222,
  "primary": #38E9B5
);

$m-queries-limit: (
  "mobile": 768px
);
```

### 4. Importa los archivos en tu archivo principal de estilos

```text
@import '_vars.scss';
@import '~mol.normalize/scss/_normalize.scss';
```

Y compilalo con el resto de tu código, para evitar cargar tantos archivos. 

___

## estructura del proyecto
Todo lo editable esta en la carpeta de `scss`. En la carpeta `docs` estan las muestras del formato de la etiqueta. En la carpeta `dist` se guardan los archivos comprimidos finales para importar.

```text
mol.normalize/
├── dist/
│   ├── mol.normalize.min.css
│   └── mol.normalize.min.css.map
├── docs/
│   ├── assets
│   │   └── esparragus-elelelelperrito-2016.jpg
│   ├── index.html
│   ├── mol.normalize.css
│   └── mol.normalize.css.map
└── scss/
    ├── _normalize.scss
    ├── _vars.scss
    └── normalize.scss
```
