# COMP2322-Project
1. Open terminal, and enter python server.py
2. Using the REST extension on vs code send these test cases:
###GET HTML file
GET http://127.0.0.1:8080/test.html

###

###GET image
GET http://127.0.0.1:8080/image.jpg

###

###HEAD request
HEAD http://127.0.0.1:8080/test.html
###

###Request with If-Modified-Since (to test 304 Not Modified)
GET http://127.0.0.1:8080/test.html
If-Modified-Since: <paste the Last-Modified value here>

###

###Non‑persistent connection
GET http://127.0.0.1:8080/test.html
Connection: close

###

###Persistent connection (keep‑alive, default in HTTP/1.1)
GET http://127.0.0.1:8080/test.html
Connection: keep-alive

###

###Request a non‑existent file → 404 Not Found
GET http://127.0.0.1:8080/missing.txt
3. the server should respond.
