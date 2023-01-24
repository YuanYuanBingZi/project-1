# UOCIS322 - Project 1 #

This project will get you started with creating a simple webpage server.

## Getting started

Directory structure:

* the "pages" (HTML files and their assets) will be located in DOCROOT. For this project that location is the `pages/` directory. Make sure you specify this in your `credentials.ini`!

* Everything that's located in `pageserver/`. That consists of a Python application (`pageserver.py`) that starts listening at a specified port and handles requests. This is the key file you'll be editing for this project.

* There's a configuration parser, much like the one seen in [project-0](https://github.com/UO-CIS322/project-0), but a more detailed version. It not only looks for your `credentials.ini` file, both in `pageserver/` and the parent directory and falls back to `default.ini` if missing, it also allows you to override those settings through CLI. These will be discussed in the lab.

* `Makefile` here refers to the two scripts provided: `start.sh` and `stop.sh`. The former starts the server, by calling `pageserver.py`. It will also store its PID (process id), in order to kill it later through `stop.sh`. However, if you notice that it failed to do so, you can kill it manually by looking up the PID.

## Tasks INFO
* NAME: TONG GUAN
* INFO: project 1 of class 322
* Brief Description:
* The project 1 is a simple web server. We use the socket to listen to the port and serve the connection. In our specified local host, if you type the existed html or css file, you can directly see them in broswer. However, if you type some thing illegal, like "~~" or "..", you will get 403 STATUS_FORBIDDEN. Or you type a filename that does not exist in our folder, you will get the 404 STATUS_NOT FOUND.

## Grading Rubric

* If everything works as expected, 100 will be assigned.
* If existing pages and files are NOT handled correctly, 30 points will be docked.
* For each of the errors not handled correctly (403, and 404), 15 points will be docked.
* If `README.md` is not updated with your name and info, 10 points will be docked.
* If `credentials.ini` is commited, 10 points will be docked.
* If the repo clones, but `make install` or `make run` throws an error, 10 will be assigned.
* If `credentials.ini` is incorrect or not submitted, 0 will be assigned.

## Authors

Michal Young, Ram Durairajan.
