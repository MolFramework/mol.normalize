# Normalize
Para normalizar los estilos que vienen definidos por defecto en cada navegador web.

( ﾟ▽ﾟ)/ Hi! [@MolFramework](https://twitter.com/MolFramework)

### Uso

Instalación con [npm](https://www.npmjs.com/):
```sh
npm install --save https://github.com/MolFramework/normalize.git
```

### Contenido
```text
normalize/
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

### Problemas conocidos

`[type="search"]`

Σ(ﾟДﾟ；El input type search por el momento funciona como un input type text, para mantener el estilo general de los inputs, esperamos puedan agregar la funcionalidad con js.
