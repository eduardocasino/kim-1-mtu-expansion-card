# KIM-1 Expansion Board for MTU Cards

## About

Welcome to my KIM-1 Expansion Board for MTU cards repository.

This board follows the MTU standard for the KIM-1 expansion bus and enables to connect up to five cards, like the [K-1008](https://github.com/eduardocasino/k-1008-visable-memory-card-replica). Additionally, all signals of the KIM-1 are replicated on an edge connector to allow further expansions and also on a pin header for easy breadboarding.

The MTU bus connects 1 to 1 to the KIM-1 expansion connector with the exception of pins 2,3, 16, 17, 18, 19, 20 and X, because MTU boards use some of these pins for power and expanded 18 bit address bus (See page 33 of the [MTU Fall 1980 6502 Peripherals and Software catalog](http://retro.hansotten.nl/uploads/files/MTU-fall-1980.pdf)) Two pin connectors have to be wired to pins J (K7) and K (DECODE ENABLE) of the KIM-1 application connector.

Like in the original MTU's bus motherboard, a five screw terminal block provides power connectios for both the KIM-1 (GND, +5V and +12V regulated) and the expansion boards (+7.5V and +16V unregulated). Also as in the original, the +12V terminal is not really connected to anything.

![components](https://github.com/eduardocasino/kim-1-mtu-expansion-card/blob/main/images/kim-1-mtu-expansion-card-comp.png?raw=true)
![front](https://github.com/eduardocasino/kim-1-mtu-expansion-card/blob/main/images/kim-1-mtu-expansion-card-front.png?raw=true)
![back](https://github.com/eduardocasino/kim-1-mtu-expansion-card/blob/main/images/kim-1-mtu-expansion-card-back.png?raw=true)

This is how an example setup with one K-1008 board would look like:

![setup](https://github.com/eduardocasino/kim-1-mtu-expansion-card/blob/main/images/kim-1-with-k-1008.png?raw=true)

The board has been built and tested with my [KIM-1](https://github.com/eduardocasino/kim-1) and [K-1008](https://github.com/eduardocasino/k-1008-visable-memory-card-replica) replicas.

## Licensing

This is a personal project that I am sharing in case it is of interest to any retrocomputing enthusiast and all the information in this repository is provided "as is", without warranty of any kind. I am not liable for any damages that may occur, whether it be to individuals, objects, KIM-1 computers, kittens or any other pets.

[![license](https://i.creativecommons.org/l/by-sa/4.0/88x31.png)](http://creativecommons.org/licenses/by-sa/4.0/)

This work is licensed under a [Creative Commons Attribution-ShareAlike 4.0 International License](http://creativecommons.org/licenses/by-sa/4.0/).

See the LICENSE.md file for details.

## Changelog
#### 19/11/2023
* License change to a less restrictive one.
#### 11/11/2023
* Fix solder mask for connectors. For real this time. Damn.
#### 04/08/2023
* Fix solder mask for connectors

## Acknowledgements

* Hans Otten and his [Retro Computing blog](http://retro.hansotten.nl/). Documentation of MTU's line of hardware expansions for the KIM-1
