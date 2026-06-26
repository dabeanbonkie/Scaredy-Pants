# Scaredy Pants Showcase
<img width="1410" height="2000" alt="image" src="https://github.com/user-attachments/assets/5d3b670a-7326-4c52-8bfe-4d37d82e8117" />


# Description
Scaredy pants is a pretty simple thing, it detects that its falling then it plays a recording of whatever sound you recorded on the microbit while showing on the fancy OLED display thats it has sadly fallen or you could show a sad face but i decided to keep it simple with a simple "ive fallen!" message. It can also let other microbit devices know it has fallen via radio which you could use to check if it has well, fallen.

# Reason
The reason i made this was honestly mostly to get a laugh out of it! I knew how to do it from the start (after all its pretty basic) and figured it would be a great project to make something funny while learning the basics of wiring and onshape. Laughter is the best medicince so maybe its a medical device.

# Usage
Open up the Scaredy Pants and Plug the Microbit into a computer. Load the program onto it fully so it can run it without being attached to the computer. Then press button A to start recording a soundbyte for the falling sound. When its done recording Put the microbit and the Kitronic Breakout board into the box then before you fully close it put the ssd1306 32*128 though the gap sideways so it fits. Then youre all set! Put it around anywhere and when it falls (preferebly with a cushion underneath) It will send the signal, play the sound and show the "ive fallen" message. Then if you want to reset it, open up the scaredy pants again but this time just click the button on the back of the microbit to reset it.

# Assembly
To assemble the Scaredy pants you will need to make the wiring and the shell. The wiring is the same for both versions but the shell is different on each.

-Wiring: To start you will need to solder on two headers onto the Kitronic Edge Connector Breakout Board on the pins 19&20. These are the SCL and SDA pins for the I2C connection to the microbit. After Soldering on said two pins, connect the Microbit to the Breakout board using the Edge connector. Next you will grab the ssd1306 32*128 display and using dupont cables, you wil connect the GND pin on the display to the 0V on the kitronic breakout board, the connect VCC on the display to the 3V pin on the breakout, then connect SCL to pin 19 on the breakout board, then lastly connect SDA to pin 20 on the breakout board (GND-0V Pin, VCC-3V Pin, SCL-Pin 19, SDA-Pin 20). You now have the full wiring complete, it should look something like this:
<img width="1152" height="2048" alt="image" src="https://github.com/user-attachments/assets/1940559a-a15d-4510-b3d9-c7ba3aa3b596" />
<img width="1152" height="2048" alt="image" src="https://github.com/user-attachments/assets/e45c6261-2fbb-44f3-9319-487a4a172c30" />
<img width="1152" height="2048" alt="image" src="https://github.com/user-attachments/assets/595180a2-32a8-40dc-be80-e4137b3cc378" />
heres the wiring in kicad:
<img width="610" height="611" alt="image" src="https://github.com/user-attachments/assets/ef7cf460-dd01-4c0f-a92f-7456d9355a56" />


-Building Scaredy pants lite: Scaredy pants light consists of two components so assembly isnt as complicated as with scaredy cat. First of all print out both parts ,the bottom piece will come with lots of support struction so make sure to clean up the bottom piece. Add all the electronic gubbins and as said earlier, make sure to put the display through the hole and then spush the halves together. After that is done grab a nut and bolt(4.8mm) and put the bolt through the holes on top of both parts, then secure the bolt ith the corresponding nut do make sure eveything stays secure. 
Here is the onshape link for the 3D-Models:
https://cad.onshape.com/documents/d5f36c360309d0da1d068bf0/w/6ce9dd0b48870b7baf7f1960/e/e9c37b9101531aa43c0be3fa 

-Building Scaredy Cat: To start off print all three components for Scaredy Cat, the backpack component will also need to be cleared of any suport structure after printing. Then start with using a hot glue gun to glue the back pack and middlepart together where the hole on the middle piece is. Then gently place in the electronics.
<img width="883" height="698" alt="image" src="https://github.com/user-attachments/assets/2b5babd3-4cad-480d-a1d9-31b0a9a307af" />
Here is the onshape links for the 3D-Models: https://cad.onshape.com/documents/16606e79f902fc667de6f470/w/4e756a9daed502361049022d/e/c285e2ff7c10394a9b17194a https://cad.onshape.com/documents/22ab5850517fe45a945864af/w/b4afa80b39f69592a3dc5f3d/e/4521a73d3c30c847e517c37a


