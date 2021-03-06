ESP WebSockets Sample
===

This sample demonstrates writing large, streaming response without blocking, 
buffering or consuming excessive memory. This sends a large file as a single 
web socket message using multiple frames.

The sample is implemented as an ESP controler with one action. A test web 
page initiates the client WebSocket request to retrieve the file. To run, 
browse to:

    http://localhost:8080/test.html

Requirements
---

* [Appweb](http://embedthis.com/downloads/appweb/download.ejs)
* [Bit Build Tool](http://embedthis.com/downloads/bit/download.ejs)

To build:
---
    bit 

To run:
---
    bit run

The server listens on port 8080. Browse to: 
 
     http://localhost:8080/test.html

This opens a web socket and and listens for WebSocket data sent by the server. 
It will display the received data in the browser window.

Code:
---
* [cache](cache) - Directory for compiled ESP modules
* [appweb.conf](appweb.conf) - Appweb server configuration file
* [echo.c](echo.c) - WebSockets echo server code
* [start.bit](start.bit) - Bit build instructions
* [web](web) - Directory containing the test.html web page

Documentation:
---
* [Appweb Documentation](http://embedthis.com/products/appweb/doc/index.html)
* [ESP Directives](http://embedthis.com/products/appweb/doc/guide/appweb/users/dir/esp.html)
* [ESP Tour](http://embedthis.com/products/appweb/doc/guide/esp/users/tour.html)
* [ESP Controllers](http://embedthis.com/products/appweb/doc/guide/esp/users/controllers.html)
* [ESP APIs](http://embedthis.com/products/appweb/doc/api/esp.html)
* [ESP Guide](http://embedthis.com/products/appweb/doc/guide/esp/users/index.html)
* [ESP Overview](http://embedthis.com/products/appweb/doc/guide/esp/users/using.html)

See Also:
---
* [esp-controller - Serving ESP controllers](../esp-controller/README.md)
* [esp-mvc - Serving ESP MVC applications](../esp-mvc/README.md)
* [esp-page - Serving ESP pages](../esp-page/README.md)
* [secure-server - Secure server](../secure-server/README.md)
* [simple-server - Simple server and embedding API](../simple-server/README.md)
* [typical-server - Fully featured server and embedding API](../typical-server/README.md)
