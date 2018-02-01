# renewable_download_js
renewable download java script


Installation

Select the directory in which you will solve the problems. Run it:

npm install node-static


Check the installation.

For this:

Create a subdirectory and in it the server.js file with the following content:

var http = require ('http');
var static = require ('node-static');
var file = new static.Server ('.');

http.createServer (function (req, res) {
   file.serve (req, res);
}). listen (8080);

console.log ('Server running on port 8080');

Run it: node server.js.

Should output:

Server running on port 8080

Open in the browser http://127.0.0.1:8080/server.js.

It should output the server.js file.

If everything works fine, now you are ready to solve problems.
