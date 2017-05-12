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