Next up is the front and middle sections of scaredy cat. First of all put the display through the face hole as done last time and after that start lining up the layers. You will notice the holes that line up between the two layers. Those holes are where we again use a nut and bolt system to keep everything together, but this one requires 4 nuts and 4 bolts(25mm). Put one of each in each hole and secure them tightly so everything stays solid. Now you have a complete Scaredy Cat!

# BOM
|name|description|price (for units)|Link|
|----|-----------|----------------|------|
|Microbit V2| A BBC Microbit V2| $ 6.45 (after tax)|https://nl.aliexpress.com/item/1005007470248064.html?pdp_npi=6%40dis%21EUR%215.62%211.80%21%21%2142.64%2113.64%21%40210152bd17819748977125334e1121%2112000040896298651%21affd%21%21%21%211%210%21&dp=CjwKCAjw9NjRBhATEiwA_p2J8Xh6WZwRcxxEfUnc5VWsoVIDvVJGWlRVSv8nMqQqzWMYimYcl1dutxoCTw4QAvD_BwE&cn=nlcluster&gad_source=1&gad_campaignid=22785620612&gbraid=0AAAAADihhqX8ySTauwRgni8OKGdHudEYT&gclid=CjwKCAjw9NjRBhATEiwA_p2J8Xh6WZwRcxxEfUnc5VWsoVIDvVJGWlRVSv8nMqQqzWMYimYcl1dutxoCTw4QAvD_BwE&aff_fcid=597aa878b6ee4c679be5a249f945e7dc-1782008874614-04027-_oEmQFg2&aff_fsk=_oEmQFg2&aff_platform=api-new-product-query&sk=_oEmQFg2&aff_trace_key=597aa878b6ee4c679be5a249f945e7dc-1782008874614-04027-_oEmQFg2&terminal_id=ffcfbaa5762d42198e2ab7016699e974&afSmartRedirect=y|
|ER_OLEDM0.91_1x-I2C| ssd1306 OLED display 32*128 0.91 inch| $ 4,24 (after tax)|https://nl.aliexpress.com/item/1005006782987637.html?src=google&src=google&albch=shopping&acnt=494-037-6276&isdl=y&slnk=&plac=&mtctp=&albbt=Google_7_shopping&aff_platform=google&aff_short_key=UneMJZVf&gclsrc=aw.ds&albagn=888888&ds_e_adid=&ds_e_matchtype=&ds_e_device=c&ds_e_network=x&ds_e_product_group_id=&ds_e_product_id=nl1005006782987637&ds_e_product_merchant_id=5762056048&ds_e_product_country=NL&ds_e_product_language=nl&ds_e_product_channel=online&ds_e_product_store_id=&ds_url_v=2&albcp=19213834753&albag=&isSmbAutoCall=false&needSmbHouyi=false&gad_source=1&gad_campaignid=17347463210&gbraid=0AAAAADznYb_UCRhPgM0kpv_taXeB_1UrA&gclid=CjwKCAjw9NjRBhATEiwA_p2J8SLELJ-GnFUkK783OCQHPe7IbFU34cyp3ij3iESXIwvzLFAdZyFedBoCdBwQAvD_BwE|
|Kitronic 5601B|BBC Micro:Bit Edge Connector Breakout Board| $3,38 (after tax)|https://www.sossolutions.nl/edge-connector-breakout-board-voor-bbc-micro-bit-kit?gad_source=1&gad_campaignid=17427468956&gbraid=0AAAAADkUwAWidxhgnEWcLnCvKilSuYwfB&gclid=CjwKCAjw9NjRBhATEiwA_p2J8eGiMncLqHLumHqC9wbWZzyZ4XnbLl_8MYP_bzrW61ABCLi50wZUaxoCdqsQAvD_BwE|




