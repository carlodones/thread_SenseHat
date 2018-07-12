# Test single 
container per ricerca errore dovuto a multiarray (numpy) e impossibilità di utilizzo di qualsiasi script python risolto con single container

# Test multi
è necessario applicare struttura multicontainer per sviluppo software, si procede alla seconda fase di test (multidocker)

# Sviluppo gestione multidocker
La terza fase di sviulippo si è conclusa positivamente con l'avvio multicontainer i Dockerfile prevedono l'importazione del pacchetto Python Jessie (segue specifica) ogni docker sio avvia in modo autonomo.

https://packages.debian.org/jessie/python/

https://packages.debian.org/jessie/

# Docker link 

https://docs.docker.com/get-started/#recap-and-cheat-sheet

https://docs.docker.com/engine/reference/builder/#cmd

# Seguono i diversi container utilizzati a fine test

# Sense-tunnel
A scrolling tunnel game using the Sense Hat orientation sensors for control.

Based on the Marble Maze tutorial found [here](https://www.raspberrypi.org/learning/sense-hat-marble-maze/). 

### Gameplay
The marble (white dot) is controlled by tilting the board in any direction. The game ends if the marble hits a red dot or is carried off screen by the tunnel wall. Start a new game by pressing the joystick.

# Raspberry-pi-sense-hat-audio-spectrum-analyzer
python code to analyze audio spectrum using the LED matrix of the Raspberry Pi sense HAT

This code is a modification of https://www.rototron.info/raspberry-pi-spectrum-analyzer/.
It's modified to work with the LED matrix of the sense HAT.

You can either play a wav file from the pi, or use a microphone. I used this USB microphone:

http://www.dx.com/p/mi-305-plug-and-play-mini-usb-microphone-black-287434#.WlJ5qt-nFPY

but any mic that works with the Raspberry Pi should be working.

## Install dependencies
```
sudo apt-get update && sudo apt-get upgrade
sudo apt-get install python-dev python-imaging python-smbus python-alsaaudio sense-hat python-numpy
```

and for using the microphone:

`sudo apt-get install python-pyaudio`

## Running
For playing a wav file:
`python audio_analyzer_wav.py /path/to/wav/file`

This version has a somewhat more creative LED visualisation:
`python audio_analyzer_disco_wav.py /path/to/wav/file`

And this version uses the microphone:
`python audio_analyzer_mic.py`

## Orientation
The default orientation of the sense HAT is, with the GPIO 
connection on top, the left side being the bottom of the visualisation.
When mounted on the pi, it means you need point the USB-ports
upward for the correct orientation.

If you want to position differently, change the `rotation = 0` 
in the code to 90, 180 or 270.

# Analizzatore Temperatura Pressione Umidità

python code to analize pressure umidity and temperature from sensors Sense Hat


