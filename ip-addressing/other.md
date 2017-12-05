# Other Concepts related to Addressing

[__<= GO BACK__](README.md)

## Overview:

1. [Ports](#ports)
2. [Packets](#packets)
3. [Remote Access](#remote-access)

## Ports
- endpoint in OS for different types of communication
- associated with IP address of host
- identified by 16-bit numbers (port numbers)
- used by Transport and Session Layer of the OSI model
- 3 parts of ports:
  - well known ports
  - registered ports
  - dynamic/private ports


## Packets
- formatted units of data carried across packet switch network
- benefits:
  - bandwidth of communications link can be shared across devices
  - each packets can find its own way across the network
  - easily rerouted if a link goes down
  - 2 parts of a packet:
    - control information found in header: (info to deliver packet)
    - payload/user info found in the body: (actual data)

## Remote Access
- communicate with computer/network from remote location using data link (internet)
- can be accomplished by VPN, Remote Desktop Software, terminal emulation
