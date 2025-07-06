# C_HUB

Hey there! This is a custom-designed USB C-Hub project made completely from scratch using EasyEDA. The idea behind this was to create a compact, multi-port USB hub which can be used with Type-C connectors for expanding the number of USB ports available on laptops or Raspberry Pi boards, which usually have limited USB slots. The project mainly includes USB switch ICs and a USB 2.0 hub controller (GL850G), which is the heart of the setup. I tried to keep the schematic clean and modular with proper grounding and bypass caps for each IC to reduce noise and improve stability. There are multiple USB A ports as output, and a single Type-C port as input, and I’ve used ESD protection diodes to avoid damage from surges.

![Screenshot 2025-07-06 192308](https://github.com/user-attachments/assets/0f83a496-f528-4a3e-aac5-8acc9ad742e6)


![image](https://github.com/user-attachments/assets/78b11d91-13f6-47e7-a67e-306d65a0e0a3)


Designing the PCB was quite fun and a bit challenging. I went for a two-layer board and made sure the traces were short and direct, especially for high-speed USB data lines. I also added some personal touch by placing a fun logo and text on the silkscreen layer because why not? The final board is 64.77mm by 34.16mm and has mounting holes for easy fitting into an enclosure. Most components are SMD to keep the form factor low and the layout tight. This project helped me learn a lot about USB routing, grounding techniques, and schematic management in EasyEDA. Planning to get this printed soon and see how it performs in real-world usage. Hope you liked the design!


![Screenshot 2025-07-06 192323](https://github.com/user-attachments/assets/36dd48fd-4cff-47ba-9bec-c72041857613)

![image](https://github.com/user-attachments/assets/82583704-14c2-4f06-a267-2c5182e1b848)

