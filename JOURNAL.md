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

## 1 hour

# Day 2: Deciding parts and starting the PCB schematic
## 11/22/2025
Today I did a lot of research on the components and I decided on using the STM32F072CBT6 as my main control unit for the keyboard as it was plenty of GPIO pins and more than enough processing power for a keyboard. Then to run the hubs and display, I will use a raspberry pi 2 to handle that. Using https://www.keyboard-layout-editor.com/#/ I generated my keyboard outline with dimensions to guide my PCB.

![Screenshot 2025-11-22 at 1](https://github.com/user-attachments/assets/244c4641-7236-4793-9c37-806ae27f0e5a)

This was my first time using KiCAD so I spent a lot of time on research, today I was only able to wire the schematic for the MCU

![Screenshot 2025-11-22 at 9](https://github.com/user-attachments/assets/5d35bdce-2ea0-486d-805c-ab2b8b084c36)

I found this guide here that was very useful for learning keyboard design and KiCAD: https://www.youtube.com/watch?v=8WXpGTIbxlQ&list=PLBD2IS_t_iWZDMdG_ZF57x9Ebm3kxKqxF&index=3

## 4.5 hours
