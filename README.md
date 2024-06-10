# FB2-Schematic
This repository contains a schematic of the Atari Flashback 2. It was created by reverse engineering a revision C board. Other board revisions will likely have some small differences. 

Some notes:
* The capacitance of the surface-mount capacitors was left blank. I could've measured them, but it would require removing them from the circuit to isolate them from other components, and I didn't think it was worth the time.
* Some unpopulated components are shown shorted on the schematic. This is because some of the components have a trace connecting their pads. Presumably, this was to save a few cents over using 0Ω resistors while still allowing other components to be installed there if the traces are cut first.
* There are several nets that carry 3.3V and GND. This is because it is a single-layer board, so jumpers were used all over the board as bridges over other traces. 3.3V and GND nets are named after the jumper they are connected to that connects towards their source. For example "+3V3_J13" is the 3.3V net after passing over J13. 
