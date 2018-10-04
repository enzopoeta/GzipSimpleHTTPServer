GzipSimpleHTTPServer
====================
Python 3.x ported (thanks for the help https://github.com/rdenadai) ! 
 
A simple modification of the very useful SimpleHTTPServer python script originally made to add gzip compression. It now supports gzip, zlib, and deflate with gzip as the implicit default.

### Static gzip file support added
If you have large files and do not want that the server performs the compression on a per-request basis, you need to compress these files and save them with the same name as the original file by adding the text ".gz" at the end, so the server will give preference to these files files instead of redoing the compression.

### With Python 3.x

````
python3 GzipSimpleHTTPServer.py
````

This will start a localhost server on port 8000. You should see this in your terminal:

````
Serving HTTP on 0.0.0.0 port 8000 ...
````

To run on a different port use:
````
python GzipSimpleHTTPServer.py --port=8080
````

For more options run:
````
python GzipSimpleHTTPServer.py --help
````
