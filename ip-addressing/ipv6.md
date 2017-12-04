# IPv6 Addressing

[__<= GO BACK__](README.md)

- designed with 128 bits addressing system (more IPs were needed)
- designed for efficient address allocation
- accommodates 64 bit MAC addresses

## Overview:

1. [IPv6 Addressing Structure](#ipv6-addressing-structure)
2. [IPv6 Subnetting](#ipv6-subnetting)
3. [Gateway & Subnet Mask](#gateway-subnet-mask)
4. [Reserved Ranges](#reserved-ranges)
5. [IPv6 Addresses](#ipv6-addresses)
6. [Ipconfig](#ipconfig)
7. [Dual IP stacks](#dual-ip-stacks)


## IPv6 Addressing Structure
- 128 bit address divided into 16 bit sections each section has 4 digit hexadecimal number
- each block is separated by a colon (:)
- 2 or more leading 0 (zero) can be removed except for 1 (:0000: => :0:) (:00ff: => :ff:)


## IPv6 Subnetting
- ISP give minimum of /48 prefix (first 48 bits are for network ID)
- after receiving subnet from ISP it's common to use first 16 bits after ISP prefix as site/Network ID


## Gateway & Subnet Mask
- gateway:
  - works similar to IPv4, is 128 bit long, address is represented in IPv6 format
  - requires DHCPv6 to obtain default gateway automatically
- subnet mask:
  - IPv4: list actual subnet mask IP address
  - IPv6: simply tell computer what prefix is being used


## Reserved Ranges
- unspecified IPv6 address (0:0:0:0:0:0:0:0):
  - indicates absence of address
  - never assigned to interface or used as destination
- loopback address(0:0:0:0:0:0:0:1):
  - identify loopback addresses, allows node to send itself packets
  - packets addressed to loopback must never be send to a link or forwarded to router
- compatibility addresses:
  - aid migration from IPv4 to IPv6 (allows coexisting of both on the network)
- 6to4 address:
  - communicate 2 nodes (both running IPv4 & IPv6) over an IPv4 routing infrastructure
  - tunneling: establish connection through public network, looks like point-to-point connection but isn't
- ISATAP Address:
  - communicate 2 nodes (both running IPv4 & IPv6) over an IPv4 routing infrastructure
  - uses locally administered interface, includes both private & public addresses
- Teredo Address:
  - represent host when using Automatic tunneling defined in internet draft teredo
  - beyond first 32 bits, Teredo addresses are used to encode the IPv4 address of a Teredo server


## IPv6 Addresses

- global unicast addresses:
  - equivalent of IPv4 public addresses, globally routable, reachable on IPv6 internet
- link local addresses:
  - communicate with neighboring node on a single link network with no router (equivalent of APIPA addresses)
- site local addresses:
  - equivalent of IPv4 private addresses, can't directly route connections to IPv6 internet
  - don't conflict with global addresses, not reachable outside of specific site they are on


## Ipconfig
- command line tool on windows, primary function: display IP address, subnet mask & default gateway


## Dual IP stacks
- a network that has IPv4 and IPv6 enabled on the same node
- especially important to let routers know about dual IP stack situations because routers are the first nodes to receive outside traffic. It has to know that it can receive both IPv4 and IPv6 into the network
