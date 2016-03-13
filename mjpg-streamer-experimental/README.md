mjpg-streamer
=============

Currently no issues are known, but since this software is quite young and not used widely it may cause problems. You must really know what you are doing, if you use this software. If you want to use the software you are obliged to check if the sourcecode does what you expect it to do and take the risk yourself to use it.


Usage
=====

When launching mjpg-streamer, you specify one or more input plugins and an output plugin. For example, to stream a V4L compatible webcam via an HTTP server (the most common use case), you
can do something like this:

	mjpg_streamer -i input_uvc.so -o output_http.so

Each plugin supports various options, you can view the plugin's options via its `--help` option:

	mjpg_streamer -i 'input_uvc.so --help'


More examples can be found in the start.sh bash script.

Plugin documentation
====================

Input plugins:

* input_testpicture
* input_http

Output plugins:

* output_http ([documentation](plugins/output_http/README.md))
