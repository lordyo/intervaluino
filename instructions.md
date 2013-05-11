Intervaluino Instructions
========================= 

Warning
-------
With the Intervaluino, you are plugging in a homebrew remote control into your digital camera. The Intervaluino was originally built for a Canon EOS 400D. There are no guarantees that it will work for your brand and model. It might even damage your camera. You have been warned.


Parts List
----------
* 1 Arduino (I used the Diecimila model) -
* 3x 100 ohm resistors
* 1x 10k ohm resistor
* 2 x 5V reed relays (NO = normally open)
* 1 x push button of your choosing
* 1 x 2.5mm male stereo jack
* 1 x 80 x 50 mm strip board (alternatively: bread board or Arduino protoshield)
* Assorted wires
* Arduino USB cable
* Arduino AC adapter OR Arduino 9V battery pack
* Basic electronic tools to cut and de-isolate wires and to solder components (if you use a strip board)
* a multimeter to test connections
* A nice box
* 20 cm of thin steel cable (used as a loop to attach the Intervaluino to the tripod)

Circuit Diagram
---------------
You can check out the circuit diagram in the file intervaluino_circuit_diagram.png

If you want to check out pictures of the assembled Intervaluino, please visit http://timmsuess.com/intervaluino

Assembly
--------
This is only a short instruction, which assumes that you can read simple circuits, understand components, and solder them.

1. According to the circuit diagram, lay out the parts and wires on the strip board to find the right spacing configuration (as opposed to the pictures above, you can use just one strip board for all the parts – no need to use two separate ones)
2. Solder the parts as per circuit diagram (make sure you test the relays – it took me a while to figure out what triggers what!) – don’t connect it to the Arduino yet
3. Solder the stereo jack to the wires (red, yellow, grey) according to the wiring diagram
4. Compile and upload the Intervaluino code (intervaluino_source.ino) via USB
5. Detach the Arduino from USB
6. Connect the strip board to the Ardunino (pins 2, 8, 11, 5V, 3x GND)
7. Connect the Arduino to USB again
8. Wait a couple of second for initialization
9. Press the button
10. Test the device with a multimeter on the stereo jack: Every couple of seconds, the circuit between F and CG should be closed, shortly followed by the circuit between SH and CG.
11. If it works, congratulations! (if it doesn’t, test your circuits thoroughly.)
12. Plug the stereo jack into your camera’s remote shutter release
13. Turn on your camera, focus it on something brightly lit, and set it to single shot
14. Repeat steps 7-9. Your camera should now shoot a picture every couple of seconds
15. Put it into a nice box, cut holes for the cable and the plugs
16. To set your own intervals, follow the instructions in the code (change the values for variables full_time and short_time)

Tips
----
* Use a tripod
* Set your camera to single shot
* Consider turning off autofocus – if you follow a static object, you will only have to focus once.
* For photo series above 1500 shots (or those with flash), get an AC adapter for both your camera and Intervaluino

Possible modifications (untested)
---------------------------------
* Instead of reed relays, use optocouplers. This will reduce the Intervaluino's susceptibility to electromagnetic influence. You will likely need to change the resistor values to do this.
* If your camera features a different kind of electronic remote shutter input, replace the 2.5mm jack with the respective part.
