# MiniJV-880-Box
STL files and components

Hi everybody,
since someone asked, I thought I'd share files and notes from my very personal version of MiniJV-880 boxing. Please take them as they are: imperfect and largely editable. Think of them as a blueprint for creating your own version, which I'm sure will be a lot better.
Do not hesitate to contact me for any doubts and/or suggestions.
And above all, have fun!


For the project I used a metal box found on AliExpress (220x80x195mm). I replaced the front and rear plastic panels with two specially designed ones (see STL file).  I also printed the various supports for the hardware components, which in this case are:

- display: Surenoo SLC2402A with IIC module
- DAC: PCM5102 I2S
- MIDI Shield: a banal Cominmark
- Rotary encoder: KY-040
- "T" shaped GPIO expansion board.

The Raspberry used (Rpi4) was already inserted in a metal box: its plastic support is designed to keep it adherent to the metal of the box and thus contribute to its cooling without having to install a fan. Be careful, this support is not good if you use an Rpi without a container because it could come into contact with the metal of the box.

The front part is equipped with slots for fixing the display and button panel. Unfortunately I couldn't find a ready-made one that I liked so I preferred to make it myself, so the dimensions of the supports and especially of the grid will have to be modified based on the size of the button panel you will use.

I used leftover components from other projects, essentially a perfboard onto which I soldered the buttons. On top of these I applied the writing, then closed with transparent key covers. the holes in the grille are larger than the buttons by about 1 tenth of a millimeter per side (I added below the reference for the buttons used).
All the buttons have a common terminal connected to ground, so there are 13 wires in total, and from the keyboard they go to a support PCB equipped with a PCB edge connector, mounted above the supports that fix the keyboard to the front panel.
I used leftover components from other projects, essentially a perfboard onto which I soldered the buttons. On top of these I applied the writing, then closed with transparent key covers. the holes in the grille are larger than the buttons by about 1 tenth of a millimeter per side (I added the reference for the buttons used below).
All the buttons have a common terminal connected to ground, so there are 13 wires in total, and from the keyboard they go to a support PCB equipped with an edge Connector PCB, mounted above the supports that fix the keyboard to the front panel.
Finally, on the front panel there are the audio output (3.5 stereo minijack), the hole for the Rotary Encoder and an extension for the SD slot, to conveniently remove the card once the box is closed.

On the rear panel there are the mini USB (power), a USB (which I mainly use as an additional MIDI connection) and a network socket, plus the three IN, OUT and THRU ports on which I soldered three pieces of MIDI cables, inserting their 5-pin DIN male connectors into the Cominmark sockets.
To avoid having to make every single connection by hand I simply used extensions cables to connect the Rpi ports to the rear panel: fast, easy and error-proof.
Again, you will find the references for these extensions at the end; on AliExpress there are hundreds of different models.

Finally, I added a link to Sketchup, which I used to draw everything.
Yes, I know it's not the best for CAD but for my purposes it's good enough... Use it to have an overall reference of the parts. The ones to print are the purple, green and gray ones. The yellow parts are dimensional representations of the box and the components to be housed.

Well, that's pretty much it. Let me know if there are any problems.
Bye




Link to Sketchup Model:
https://app.sketchup.com/share/tc/europe/rp3Lkhn_vkg?source=web&stoken=tq2dXMXPWeA5VtgYNlE1SekmQYrnYpZajxxdF6qekr3p-wGEgr8Ih1lfUC_PohOD


Here some keyword search on AliExpress

- Box: BDA 40007 -A2-W195, 220x80x195mm
- Display: Surenoo 242 24X2 2402 LCM
- Dac: I2S PCM5102A
- MIDI interface: MIDI Shield


- Midi sockets: avssz d-type din conference midi module
- Audio socket: 22 cm DC3.5mm TRS
- SD extension: mini sim card extension
- usb extension: D-type Car Chassis Front USB3.0 Panel Installation
- Ethernet extension: ethernet cable panel extension
- Buttons: Microswitch A14 A24

