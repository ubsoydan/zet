# 20230810190805
# Layer 2 - Data Link

This extends to [OSI 7 Layer Model, 20230810175926](../20230810175926/README.md)
This extends to [Layer 1 Physical, 20230810182033](..//20230810182033/README.md)

Layer 2 sits on top of layer 1 with the exception of having a unique addressable
asset which is MAC address. If device1 decides to send a package, it will have
a certain address to go which is device2's MAC addresss. That package is called
frame and it is passed to layer 1 to do logistics of sending package.

Layer 1 takes the package, checks if there is another carrier on layer 1 level
which could be another device sending another package. If no carrier found,
layer 1 converts and transmits the frame. By the way, layer 1  doesn't know 
what frame carries, it is an encapsulated raw data and it has a certain address
to arrive at.

Opposite layer 1 receives the frame and passes up to layer 2. And the same cycle
goes on. However, if a device's frame collide with another's, a random rejecting
happens and one of the packages backs off for a moment to prevent collision.

All the layer 2 actions happen thanks to network switches. Switches understand
frames and MAC addresses. They keep track of MAC addresses of devices on
the network, called MAC address table. So with the help of the table, they
forward only valid frames to valid MAC addresses unlike hubs which just
broadcasts all the data regardless.  
