Preview 'Readme.md'
```js
  var express = require("express");
  console.log("yes");
  var app = express();
  
  app.get('/', function(req, res) {
    res.send("Hello, World!");
  });
  
  app.listen(3000);
```

# Installation

```npm
  $ npm install -g express
```
