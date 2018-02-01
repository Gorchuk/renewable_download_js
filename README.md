# renewable_download_js
renewable download java script



Installation
To configure the environment it will be sufficient to do two steps:

First, install the Node.JS server itself.

If you have a Unix system - it is recommended that you build the latest version from the sources, as well as NPM. You can do it.

If Windows - visit the site http://nodejs.org or download the installer (32 or 64-bit) with the .msi extension from http://nodejs.org/dist/latest/.

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
