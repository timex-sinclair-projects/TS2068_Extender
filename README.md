# TS2068 Extender
Expansion bus PCB for the Timex Sinclair 2068

This expansion bus gives you four slots and a pass through connector. 

## Power

The expansion bus can be powered from the TS2068, an external 5 volt power supply or both.

Each slot and the pass through connector has a jumper that you can use to select the power source (TS or external 5v).

Each slot also has a jumper to allow for passing the /BE signal forward to the device in next lower slot number (ie, from slot 2 to slot 1) 
via the BUSISO pin. For devices that use /BE and recognizes the BUSISO pin going low, the device in the lower slot number will avoid
asserting /BE.

## Assembly

1. Start with the lowest profile components: the resistors and power diode (D1). The resistors have no orientation but the white band of D1 aligns with the white band on the circuit board.
2. Next, solder in the LED. The LED has a flat face that aligns with the flattened side of the LED symbol.
3. Solder the jumpers in next. The easiest way to do this may be to insert all the jumpers, place a bit of 
stiff foam or cardboard over them, invert the board (using the foam or cardboard to hold the jumpers in), 
place it face down on the table and solder 1 pin of each jumper. Next, check each jumper to ensure it's
properly soldered and vertical, then solder all the remaining pins.
4. Solder the relay and power connector. The jack side of the power connector should face the external edge of the PCB. The relay has a pin layout that fits in the PCB in only one way.
5. Insert and solder all 4 sockets next. The foam or cardboard may come in handy for these.
6. The last step is the most challenging: soldering the edge connector.
   a. Holding the edge connector with both hands and the pins facing away from you, place it on a hard surface at a low angle.
   b. Press down firmly to bend all the pins on one side and rotate the connector away from you. Your goal is to bend all pins on one side inward.
   c. Flip the connector and do the same. Ben from ByteDelight does this in one of his videos, here: https://www.youtube.com/live/ftt2_SxY5t8?si=WbfHqXK8gkp224uI&t=9232
   d. You should have a gap between the pins slightly less than the thickness of the board. Either slide it on from one side (sort of like a zipper) or wiggle it on like Ben does in his video.
   e. Double-check to ensure the connector is parallel to the PCB, solder just one pin and check again that it's still parallel. If not, heat up the pin and align.
   f. Solder all remaining pins of the connector.
7. If you plan to use a TS Pico with the board, move the Bypass jumper for Slot one so it's just on one pin.
8. Plug just the board in to your TS 2068, turn on the power and confirm the computer boots correctly and the LED on the expansion bus lights. If not, power off the computer, remove the expansion bus and confirm the TS 2068 works properly, then double-check all your solder connections.
