# Multiple RFID Readers

This is a multiple RFID Readers system designed specifically for an Escape Room. The door will open after the 4 right cards(Tags) are read and recognized.

## Changes
This is a modification of https://github.com/Annaane/MultiRfid

The original code was not ideal for 2 reasons:
  1.  you could use the same tag on all readers one after the other and the door would open
  2. there was no association between reader and tag, so you could mix and match, often this is not what you want for an escape room.

In this version you need to associate the right tag with the right reader in order to unlock the door.

I tried to keep modifications to a minimum so you can compare it to the original code.
  


## Requirements :
   #### Hardware :
   * Arduino UNO.
   * 4 x MFRC522 RFID Reader Modules.
   * 13.56 MHz RFID key/card tags. 
   * Relay module.
   * Leds.
   * Jumper wires.
   * Push button (for manual opening).
   #### Software :
   * Arduino IDE.
   * Arduino [RFID Library for MFRC522 by miguelbalboa](https://github.com/miguelbalboa/rfid).     

## Functioning :
   * Green Led turns on when the door opens.
   * Red Led blinks slowly two times when system needs more tags (less than 4 cards).
   * Red Led blinks fast many times (4, maybe?) when the card isn't allowed.
   * A push button added for manual opening (intended for the cleaning staff).
   
 ## TL;DR?
 Do you want to **_see it_** working ? Check the video : https://www.youtube.com/watch?v=ahc8Yai_sWI
