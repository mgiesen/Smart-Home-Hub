# Smart Home Hub
The Smart Home Hub is a simple and lightweight plattform to remote control 433 MHz devices using a mobile device like a smartphone or a tablet. The Hub is designed to be very cost efficient and open source. The overal material costs are smaller than 10 USD. This enables a simple way to get startet with a smart home. Initially I designed the system around 2015 because of the high costs and rare availability of commercial solutions. After a couple of years I switched to the Homekit plattform to devote myself to new projects. I think meanwhile 433 MHz is outdated, but its still fun to play around and get an basic understanding of radio transmission. Hopefully the project helps you on your journey of development. 

![Project Overview](/Images/overview.png "Project Overview")

### Casing
The original case design was a little more basic to enable injection molding, but since I decided to not commercialy produce the device, I changed the casing a little bit for an special look. 
![Casing](Images/casing.jpg "Casing")

### Inside Look
In addition to smaller IC's, the PCB contains the follwing modules which are widely available on the market
- ESP8266 12E
- ISM Sender 433 MHz (FS1000A)
- ISM Receiver 433 MHz
![Inside Look](Images/inside_look.jpg "Inside Look")

### Casing lid
The lid consists of two parts, which are glued together, to prevent support structures while 3D printing
- The lid is locked by four screws on the site
![Casing lid](Images/open_lid.jpg "Casing lid")

### Backview
- Push button for hard reset
- USB Type B Connector for data transmission and powering
- Indication RGB LED
![Backview](Images/backview.jpg "Backview")

### PCB Design
I realised that many RGB LEDs sharing the same pin-layout, but the one half is using a common anod, the other half a common cathod. Because I wanted to use both, as long as I have them in storage, I designed the circuit with a variable tracing possibility, where you either can connect GND or 3,3V to the LED. I did without differnt series resistors, to save material costs and soldering time.
![PCB Layout](Images/pcb_layout.png "PCB Layout")
![PCB 3D](Images/pcb_rendering.jpg "PCB 3D")

### Software
To enable a good availability, the UI is served as a webapp, stored on the ESP8266. Every modern Browser can open the interface, as long its connected to the local wifi. To setup the Smart Home Hub, there is an captive portal to enter the wifi credentials. For design reasons I implemented an solution, but there are planty very good librarys for that. 
![Webapp](Images/webapp.jpg "Webapp")

### Assembling 
[![Assembling Video](Images/youtube.jpg)](https://www.youtube.com/watch?v=qMJYErCeu4k "Assembling Video")

### Parts
![Parts](Images/parts.jpg "Parts")

### Disclaimer
I didnt started the project with publishing it to the public in mind, so probably the documentation is not perfect. Also I am neither specialized in C++ nor in Electronics. So every recommendation is welcome and feel free to improve the software as well as the design. Meanwhile I am more than five years ahead and would probably do many things very different than shown. If there a good community improvements to the project, I will publish them, but I dind't plan to further work on the project for my own. 

I hope you liked the small overview and can use the information for your own work

Cheers
Max
