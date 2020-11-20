# Headphone-PCB
This is a pcb, that was kindly provided by a user of my Tonuino-fork. It makes use of a DAC named 'PCM5102A' with a TDA1308 as amp. PCM5102A supports I2S, so it can connected in parallel to MAX98357a to the I2S-pins BCLK, LRC and DIN. Of course, it needs 3.3V and GND, too. Please note that SMD-technique is used. <br />
The 6th pin of connector J1 is used to indicate whether there's a plug or not. That means if there is a plug, this pin is pulled to GND and therefore can be used to connect to MAX98357.SD. Doing so will mute MAX's amp and vice versa. Off course you need a special [headphone jack](https://www.conrad.de/de/p/cliff-fcr1295-klinken-steckverbinder-3-5-mm-buchse-einbau-horizontal-polzahl-3-stereo-schwarz-1-st-705830.html) to use this feature. Additionaly this 6th pin can be connected to the ESP32 in order to make use of the feature `HEADPHONE_ADJUST_ENABLE`. Doing so can optionally limit the headphone's maximum volume (configureable via GUI). <br />

## Disclaimer
PCB-circuit is provided 'as is' without warranty. As previously stated it was kindly provided by a user and I only can give limited support to it. However: it runs fine without any problems in my Tonuinos.