# Scaredy Pants Showcase
<img width="1410" height="2000" alt="Image" src="https://github.com/user-attachments/assets/2503d0c0-5f22-43a9-9bb5-f7e7b7eacbaa" />

# Description
Scaredy pants is a pretty simple thing, it detects that its falling then it plays a recording of whatever sound you recorded on the microbit while showing on the fancy OLED display thats it has sadly fallen or you could show a sad face but i decided to keep it simple with a simple "ive fallen!" message. It can also let other microbit devices know it has fallen via radio which you could use to check if it has well, fallen.

# Reason
The reason i made this was honestly mostly to get a laugh out of it! I knew how to do it from the start (after all its pretty basic) and figured it would be a great project to make something funny while learning the basics of wiring and onshape. Laughter is the best medicince so maybe its a medical device.

# Usage
Open up the Scaredy Pants and Plug the Microbit into a computer. Load the program onto it fully so it can run it without being attached to the computer. Then press button A to start recording a soundbyte for the falling sound. When its done recording Put the microbit and the Kitronic Breakout board into the box then before you fully close it put the ssd1306 32*128 though the gap sideways so it fits. Then youre all set! Put it around anywhere and when it falls (preferebly with a cushion underneath) It will send the signal, play the sound and show the "ive fallen" message. Then if you want to reset it, open up the scaredy pants again but this time just click the button on the back of the microbit to reset it.

# Assembly
To assemble the Scaredy pants you will need to make the wiring and the shell. The wiring is the same for both versions but the shell is different on each.

-Wiring: To start you will need to solder on two headers onto the Kitronic Edge Connector Breakout Board on the pins 19&20. These are the SCL and SDA pins for the I2C connection to the microbit. After Soldering on said two pins, connect the Microbit to the Breakout board using the Edge connector. Next you will grab the ssd1306 32*128 display and using dupont cables, you wil connect the GND pin on the display to the 0V on the kitronic breakout board. Then connect the VCC pin on the display to the 3V pin on the breakout board. Then connect the SCL pin on the display to the newly soldered pin 19 on the breakout board. And lastly connect the SDA pin on the display to the second soldered pin, pin 20 on the breakout board. You now have the full wiring complete, it should look something like this:
<img width="1152" height="2048" alt="image" src="https://github.com/user-attachments/assets/1940559a-a15d-4510-b3d9-c7ba3aa3b596" />
<img width="1152" height="2048" alt="image" src="https://github.com/user-attachments/assets/e45c6261-2fbb-44f3-9319-487a4a172c30" />


