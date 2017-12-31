# Node JS - Building the application stack

### A Basic HTTP Server
Create a new file *server.js*.

```javascript
var http = require("http");

http.createServer(function(request, response) {
  response.writeHead(200, {"Content-Type": "text/plain"});
  response.write("Hello World");
  response.end();
}).listen(8888);
```

Run and test it.
```shell
node server.js
```

Open browser and go to [localhost](http://localhost:8888).
This should display a web page that says "Hello World".