capture_uvc.py
====
simple still image capture tool for UVC camera.


Setup
----
    $ sudo apt-get install v4l-utils python-opencv python-dev
    $ wget https://.../capture_uvc.py
    $ chmod +x capture_uvc.py

How to use:
----
   $ v4l2-ctl --device=/dev/video0 --list-formats-ext
   $ v4l2-ctl --device=/dev/video0 -c exposure_auto=1,exposure_auto_priority=0,exposure_absolute=160
   $ ./capture_uvc.py -w 1920 -h 1080 -o capture.png

Copyright and license
----
Copyright (c) 2016 yoggy

Released under the [MIT license](LICENSE.txt)
