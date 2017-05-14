# js-env

[EditorConfig](http://editorconfig.org/) helps developers define and maintain consistent coding styles between different editors and IDEs.

**package managers:**
- [Bower](https://bower.io/)
- [npm](https://www.npmjs.com/)
- [JSPM](http://jspm.io/)
- Jam
- volo

**package security:**
- retire.js
- [Node security platform](https://nodesecurity.io/)
```
npm install -g nsp
nsp check
```

**development webservers:**
- [http-server](https://www.npmjs.com/package/http-server)
- [live-server](https://www.npmjs.com/package/live-server)
- [express](https://expressjs.com/)
- budo
- webpack dev server
- [browsersync](https://www.browsersync.io/)

**sharing local projects:**
- [localtunnel](https://localtunnel.github.io/www/)
- [ngrok](https://ngrok.com/)
- Surge
- now
```
npm install localtunnel -g
node buildScripts/srcServer.js
lt --port 3000
lt --port 3000 --subdomain klymchuk
```

**task runners:**
- [grunt](https://gruntjs.com/)
- [gulp](http://gulpjs.com/)
- [npm scripts](https://docs.npmjs.com/misc/scripts)
```
 "scripts": {
    "start": "node buildScripts/srcServer.js",
 },
  
  npm run start
  npm start -s
```

**transpilers:**
- [babel](https://babeljs.io/)
- [typeScript](https://www.typescriptlang.org/)
- elm

_.babelrc_
```
{
  "presets": [
    "latest"
  ]
}
```
_package.json_
```
 "devDependencies": {
    "babel-cli": "6.16.0",
    "babel-core": "6.17.0",
    "babel-loader": "6.2.5",
    "babel-preset-latest": "6.16.0",
    "babel-register": "6.16.3",
    .....
 ```
 after that we can use es6 syntax:
 ```
 //--es5
var express = require('express');
var path = require('path');
var open = require('open');
var port = 3000;
var app = express();

//es6 from babel
import express from 'express';
import path from 'path';
import open from 'open';
const port = 3000;
const app = express();
```
 
for using es6 syntax we need to use **babel-node** instead of **node**
```
  "scripts": {
    "prestart": "babel-node buildScripts/startMessage.js",
```

**bundlers:**
- [browserify](http://browserify.org/)
- [webpack](https://webpack.github.io/docs/)
- [rollup](https://rollupjs.org/)
- [JSPM](http://jspm.io/)
