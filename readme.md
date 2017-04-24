[Version française / French version](https://github.com/madnerdorg/buzzer/blob/master/readme.fr.md)  

Buzzer is a device based on an Arduino nano to control a buzzer using [https://github.com/madnerdorg/libreconnect](libreconnect)   
**Warning: This application should be considered alpha, and could not work correctly.**      

![Midi Buzzer](https://github.com/madnerdorg/buzzer/raw/master/doc/thumbnail_buzzer.png)  

# Usage 
## Midi Keyboard

* Plug your **MIDI keyboard**.
* Go to http://madnerd.org/interface/midi ## Midi Software
You can compose music that will be played by the buzzer.    

### LoopMidi 
![LoopMidi Add Midi Port](https://github.com/madnerdorg/buzzer/raw/master/doc/loopMidi.png)     
We are going to use loopMidi to generate virtual midi port on Windows.
* Download : [loopMidi](http://www.tobias-erichsen.de/software/loopmidi.html)
* Click on **+** to create a virtual midi port

### LMMS
Examples are available in **lmms/** 

![buzzer on LMMS](https://github.com/madnerdorg/buzzer/raw/master/doc/buzzer_lmms.png)
* Download **LMMS** : https://lmms.io/download/#windows
* On **TripleOscillator** put the volume to 0
* Click on the gear next to **TripleOscillator**
* Click on Midi and choose your **virtual midi port** (**Loopmidi by default**) ## Commands
* /info --------> Display name:port    
* X -------> Where X is the frequency in hz
* OFF -------> Stop sound    

# Components
* Arduino nano CH340G: 2€    
* 10 Buzzer : 1.80€  (1 Buzzer:0.18€)  
* Resistor pack 400pcs (3€) (1 resistor: 0.0071€) 
* 5 pcs stripboard (1.18€) (1 stripboard : 0.24€ )  
* Total : 7.98€ (2.43€)   

# Wiring
Don't forget to isolate the circuit from the arduino   
## Buzzer only 
![UBuzzer Wiring](https://github.com/madnerdorg/buzzer/raw/master/doc/buzzer_wiring.png)   
* Pin 9 : RESISTOR (100Ohm) --- Buzzer +   
* Pin 10 : Buzzer -    

## Buzzer/Led
You can add a led (**before the resistor**)
* Pin 9 : RESISTOR (100Ohm) --- Led + / Buzzer +   
* Pin 10 : Led - / Buzzer -    

# 3D Printing
This model is a **all purpose case** for arduino nano projects    
Models by Olivier Sarrailh : https://github.com/madnerdorg/buzzer/tree/master/3D    
**You won't be able to properly close the case as the buzzer takes too much place, but you should still be able to close it**

# Licences

# Buzzer.ino
* Author: Rémi Sarrailh (madnerd.org)   
* Licence: MIT

# ToneAC
* Author: Tim Eckel
* Licence : GNU GPL v3
* Link: https://bitbucket.org/teckel12/arduino-toneac/wiki/Home
* Donate : [PayPal](https://bitbucket.org/teckel12/arduino-toneac/wiki/Home#!show-your-appreciation)
