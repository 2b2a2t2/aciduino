# Aciduino V2

Put your DIY super powers to the test building your own Roland's TB-303 and/or TB-808 step sequencer! An Arduino based clone project specially hacked with corrosive features to improve live performances! Save your money building the classic and timeless TB-303 and TR-808 step sequencer clone faster than a blink of an eye.

This version is multi-architecture, allowing for the use of different microcontrollers in the build. Currently, it supports Arduino Mega, any Teensy >= 3.2, and features experimental and ongoing support for ESP32.

Aciduino V2 is also the first official [uMODULAR](https://github.com/midilab/uMODULAR) app, leveraging uMODULAR schematics, [uCtrl](https://github.com/midilab/uCtrl) drivers/interface library, and [uClock](https://github.com/midilab/uClock) BPM clock generator.

# Download

The recommended way for aciduino users is to make use of release pack on [Releases area](https://github.com/midilab/aciduino/releases), make sure to download the one named aciduino-v2_xxx.zip, where xxx is the version released.  
  
If you want to get the latest on the edge features and keep in track with development of aciduino you can make use of git version via clone.  
  
As this version utilizes uCtrl and uClock libraries as submodules, please remember to initialize the submodules immediately after cloning the repository.  

```console
phuture@acidlab:~$ git clone https://github.com/midilab/aciduino.git
phuture@acidlab:~$ cd aciduino/
phuture@acidlab:~$ git submodule update --init --recursive
```

## How does it looks like?

![Image of aciduino on protoboard](https://raw.githubusercontent.com/midilab/aciduino/master/v2/hardware/imgs/aciduino_v2_teensy_bb.jpg)

![Image of aciduino teensy on protoboard](https://raw.githubusercontent.com/midilab/aciduino/master/v2/hardware/imgs/aciduino_lite_v2-teensy.png)

![Image of aciduino mega on protoboard](https://raw.githubusercontent.com/midilab/aciduino/master/v2/hardware/imgs/aciduino_v2-avr_mega_bb.png)

Aciduino v2 brings new acid elements such as 808 step sequencer and a generative engine based on euclidian algorithm for great acid drums ideas.

A oled screen to get access to all parameters that matters in realtime, a easy to edit grid system for 808 and 303.

![Image of aciduino on protoboard](https://raw.githubusercontent.com/midilab/aciduino/master/v2/hardware/imgs/aciduino-v2-808-grid.jpg)

[Click here for more info](https://github.com/midilab/aciduino/tree/master/v2/)

## Assembly

Place the buttons, knob and powerlines

![Image of aciduino on protoboard](https://raw.githubusercontent.com/midilab/aciduino/master/v2/hardware/imgs/step1.jpg)

You need to increase the size of two of the hole to place the pot base support on top (+) connect grid line.

![Image of aciduino on protoboard](https://raw.githubusercontent.com/midilab/aciduino/master/v2/hardware/imgs/step1_pot_placement.jpg)

Place signal lines for buttons

![Image of aciduino on protoboard](https://raw.githubusercontent.com/midilab/aciduino/master/v2/hardware/imgs/step2.jpg)

## How to use?

The interface presents you simple schema to navigate and interact with you aciduino.

**Navigation buttons:** UP, DOWN, LEFT. RIGTH. use to navigate thru page elements.  
*4 right most buttons*  

**Element buttons:** If the current selected element has an action, it will show up at bottom of your display with the action name for each button.  
*2 upper buttons*  

**Generic buttons:** Acts as value changer, a decrementer and incrementer for almost all elements.  
*2 lower buttons*  

**Pot:** Acts as a value changer just like generic buttons, most of elements can be changed using generic buttons or the pot as wish.  

**Shift button** Hold it while press another interface button.  
*1 alone button at left*  

**Shift + Nav UP/DOWN:** Change page  
**Shift + Nav LEFT/RIGHT:** Changes subpage  
**Shift + Generic button 1:** Previous track  
**Shift + Generic button 2:** Next track  

**Step Sequencer Pot, Shift + Pot**  
303: [Pot] Changes notes [Shift + Pot] Changes octave   
808: [Pot] Changes voice [Shift + Pot] Changes voice config(midi cc or cv port)  

# uMODULAR uOne

One of the uMODULAR projects to run your Aciduino V2, soon avaliable.

![Image of aciduino on uone front](https://raw.githubusercontent.com/midilab/aciduino/master/v2/hardware/imgs/uone_umodular.jpg)

![Image of aciduino on uone back](https://raw.githubusercontent.com/midilab/aciduino/master/v2/hardware/imgs/uone_back.jpeg)
