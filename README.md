# MacOS-Keyboard-Submission

This project is just a simple MacOS keyboard, although honestly you can modify any keyboard to beomce a MacOS keyboard by changing its firmware. 
I started this project because I thought it would be fun to learn how to design a PCB and solder electronic components. While I'm mostly a software guy I've really wanted to learn the electronical side of things for a while now so after discovering blueprint I thought it would be a great idea to get some experience. I used a template from ScottoKeebs, which included the MCU and the power supply prewired.
## Features
The main features of this keyboard are:
- 95 keys
- 6 macro keys
- 101 per-key leds
- volume knob

Later on I want to try to add a LCD screen to the keyboard and some hubs.

# PCB and Schematic
The PCB and schematic were designed using KiCad. It is a standard 2 layer design.
<img width="1231" height="860" alt="Screenshot 2025-12-02 at 10 13 27 PM" src="https://github.com/user-attachments/assets/b6fd0765-321a-43fb-89dd-0f99de0ba42e" />
<img width="1289" height="497" alt="Screenshot 2025-12-02 at 10 13 40 PM" src="https://github.com/user-attachments/assets/3bf9ab96-46f8-4e74-a6c7-f35d646940f4" />
<img width="1567" height="570" alt="Screenshot 2025-12-02 at 10 13 53 PM" src="https://github.com/user-attachments/assets/56c31ab0-b220-40cf-a1c9-bc25208f7079" />
<img width="1607" height="639" alt="Screenshot 2025-12-02 at 10 14 31 PM" src="https://github.com/user-attachments/assets/b1076d44-ed21-4ffd-a124-611670982d90" />
<img width="1583" height="620" alt="Screenshot 2025-12-02 at 10 14 37 PM" src="https://github.com/user-attachments/assets/ca5fb593-0200-4b3c-bb74-bfd8fbf27943" />

Below is the case for my keyboard.
<img width="727" height="438" alt="Screenshot 2025-12-02 at 10 17 44 PM" src="https://github.com/user-attachments/assets/c327d89b-9a1f-4781-a55d-5044c5f52d18" />
<img width="1306" height="612" alt="Screenshot 2025-12-02 at 10 17 24 PM" src="https://github.com/user-attachments/assets/e0cd4ecb-c385-45a6-8425-582f296fcf7c" />

Onshape link: https://cad.onshape.com/documents/4c8306176f584344784f98ef/w/69e2811755be6605c0c07897/e/ae6883cfd18f4e06578fb81e

# Bom
BOM link: https://docs.google.com/spreadsheets/d/1dYup_cxLSYAhRu9MLTjsDp3llwcmy9G50tkykbGbxao/edit?gid=810680966#gid=810680966

