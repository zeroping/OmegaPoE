# OmegaPoE
A Power-over-Ethernet Dock for the Onion Omega board

This is a KiCad circut board design for an Onion Omega "dock" that connects the Onion via Ethernet, while also powering it via 802.3af Power-over-Ethernet.

The Onion Omega is a cheap ($10.75) linux single-board computer, and supports WiFi and Ethernet. For more information on the Onion Omega, see [the Onion Omega site](http://onion.io/omega2/).

This board is designed to be as small as possible while still providing an isolated 15-watt PoE supply. The 48 VDC power from PoE is converted into 12 V using a TI LM5070 in a flyback configuration. The 12 V is further stepped down to 5 V and 3.3 V using two TPS62135x DC-DC buck converters. 12 V was chosen to allow running 12V perhierals off of the board, such as 12V LED lighing strips. 
