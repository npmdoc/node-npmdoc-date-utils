# api documentation for  [date-utils (v1.2.21)](https://jerrysievert.github.io/date-utils/)  [![npm package](https://img.shields.io/npm/v/npmdoc-date-utils.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-date-utils) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-date-utils.svg)](https://travis-ci.org/npmdoc/node-npmdoc-date-utils)
#### Date add-ons for Node.js

[![NPM](https://nodei.co/npm/date-utils.png?downloads=true)](https://www.npmjs.com/package/date-utils)

[![apidoc](https://npmdoc.github.io/node-npmdoc-date-utils/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-date-utils_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-date-utils/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-date-utils/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-date-utils/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Jerry Sievert",
        "email": "code@legitimatesounding.com",
        "url": "http://legitimatesounding.com/blog/"
    },
    "bugs": {
        "url": "http://github.com/JerrySievert/date-utils/issues"
    },
    "contributors": [
        {
            "name": "Jerry Sievert",
            "url": "http://legitimatesounding.com"
        }
    ],
    "dependencies": {},
    "description": "Date add-ons for Node.js",
    "devDependencies": {
        "gulp": "^3.7.0",
        "gulp-complexity": "^0.2.1",
        "gulp-rename": "^1.2.0",
        "gulp-shell": "^0.2.8",
        "gulp-uglify": "^0.3.0",
        "ink-docstrap": "^0.4.12",
        "jsdoc": "^3.3.0-alpha9",
        "vows": ">=0.7.0"
    },
    "directories": {
        "lib": "./lib",
        "test": "./test"
    },
    "dist": {
        "shasum": "61fb16cdc1274b3c9acaaffe9fc69df8720a2b64",
        "tarball": "https://registry.npmjs.org/date-utils/-/date-utils-1.2.21.tgz"
    },
    "engines": {
        "node": ">0.4.0"
    },
    "gitHead": "0118289aca58fdb26ac7889f2099f73401cf31f1",
    "homepage": "https://jerrysievert.github.io/date-utils/",
    "keywords": [
        "date",
        "utils",
        "date-utils",
        "time"
    ],
    "license": "MIT",
    "main": "./lib/date-utils",
    "maintainers": [
        {
            "name": "jerrysievert",
            "email": "code@legitimatesounding.com"
        }
    ],
    "name": "date-utils",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+ssh://git@github.com/JerrySievert/date-utils.git"
    },
    "scripts": {
        "test": "vows -i --spec"
    },
    "version": "1.2.21"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module date-utils](#apidoc.module.date-utils)
1.  [function <span class="apidocSignatureSpan">date-utils.</span>language (lang)](#apidoc.element.date-utils.language)



# <a name="apidoc.module.date-utils"></a>[module date-utils](#apidoc.module.date-utils)

#### <a name="apidoc.element.date-utils.language"></a>[function <span class="apidocSignatureSpan">date-utils.</span>language (lang)](#apidoc.element.date-utils.language)
- description and source-code
```javascript
language = function (lang) {
    if (lang == "es") {
        monthsAbbr = [
            'Ene',
            'Feb',
            'Mar',
            'Abr',
            'May',
            'Jun',
            'Jul',
            'Ago',
            'Sep',
            'Oct',
            'Nov',
            'Dic'
        ];

        monthsFull = [
            'Enero',
            'Febrero',
            'Marzo',
            'Abril',
            'Mayo',
            'Junio',
            'Julio',
            'Agosto',
            'Septiembre',
            'Octubre',
            'Noviembre',
            'Diciembre'
        ];

        daysAbbr = [
            'Dom',
            'Lun',
            'Mar',
            'Mie',
            'Jue',
            'Vie',
            'Sab'
        ];

        daysFull = [
            'Domingo',
            'Lunes',
            'Martes',
            'Miércoles',
            'Jueves',
            'Viernes',
            'Sábado'
        ];

        dayNames = {
            'do': 0,
            'dom': 0,
            'domingo': 0,
            'lu': 1,
            'lun': 1,
            'lunes': 1,
            'ma': 2,
            'mar': 2,
            'martes': 2,
            'mi': 3,
            'mie': 3,
            'miercoles': 3,
            'ju': 4,
            'jue': 4,
            'jueves': 4,
            'vi': 5,
            'vie': 5,
            'viernes': 5,
            'sa': 6,
            'sab': 6,
            'sabado': 6
        };
        monthsAll = monthsFull.concat(monthsAbbr);
        daysAll = [
            'do',
            'dom',
            'domingo',
            'lu',
            'lun',
            'lunes',
            'ma',
            'mar',
            'martes',
            'mi',
            'mie',
            'miércoles',
            'ju',
            'jue',
            'jueves',
            'vi',
            'vie',
            'viernes',
            'sa',
            'sab',
            'sábado'
        ];

        monthNames = {
            'ene': 0,
            'enero': 0,
            'feb': 1,
            'febrero': 1,
            'mar': 2,
            'marzo': 2,
            'abr': 3,
            'abril': 3,
            'may': 4,
            'mayo':4,
            'jun': 5,
            'junio': 5,
            'jul': 6,
            'julio': 6,
            'ago': 7,
            'agosto': 7,
            'sep': 8,
            'septiembre': 8,
            'oct': 9,
            'octubre': 9,
            'nov': 10,
            'noviembre': 10,
            'dic': 11,
            'diciembre': 11
        };
    } else if (lang == "fr") {
        monthsAbbr = [
            'Jan',
            'Fév',
            'Mar',
            'Avr',
            'Mai',
            'Jui',
            'Jul',
            'Aoû',
            'Sep',
            'Oct',
            'Nov',
            'Déc'
        ];

        monthsFull = [
            'Janvier',
            'Février',
            'Mars',
            'Avril',
            'Mai',
            'Juin',
            'Juillet',
            'Août',
            'Septembre',
            'Octobre',
            'Novembre',
            'Décembre'
        ];

        daysAbbr = [
            'Dim',
            'Lun',
            'Mar',
            'Mer',
            'Jeu',
            'Ven',
            'Sam'
        ];

        daysFull = [
            'Dimanchi',
            'Lundi',
            'Mardi',
            'Mercredi',
            'Jeudi',
            'Vendredi',
            'Samedi'
        ];

        dayNames = {
            'di': 0,
            'dim': 0,
            'dimanchi': 0,
            'lu': 1,
            'lun': 1,
            'lundi': 1,
            'ma': 2,
            'mar': 2,
            'mardi': 2,
            'me': 3,
            'mer': 3,
            'mercredi': 3,
            'je': 4,
            'jeu': 4,
            'jeudi': 4,
            've': 5,
            'ven': 5,
            'vendredi': 5,
            'sa': 6,
            'sam': 6,
            'samedi': 6
        };
        monthsAll = monthsFull.concat(monthsAbbr);
        days ...
```
- example usage
```shell
...
    $ npm install date-utils

    require('date-utils');

Note: This did not work in the 'REPL' before 'Node.js 0.6' due to how 'Node.js' handles context in the 'REPL'.

## Changing Languages
    require('date-utils').language("es")

Supported languages:

- Spanish - "es"
- French - "fr"
- Portuguese Brazilian - "pt-BR"
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