[Uploading MacOS KeyboardLCSC Items,,,,,,,,,,,,
Index,LCSC#,MPN,Manufacturer,Package,Description,RoHS,Quantity,MOQ,Multiple,Unit Price($),Extended Price($),Product Link
1,C23733,CL05A475MP5NRNC,Samsung Electro-Mechanics,402,10V 4.7uF X5R ±20% 0402 Ceramic Capacitors RoHS,yes,50,50,50,0.0048,0.24,https://www.lcsc.com/product-detail/C23733.html
2,C2827654,USBLC6-2SC6,TECH PUBLIC,SOT-23-6,6A 12V 150W 6V Unidirectional 5V SOT-23-6 TVS Diodes RoHS,yes,10,10,10,0.0384,0.38,https://www.lcsc.com/product-detail/C2827654.html
3,C5446,XC6206P332MR-G,TOREX,SOT-23-3L,"Positive Fixed 3.3V SOT-23-3L Voltage Regulators - Linear, Low Drop Out (LDO) Regulators RoHS",yes,5,5,5,0.1033,0.52,https://www.lcsc.com/product-detail/C5446.html
4,C354152,SN74AHCT125N,TI,DIP-14,"1 4.5V~5.5V 4 DIP-14 Buffers, Drivers, Receivers, Transceivers RoHS",yes,1,1,1,0.684,0.68,https://www.lcsc.com/product-detail/C354152.html
5,C470754,EC11E15244B2,ALPSALPINE,Through Hole,Through Hole Encoders RoHS,yes,1,1,1,1.9975,2,https://www.lcsc.com/product-detail/C470754.html
6,C115351,SKQGABE010,ALPSALPINE,"SMD-4P,5.2x5.2mm","12V 5.2mm Round Button 5.2mm SPST 50mA SMD-4P,5.2x5.2mm Tactile Switches RoHS",yes,5,5,5,0.1076,0.54,https://www.lcsc.com/product-detail/C115351.html
7,C2073614,PNM0402E5000BST1,VISHAY,402,50mW 500Ω 75V ±25ppm/℃ Thin Film Resistor ±0.1% 0402 Chip Resistor - Surface Mount RoHS,yes,2,1,1,1.4497,2.9,https://www.lcsc.com/product-detail/C2073614.html
8,C25905,0402WGF5101TCE,UNI-ROYAL,402,5.1kΩ 62.5mW 50V ±100ppm/℃ Thick Film Resistor ±1% 0402 Chip Resistor - Surface Mount RoHS,yes,100,100,100,0.0005,0.05,https://www.lcsc.com/product-detail/C25905.html
9,C25744,0402WGF1002TCE,UNI-ROYAL,402,10kΩ 62.5mW 50V ±100ppm/℃ Thick Film Resistor ±1% 0402 Chip Resistor - Surface Mount RoHS,yes,100,100,100,0.0006,0.06,https://www.lcsc.com/product-detail/C25744.html
10,C165948,TYPE-C-31-M-12,Korean Hroparts Elec,SMD,"1 16P Type-C SMD USB, DVI, HDMI Connector Assemblies RoHS",yes,5,5,5,0.1752,0.88,https://www.lcsc.com/product-detail/C165948.html
11,C210357,MF-FSMF050X-2,BOURNS,603,6V 500mA 40A 1A 100mΩ 0603 PTC Resettable Fuses RoHS,yes,20,20,20,0.0359,0.72,https://www.lcsc.com/product-detail/C210357.html
12,C60474,CC0402KRX7R7BB104,YAGEO,402,16V 100nF X7R ±10% 0402 Ceramic Capacitors RoHS,yes,200,100,100,0.0009,0.18,https://www.lcsc.com/product-detail/C60474.html
13,C5149201,SK6812MINI-E,OPSCO Optoelectronics,SMD,"SMD LED Addressable, Specialty RoHS",yes,105,5,5,0.0683,7.17,https://www.lcsc.com/product-detail/C5149201.html
14,C52923,CL05A105KA5NQNC,Samsung Electro-Mechanics,402,25V 1uF X5R ±10% 0402 Ceramic Capacitors RoHS,yes,100,100,100,0.003,0.3,https://www.lcsc.com/product-detail/C52923.html
15,C15195,CL05B103KB5NNNC,Samsung Electro-Mechanics,402,50V 10nF X7R ±10% 0402 Ceramic Capacitors RoHS,yes,100,100,100,0.0014,0.14,https://www.lcsc.com/product-detail/C15195.html
16,C307331,CL05B104KB54PNC,Samsung Electro-Mechanics,402,50V 100nF X7R ±10% 0402 Ceramic Capacitors RoHS,yes,100,100,100,0.0038,0.38,https://www.lcsc.com/product-detail/C307331.html
17,C81720,STM32F072CBT6,ST,LQFP-48(7x7),ARM Cortex-M0 48MHz 37 LQFP-48(7x7) Microcontrollers RoHS,yes,1,1,1,1.3444,1.34,https://www.lcsc.com/product-detail/C81720.html
18,C84410,1N4148TR,onsemi,DO-35,4A 4ns 100V 1V@10mA 200mA DO-35 Single Diodes RoHS,yes,150,50,50,0.0155,2.33,https://www.lcsc.com/product-detail/C84410.html
19,C15008,CL31A107MQHNNNE,Samsung Electro-Mechanics,1206,6.3V 100uF X5R ±20% 1206 Ceramic Capacitors RoHS,yes,10,10,10,0.0552,0.55,https://www.lcsc.com/product-detail/C15008.html
Sub Total,,,,,,,,,,,21.36,
Shipping and Taxes,,,,,,,,,,,10,
Line Total,,,,,,,,,,,31.36,
,,,,,,,,,,,,
Mechincalkeyboards.com Items,,,,,,,,,,,,
Index,Manufacturer,Item,Quantity,Multiple,Unit Price($),Extended Price($),Product Link,,,,,
1,Kailh,Kailh Switch Hot Swap Socket,110,10,0.11,12.1,https://mechanicalkeyboards.com/products/kailh-switch-hot-swap-socket?variant=47416807194924,,,,,
2,Cherry,Cherry MX Silent Black 60g Linear Switch,110,10,0.5,55,https://mechanicalkeyboards.com/products/cherry-mx-silent-black-60g-linear?variant=47607467016492&country=US&currency=USD&utm_medium=product_sync&utm_source=google&utm_content=sag_organic&utm_campaign=sag_organic&srsltid=AfmBOoplOW0TOqYJWSCwaqFnCc0V0J1uw9Fu6u8llsd3mldauiAsW2AIT3Q,,,,,
Sub Total,,,,,,67.1,,,,,,
Shipping and Taxes,,,,,,0,,,,,,
Line Total,,,,,,67.1,,,,,,
,,,,,,,,,,,,
McMaster-Carr Items,,,,,,,,,,,,
Index,Manufacturer,Item,Quantity,Multiple,Unit Price($),Extended Price($),Product Link,,,,,
1,McMaster-Carr ,Adhesive-Back Polyurethane Rubber Bumpers,1 (pack of 72),1,4.77,4.77,https://www.mcmaster.com/95495K931/,,,,,
2,McMaster-Carr ,Uncoated High-Speed Steel Chip-Clearing Tap,1,1,13.94,13.94,https://www.mcmaster.com/3192N11/,,,,,
Sub Total,,,,,,4.77,,,,,,
Shipping and Taxes,,,,,,0,,,,,,
Line Total,,,,,,18.71,,,,,,
,,,,,,,,,,,,
JLC PCB,,,,,,,,,,,,
Index,Manufacturer,Item,Quantity,Multiple,Unit Price($),Extended Price($),,,,,,
1,JLC,PCB,1,5,62.9,62.9,,,,,,
Sub Total,,,,,,62.9,,,,,,
Shipping and Taxes,,,,,,0,,,,,,
Line Total,,,,,,62.9,,,,,,
,,,,,,,,,,,,
Grand Total,,,,,,180.07,,,,,,
Grand Total after 7.25% tax estimate,,,,,,193.125075,,,,,, - export_cart_20251203_102105.csv…]()
