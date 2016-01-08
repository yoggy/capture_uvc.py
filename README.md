capture_uvc.py
====
Simple still image capture tool for UVC camera.

Setup
----
    $ sudo apt-get install v4l-utils python-opencv python-dev
    $ wget https://.../capture_uvc.py
    $ chmod +x capture_uvc.py

How to use:
----
UVC camera parameter settings...

    
    $ v4l2-ctl --device=/dev/video0 --list-formats-ext
    $ v4l2-ctl --device=/dev/video0 -c exposure_auto=1,exposure_auto_priority=0,exposure_absolute=160
    

Capture still image.

    
    $ ./capture_uvc.py 1920x1080 capture.png
    

Copyright and license
----
Copyright (c) 2016 yoggy

Released under the [MIT license](LICENSE.txt)
