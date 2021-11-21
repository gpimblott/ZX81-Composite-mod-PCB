# ZX81-Composite-mod-PCB
PCB that implements the ZX81 composite mod including the backporch signal for older versions 

The PCB KiKad files in this repo implement a composite mod board for the ZX81 as described [here](http://zx.zigg.net/misc-projects/ZX81_Video_Conditioning.pdf).  More details can also be found on the excellent [joulespercoulomb YouTube video](https://www.youtube.com/watch?v=1irH3KuGyl0).

![ZX81Schematic](https://user-images.githubusercontent.com/2563249/142768406-5d6e7f86-b81a-464e-93f6-7f0ccd4e1ada.png | width=300)

If the backporch signal is not required then the 555 timer chip can be omitted.  I have used this on two ZX81's without the 555 and it results in a much better picture than the frequently described transistor mod alone.

# Parts list

The following components are needed to complete the PCB
* R1,R2 - 10K Resistor
* R3 - 68 Resistor
* R4 - 56 Resistor
* C1 - 22uF electrolytic capacitor
* C2 - 10nF ceramic disc capacitor
* C3 - 820pF ceramic disc capacitor
* C4 - 82pF ceramic disc capacitor
* Q1,Q2 - 2N2222 transistor
* D1,D2 - 1N4148 signal diodes
* U1 - NE555 Timer (Optional)

# Fitting the board
The board is redesigned to fit inside the existing housing once the original modulator has been removed.  This is done by desoldering the 5v and video signal wires entering the metal casing from the mother board then desoldering the large casing anchors.  Once this is done you should be able to remove the modulator.  The bottom can then be removed.  Once this is done the ground bridges will need to be desoldered anchoring the PCB into the case.  The signal wire from the PCB to the composite output jack will also need to be desoldered.

Getting it free can be pain and worse if you want to keep the original modulator in one piece.  Once removed the new PCB can be inserted and connected to the necessary locations
* 5v to the motherboard (same as the original)
* Video in to the motherboard (same as the original)
* Video out to the centre of the jack
* Ground to the modulator casing (don't forget to use the underside pads to anchor the PCB into the casing (and earth the PCB)

![PCB installed in place of original modulator](https://user-images.githubusercontent.com/2563249/142767879-9eadfb79-f528-465a-b3aa-ff493ee1c5ed.jpg | width=300 )
