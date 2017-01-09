# [Slideshow Offline](https://github.com/gitpitch/gitpitch/wiki/Slideshow-Offline)

Click the Offline icon found below the slideshow presentation (https://gitpitch.com/Starignus/RPIGPIO) to have the presentation turned into a self-contained zip archive file, PITCHME.zip, which will download directly from your browser.

Once downloaded, expand the zip archive file. You should see the following files in the top-level directory within the expanded zip archive:

![Figure archive](gp-zip-archive.png)

To launch the slideshow presentation you will need to open the index.html file under a local web server. For example, if you have Python 2 installed on your local system you can move into the top-level directory within the expanded zip archive and launch a simple HTTP server as follows:

```
python -m SimpleHTTPServer
```

Note: At the end we can add a port number

You can then open your GitPitch slideshow presentation in your browser as follows:

```bash
http://localhost:8000
```
You can use any local HTTP server you like to serve your slideshow presentation. If you are unsure what HTTP server to use then this really useful Web Servers GitHub GIST provides an extensive selection of simple-to-use HTTP servers.

Note: As GIST Slides and Video Slides are dependent on Internet access, both are automatically disabled in offline slideshow presentations.
