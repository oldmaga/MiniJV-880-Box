# MiniJV-880-Box
STL files and hardware notes for my personal MiniJV-880 box build.

<img width="1920" height="1080" alt="WhatsApp Image 2026-05-16 at 18 43 58" src="https://github.com/user-attachments/assets/e0f8f6c8-fe35-49dc-b129-ddc66eb776ce" />

This repository is dedicated to the mechanical and hardware side of the project:

- printable STL files for the enclosure panels and internal holders;
- notes about the box, display, DAC, MIDI interface, encoder, buttons, SD extension and rear-panel connectors;
- general references for the components I used.

This repository does **not** contain the MiniJV880 software/firmware source code, Roland ROMs, SR-JV80 content, SysEx sound banks, CardRAM images, or any other Roland copyrighted sound material.


## Related repositories

- Hardware box / STL files: https://github.com/oldmaga/MiniJV-880-Box
- Software / CardRAM public source snapshot: https://github.com/oldmaga/MiniJV880-CardRAM-public

This repository contains the hardware box/STL side of the project.  
The MiniJV880-CardRAM-public repository contains the public-clean software/CardRAM source snapshot.

## Software

The software/firmware part is maintained separately.

Software repository:

https://github.com/oldmaga/MiniJV880-CardRAM-public

The software repository contains a public-clean source snapshot, documentation and tools that can be shared safely.

It does not include:

- Roland JV-880 ROM/NVRAM files
- SR-JV80 expansion images
- PN-JV80 SysEx files
- RD-500 files
- CardRAM images containing sound data
- compiled firmware images
- ready-made SD-card images


## Hardware notes

Hi everybody,

since someone asked, I thought I'd share files and notes from my very personal version of MiniJV-880 boxing. Please take them as they are: imperfect and largely editable. Think of them as a blueprint for creating your own version, which I'm sure will be a lot better.

Do not hesitate to contact me for any doubts and/or suggestions.

And above all, have fun!

For the project I used a metal box found on AliExpress: 220 x 80 x 195 mm. I replaced the front and rear plastic panels with two specially designed ones, available in the STL folder. I also printed the various supports for the hardware components, which in this case are:

- display: Surenoo SLC2402A with IIC module;
- DAC: PCM5102 I2S;
- MIDI Shield: basic Cominmark MIDI Shield;
- rotary encoder: KY-040;
- "T" shaped GPIO expansion board.

The Raspberry Pi used in this build is an RPi 4 already inserted in a metal case. Its plastic support is designed to keep it close to the metal box, helping cooling without installing a fan.

Be careful: this support is not suitable for a bare Raspberry Pi without its own case, because the board could come into contact with the metal box.

The front panel includes slots for fixing the display and the button panel. I could not find a ready-made button panel I liked, so I made one myself. For this reason, the support dimensions and especially the button grid will probably need to be adapted to the specific button panel used in your own build.

I used leftover components from other projects, essentially a perfboard onto which I soldered the buttons. On top of the buttons I applied the labels, then closed them with transparent key covers. The holes in the grille are about 0.1 mm larger than the buttons on each side.

All buttons have one common terminal connected to ground, so there are 13 wires in total. From the keyboard they go to a support PCB equipped with a PCB edge connector, mounted above the supports that fix the keyboard to the front panel.

The front panel also includes:

- the audio output, using a 3.5 mm stereo minijack;
- the hole for the rotary encoder;
- an SD-card extension, useful to remove the card after the box is closed.




On the rear panel there are:

<img width="2040" height="1530" alt="WhatsApp Image 2026-05-16 at 18 40 53" src="https://github.com/user-attachments/assets/ceb0c5f2-1787-496b-a62f-951b46a7f953" />

- mini USB for power;
- one USB connector, mainly used as an additional MIDI connection;
- one network socket;
- MIDI IN, OUT and THRU ports
- one mini usb-serial port for logging (last added, not yet in the STL files).

For the MIDI ports I soldered three pieces of MIDI cable to the Cominmark board and inserted their 5-pin DIN male connectors into the panel sockets.

To avoid making every single connection by hand, I used extension cables to connect the Raspberry Pi ports to the rear panel. This is fast, easy and less error-prone. You will find some search keywords for these parts below; on AliExpress there are many equivalent models.

Finally, I added a link to the SketchUp model I used to draw everything. I know SketchUp is not the best CAD tool, but for my purposes it was good enough. Use the model as an overall reference for the parts.

In the SketchUp model:

- purple, green and gray parts are the parts to print;
- yellow parts are dimensional references for the box and the components to be housed.

Well, that's pretty much it.

Let me know if there are any problems.

Bye.

## SketchUp model

https://app.sketchup.com/share/tc/europe/rp3Lkhn_vkg?source=web&stoken=tq2dXMXPWeA5VtgYNlE1SekmQYrnYpZajxxdF6qekr3p-wGEgr8Ih1lfUC_PohOD

## Component search keywords

Some useful AliExpress/Amazon search keywords:

- Box: `BDA 40007 -A2-W195`, 220 x 80 x 195 mm
- Display: `Surenoo 242 24X2 2402 LCM`
- DAC: `I2S PCM5102A`
- MIDI interface: `MIDI Shield`
- MIDI sockets: `avssz d-type din conference midi module`
- Audio socket: `22 cm DC3.5mm TRS`
- SD extension: `mini sim card extension`
- USB extension: `D-type Car Chassis Front USB3.0 Panel Installation`
- Ethernet extension: `ethernet cable panel extension`
- Buttons: `Microswitch A14 A24`
- Log system:  Mini-USB serial adapter FTDI FT232-AZ
  
