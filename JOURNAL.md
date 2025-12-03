# Total Time: 46.5 hours

# Day 1: Brainstorming and first concepts.
## 11/21/2025
Here is my starting idea:

<img width="819" height="365" alt="Screenshot 2025-12-02 at 10 30 39 PM" src="https://github.com/user-attachments/assets/9f7092bd-9d97-49eb-8789-fcaa36e199e7" />

- 100% mechanical keyboard
- Hot swappable
- LCD(probably to save cost) screen display
- 2 USB 3.0
- 2 USB C
- 1 microSD reader
- 1 ethernet port

I'd like to have an aluminum case for my keyboard but since it will likely have to be custom, I'm not too sure how to machine one. (Also it seems that nobody sells 100% shells anyways)

## 1.0 hour


# Day 2: Deciding parts and starting the PCB schematic
## 11/22/2025
Today I did a lot of research on the components and I decided on using the STM32F072CBT6 as my main control unit for the keyboard as it was plenty of GPIO pins and more than enough processing power for a keyboard. Then to run the hubs and display, I will use a raspberry pi 2 to handle that. Using https://www.keyboard-layout-editor.com/#/ I generated my keyboard outline with dimensions to guide my PCB.

![Screenshot 2025-11-22 at 1](https://github.com/user-attachments/assets/244c4641-7236-4793-9c37-806ae27f0e5a)

This was my first time using KiCAD so I spent a lot of time on research, today I was only able to wire the schematic for the MCU

![Screenshot 2025-11-22 at 9](https://github.com/user-attachments/assets/5d35bdce-2ea0-486d-805c-ab2b8b084c36)

I found this guide here that was very useful for learning keyboard design and KiCAD: https://www.youtube.com/watch?v=8WXpGTIbxlQ&list=PLBD2IS_t_iWZDMdG_ZF57x9Ebm3kxKqxF&index=3

## 4.5 hours


# Day 3: Finishing the Schematics and building the PCB
## 11/23/2025
After following the really nice guide I found, I was able to finish the schematic for all the modules. In total, I have:

MCU + Power supply

<img width="182" height="467" alt="Screenshot 2025-11-24 at 11 00 52 AM" src="https://github.com/user-attachments/assets/30148abd-b303-4c04-bbff-af80cfdfd860" />


Keyboard matrix

<img width="862" height="410" alt="Screenshot 2025-11-24 at 12 14 33 AM" src="https://github.com/user-attachments/assets/ff5456cd-8ca9-4f56-9764-71b982c43d50" />


LED panel

<img width="313" height="233" alt="Screenshot 2025-11-24 at 12 14 51 AM" src="https://github.com/user-attachments/assets/503b3c75-35be-44a5-9004-48d9811625ee" />

<img width="717" height="331" alt="Screenshot 2025-11-24 at 12 15 04 AM" src="https://github.com/user-attachments/assets/6fd4f486-3f05-4f80-9922-b2d06d1e448c" />

Volume Knob

<img width="388" height="419" alt="Screenshot 2025-11-24 at 12 15 19 AM" src="https://github.com/user-attachments/assets/bcf087fa-9632-42b9-b679-0dd803593827" />


After I used my keyboard layout to add the keys to the PCB

![Screenshot 2025-11-24 at 12](https://github.com/user-attachments/assets/e18ffa6e-4fdf-4e9a-80e0-a74a2a97d7fe)




Since the LCD screen is hooked up to a separate microcontroller, I think I will add it later as it is easy and modular to add.

## 9.0 hours

# Day 4/5: Routing the PCB
## 11/25/2025
I went on a flight so I couldn't really work on the project the left few days but I'm finally back. Today I started hooking up the switches on the keyboard and adding the LEDS in.

![1](https://github.com/user-attachments/assets/19dfa811-1722-4652-89b5-959f3ab7ff87)

My matrix routing is quite simple, but I took a bit of time to figure out the routing for LEDS as I had to try my best to avoid EMI. I think that this configuration for LEDS will work:

![2](https://github.com/user-attachments/assets/ca526f00-74a3-420b-a45a-306f0abe86e2)

Though it is a bit time consuming so it will probably take me two more days to finish the routing.

<img width="778" height="314" alt="3" src="https://github.com/user-attachments/assets/4997c56b-10bf-4854-9aa0-ad3b1434c879" />

Also, I decided to use a rotary encoder instead of a potentiometer for the volume knob as its probably easier to code later.

## 3.0 hours

# Day ???????: Finished the PCB!
## 11/30/2025
This is going to be a long one...
I did not do a single journal last week as I was on Thanksgiving break. Luckily between my time spent on airplane flights, car rides, and general downtime, I was able to put in an honestly absurd amount of time.

I decided that a screen + hubs is WAY too hard for my first project, so I will do them later as an add on.

For LEDS, I decided to switch from WS2812B to sk6812mini e because they are reverse mounted. Also I switched my diode placements to the top of the switches to allow for more space on my LED traces.

Speaking of LED traces, I must have messed this part up at least 3 times. First, I used the wrong footprint, then I accidently routed them all in parallel, before finally routing them together correctly.

Enough yapping here is my finished PCB:

![11](https://github.com/user-attachments/assets/72692c74-7883-4975-af0e-e6e49a6abacf)
![22](https://github.com/user-attachments/assets/8ed80b0f-74eb-44f2-821b-a5d6bce7bef4)
![33](https://github.com/user-attachments/assets/64a7cf29-b520-4ea7-81ac-5aee31389391)

And my schematics:

<img width="944" height="663" alt="44" src="https://github.com/user-attachments/assets/a54a2f0a-b5a4-4997-b2eb-cbf8d766b1d5" />
<img width="841" height="368" alt="55" src="https://github.com/user-attachments/assets/f3acc254-cc69-4e64-8445-5142664351d8" />

## 20.0 hours

# Day ???? + 1: Case design
## 12/1/2025
I made some minor changes to the model by making the fill zone look neater and putting components closer to the center of the board.

Making the case was quite easy because I generated my keyboard layout with a DXF file of the outline using these two links:
https://www.keyboard-layout-editor.com/
https://kbplate.ai03.com/

All I did was import the DXF as a sketch to Onshape then add 3 layers of offsets.

![1](https://github.com/user-attachments/assets/27b3ea1b-e7b4-420f-b60d-518094840aa0)

Next I extruded the plate and the casings.

![2](https://github.com/user-attachments/assets/2688c241-3504-4d91-9a78-a38104490ffa)

I decided to do a top mount design, and I will use some 3dp spacers to support my the pcb. (I dont think grip strength of the mounts is enough to hold the pcb)

![3](https://github.com/user-attachments/assets/16d63a8c-9900-4d54-82c0-31dd2dad5b04)

Finally on the bottom, I added an angle attachment and rubber stoppers. The idea is that the triangle is able to be changed so that I can 3dp many different angles to see what fits for me.

![4](https://github.com/user-attachments/assets/e14ad69d-61c1-45ec-bfa9-f6acf318c288)

As for the case itself I want it to be acrylic or aluminum, but I will 3dp the first few iterations with PETG so that I can get a good design first.

![5](https://github.com/user-attachments/assets/39e1924e-6451-4f9a-8671-fd4fddd1996a)

# 6.0 hours

# Finishing details on case + BOM
## 12/2/2025
Added a usb cutout for a usb wire.
<img width="570" height="339" alt="1" src="https://github.com/user-attachments/assets/a416a079-b0c3-48ee-b319-90594f622773" />


I also inserted all the needed bolts and nuts. Most of my holes will be tapped and then screwed together with a 0 80 screw. (I hate metric)

Finally I added the step file of my PCB to make sure everything will fit together.
<img width="1256" height="749" alt="2" src="https://github.com/user-attachments/assets/2e543afe-edb2-4bc2-aad6-50b105b0731d" />


Here is my BOM: https://docs.google.com/spreadsheets/d/1dYup_cxLSYAhRu9MLTjsDp3llwcmy9G50tkykbGbxao/edit?gid=810680966#gid=810680966

## 2.0 hours

# Quick Update
## 12/2/2025
CHANGED ALL THE HOLES BACK TO METRIC >:(
0 80 was WAYY to expensive
<img width="297" height="249" alt="Screenshot 2025-12-02 at 9 46 58 PM" src="https://github.com/user-attachments/assets/b2a93eb7-26ed-4b2a-8d73-c38cfd4428d7" />

I think changing my screws from 0 80 to M3 dropped the BOM cost by 20-30. Also I have random m3 screws at home and robotics lmao.
# 1.0 hour

As a quick sidenote I didn't realize I had to add a jornual markdown so as I was copying my jornual from the Blueprint website too here, I realize that I sound progressively more insane in each entry.
