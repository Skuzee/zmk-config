# 3_8th ortho keeb  
Wireless Bluetooth, RGB, 18650 powered, USB C, 39 key, ortho mechanical keyboard.  
39 keys is exactly 3/8ths of a full 104 key keyboard.  
  
<img src="/pics/0-keyboard.jpg" width="800" />  
When I set out to build a custom keyboard, my original inspiration was that it would be a work of art as much as it would be a functional keyboard. Early designs were handwired and consisted of many layers of laser cut acrylic that sandwiched the wires in place. I wanted it's construction to be as much a feature as anything else.  
The original schematic used MAX7219 8-segment display driver chips to address 4 pin LEDs. I soon realized, with that many connections per key, a hand wired approach would not be feasible. I swapped the LEDs to SK6812 MINI-E RGB ( WS2812B) rear mount SMD addressable leds and moved my design into Kicad.  
<img src="/pics/1-all-parts.jpg" width="800" />  
Here are all the components layed out. (The 3D printed case is not the final design at this time.)  
<img src="/pics/2-switch-matrix.PNG" width="800" />  
Very standard switch matrix with ortho layout and a single key missing. This will be my Space and Enter key. Or, a double Spacebar depending on layout.  
<img src="/pics/3-RGB-LEDs.PNG" width="800" />  
This is the bus of addressable RGB LEDs with a 300ohm resistor to cut down on noise.  
<img src="/pics/4-power-circuit.PNG" width="800" />  
I knew from the beginning that I wanted this to be a wireless battery powered keyboard. Since each LED could draw 60mA each I knew I had to size my power traces and power supply accordingly! Because of this constraint the LEDs are powered from the battery via the external Pololu U3V70F5 step-up regulator.  
<img src="/pics/5-micro-controller.PNG" width="800" />  
The Nice!Nano is a promicro replacement that supports bluetooth, customizable zmk firmware, and 500mA battery charging and protection.  
<img src="/pics/6-combine-pcb.PNG" width="800" />  
Routing all the traces while staying within acceptable distances from other traces and holes was the biggest difficulty while designing the PCB layout.  
<img src="/pics/7-front-pcb.PNG" width="800" />  
   
<img src="/pics/8-rear-pcb.PNG" width="800" />  
   
<img src="/pics/9-top-pcb.jpg" width="800" />  
Here is the populated PCB  
<img src="/pics/10-bot-pcb.jpg" width="800" />  
   
<img src="/pics/11-lasercut-frame.jpg" width="800" />   
Each panel of the laser cut frame was a double-sided operation; with indents to embed keys into the surface. This gives a final lower profile, while accounting for the difference between key-height and the acrylic material thickness.  
<img src="/pics/12-lasercut-frame-close.jpg" width="800" />  
  You can see the reliefs for the keys, key retaining latches, and diode legs.  
<img src="/pics/13-frame-pcb-case.jpg" width="800" />  
  PCB loosely assembled in the frame and case.  
<img src="/pics/14-keys-installed.jpg" width="800" />  
  All key installed.  
<img src="/pics/15-rgb.jpg" width="800" />  
  RGB test!  
<img src="/pics/16-rgb.jpg" width="800" />  
 
<img src="/pics/17-rgb.jpg" width="800" />  
