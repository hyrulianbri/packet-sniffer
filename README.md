Use this in conjunction with Scapy
In Scapy, we will use the sniff() function to capture network packets.
To see a list of what functions Scapy has available, open Scapy and run the lsc() function.
Run the ls() function to see ALL the supported protocols.
Run the ls(protocol) function to see the fields and default values for any protocol. E.g. ls(BOOTP)
See packet layers and contents with the .show() method.
Dig into a specific packet layer using a list index: pkts[3][2].summary()
...the first index chooses the packet out of the pkts list, the second index chooses the layer for that specific packet.
Using the .command() method will return a string for the command necessary to recreate that sniffed packet.

To see the list of optional arguments for the sniff() function:
print(sniff.__doc__)
