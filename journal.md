---
title: "C type HUB"
author: "sharanya"
description: "A hub with 2 * usb A and 2* c type"
created_at: "2025-07-5"
Total time spent: 6 hours
---



## JULY 5th morning:


![image](https://github.com/user-attachments/assets/bd3c744b-49d9-4c99-aa20-f391b7670cb6)


The first hour was spent planning out what I wanted to build. After facing the issue of limited USB ports on laptops and Raspberry Pi boards, I decided to create my own USB hub using a Type-C input and multiple USB A outputs. I went through the GL850G datasheet and USB switch ICs to understand their working and pin configurations. Once I was clear on how the hub controller communicates and distributes the signals, I moved on to schematic design in EasyEDA.


![Screenshot 2025-07-06 190643](https://github.com/user-attachments/assets/3260fa5b-1b80-4abb-92d1-d9b7f883a82e)



he second hour was completely dedicated to drawing the full schematic. I placed the main GL850G controller in the center and routed the USB D+ and D− lines carefully from the input to the controller and then from the controller to four USB output ports. I also added ESD protection using TVS diodes and designed the power rail distribution from the VBUS line. LEDs were added to indicate power status and port activity. Proper pull-up and pull-down resistors were used where necessary as per the USB specification. At the end of this hour, the schematic was complete and checked for ERC errors.

![image](https://github.com/user-attachments/assets/40939303-b1ff-41c1-bee2-df7082a54e31)



In the third hour, I started converting the schematic to PCB layout. This took a bit longer than expected because of the tight spacing and the requirement for short, straight differential pairs. I routed all USB traces keeping in mind the impedance matching and kept all traces as short and direct as possible. I also made sure the 5V and ground lines were thick enough to carry the current. Most components used are SMD to save space and make the board more compact. This was a bit tricky, but it gave me good practice with precise component placement.



![image](https://github.com/user-attachments/assets/99de0c8b-337c-4bab-b96e-14af99dddcd9)



In the fourth hour, I finalised the PCB dimensions and shape. I wanted a cool-looking board, so I made a rounded rectangle of about 65 mm by 34 mm, which fits easily in a pocket-sized enclosure. Then I added some graphics on the silkscreen layer . Mounting holes were also added to support enclosure fitting later. Once everything was double-checked, I ran the DRC and fixed a few spacing issues between traces and vias.



![image](https://github.com/user-attachments/assets/6ad5306d-8299-453c-a531-32711bd9783e)

![image](https://github.com/user-attachments/assets/80f40d07-ec75-4fd7-8ebb-86b9c379bf1f)


The fifth hour was used to generate the 3D view of the PCB and export the Gerber files. I also imported the board into the 3D enclosure designer and started working on the top and bottom case. The cutouts were made for USB ports and screws. I visualized the final product using the 3D viewer and it came out really well. It gave a clear idea of how the PCB will sit inside the enclosure and how all components will align.


![image](https://github.com/user-attachments/assets/b428395b-20d8-4864-9e74-4501233208da)



![image](https://github.com/user-attachments/assets/7b0a1b6a-a4d6-4b04-b7bc-a9607d8a921e)



Finally, in the sixth hour, I prepared all the files for fabrication and saved the project. I noted the BOM, double-checked component footprints, and got everything ready to be sent for PCB printing and enclosure manufacturing. Overall, this mini-project helped me apply my circuit theory knowledge, practice PCB layout skills, and understand real-world challenges like USB routing and signal integrity. It was an exciting and satisfying project to complete in such a short span of time.


