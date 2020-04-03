# mise en place d'un projet d3

Dans un nouveau dossier:

```
npm init -y
npm install parcel-bundler --save-dev
npm install d3 --save
```

Dans `.gitignore`

```
node_modules
dist
.cache
```

Dans un dossier `src`

## `src/index.html`

```html
<!DOCTYPE html>
<html>
  <head>

  </head>
  <body>
    <script src="index.js"></script>
  </body>
</html>
```

## `src/index.js`

```js
import * as d3 from 'd3'

console.log(d3)
```

Dans `package.json`, un scripte pour démarrer:

```js
{
  "name": "mise-place-d3",
  "version": "1.0.0",
  "description": "",
  "main": "index.js",
  "scripts": {
    "test": "echo \"Error: no test specified\" && exit 1",
    "dev": "parcel src/index.html"
  },
  "keywords": [],
  "author": "",
  "license": "ISC",
  "devDependencies": {
    "parcel-bundler": "^1.12.4"
  },
  "dependencies": {
    "d3": "^5.15.1"
  }
}
```