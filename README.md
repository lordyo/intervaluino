Intervaluino
============
An open source intervalometer for DSLR cameras using the Arduino microcontroller

Usage
-----
The Intervaluino is an open hardware intervalometer. It allows you to control your DSLR camera to take a picture every X seconds to create time-lapse videos with excellent picture quality. The Arduino microcontroller used in this project can be programmed via USB to the desired interval. Key features:

*Works for Canon cameras that use a 2.5mm stereo jack-controlled remote shutter release (EOS 300D, 350D, 400D, DigitalRebel)
*Powered by USB, AC adapter or 9V battery
*Timing programmable via the Arduino programming interface
*Start/stop push button
*Focuses before shooting
*Maximum interval between shots: 24 days 20 hours

Prerequisites
-------------
In order to build an Intervaluino you will need to:
*be able to read simple circuit diagrams
*be able to solder
*be familiar with basic Arduino functionality (how to upload code)

In order to use the Intervaluino, you will need to have a camera which accepts *digital* shutter release input - in the current configuration via a 2.5mm stereo jack. If you can find remote shutter release cables for your camera, then the intervaluino will probably work. It won't work with cameras using purely mechanical (piston) or no shutter release input.

Warning
-------
The Intervaluino was originally built for a Canon EOS 400D. There are no guarantees that it will work for your brand and model. It might even damage your camera. 

Parts, assembly and installation
--------------------------------
Please read the separate instructions.

Contributing
------------
* Create something awesome -- make the configuration or code better, add some functionality, whatever (this is the hardest part).
* `Fork it`
* Create a topic branch to house your changes
* Get all of your commits in the new topic branch
* Submit a `pull request`

More about Intervaluino
-----------------------
*Intervaluino's home: http://timmsuess.com/intervaluino (with pictures)
*Intervaluino on Make:  http://blog.makezine.com/2008/06/22/how-to-timelapse-photos-w/
*Intervaluino Plus:  http://tech.enekochan.com/2012/06/21/intervaluino-plus-a-configurable-intervalometer-made-with-arduino/

License
-------
Copyright 2008 by Timm Suess, timmsuess.com

Published under a [Creative Commons -by -nc -sa 3.0 license] https://creativecommons.org/licenses/by-nc-sa/3.0/ : Use it, share it, change it, as long as you tell it’s based on my work (refer to Timm Suess, timmsuess.com), don’t use it commercially, and use the same or similar license for derivatives.