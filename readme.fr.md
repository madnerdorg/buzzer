[English Version](https://github.com/madnerdorg/buzzer/)

buzzer est un appareil fait à partir d'un arduino nano pour contrôler un buzzer à l'aide de [https://github.com/madnerdorg/libreconnect](libreconnect)   
**Attention: Cette application est en alpha, et pourrait ne pas fonctionner correctement**      
![Midi Buzzer](https://github.com/madnerdorg/buzzer/raw/master/doc/thumbnail_buzzer.png)  
# Utilisation
## Clavier Midi
* Brancher votre **midi keyboard**.
* Aller sur [TODO]

## Logiciel Midi
Vous pouvez composer des musiques qui seront jouer par le buzzer.   
### LoopMidi
![LoopMidi Add Midi Port](https://github.com/madnerdorg/buzzer/raw/master/doc/loopMidi.png)     
Nous allons utiliser loopMidi pour générer des ports midi virtuels sur Windows.
* Télécharger: http://www.tobias-erichsen.de/software/loopmidi.html   
* Cliquez sur **+** pour créer un port midi virtuel

### LMMS
Des exemples sont disponibles dans **lmms/**

![buzzer on LMMS](https://github.com/madnerdorg/buzzer/raw/master/doc/buzzer_lmms.png)
* Télécharger **LMMS** : https://lmms.io/download/#windows
* Sur **TripleOscillator** mettez le volume à 0
* Cliquer sur la roue près de **TripleOscillator**
* Clicquer sur Midi et choissisez votre **port midi virtuel** (**Par défaut: Loopmidi**)

## Commandes
* /info --------> Affiche le nom:port    
* X -------> Où x est la fréquence en HZ.
* OFF -------> Arrête le son    

# Composants
* Arduino nano CH340G: 2€    
* 10 Buzzer : 1.80€  (1 Buzzer:0.18€)  
* Resistor pack 400pcs (3€) (1 resistor: 0.0071€) 
* 5 pcs stripboard (1.18€) (1 stripboard : 0.24€ )  
* Total : 7.98€ (2.43€)   

# Branchement
N'oubliez pas d'isoler le circuit de l'Arduino  
## Buzzer seul
![UBuzzer Wiring](https://github.com/madnerdorg/buzzer/raw/master/doc/buzzer_wiring.png)   
* Pin 9 : RESISTANCE (100Ohm) --- Buzzer +   
* Pin 10 : Buzzer -    

## Buzzer/Led
Vous pouvez ajouter une led (**avant la résistance**)
* Pin 9 : RESISTANCE (100Ohm) --- Led + / Buzzer +   
* Pin 10 : Led - / Buzzer -    

# Impression 3D
Ce modèle est un **boitier réutilisable** pour des projets avec un arduino nano    
Modèles fait par Olivier Sarrailh : https://github.com/madnerdorg/buzzer/tree/master/3D    
**Le boitier est légerement trop petit pour être correctement fermé**

# Licences
# Buzzer.ino
* Auteur: Rémi Sarrailh (madnerd.org)   
* Licence: MIT

# ToneAC
* Author: Tim Eckel
* Licence : GNU GPL v3
* Lien: https://bitbucket.org/teckel12/arduino-toneac/wiki/Home
* Donation : [PayPal](https://bitbucket.org/teckel12/arduino-toneac/wiki/Home#!show-your-appreciation)