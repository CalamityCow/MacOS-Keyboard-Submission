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
