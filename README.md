# Mol Normalize
Para normalizar los estilos que vienen definidos por defecto en cada navegador web.

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
    └── normalize.scss.
```

## Problemas conocidos

`[type="search"]`

Σ(ﾟДﾟ；El input type search por el momento funciona como un input type text, para mantener el estilo general de los inputs, esperamos puedan agregar la funcionalidad con js.
