# Network Topologies

[__<= GO BACK__](README.md)

__Physical Topology:__ physical layout of the network

__Logical Topology:__ how data moves through the network, pattern of data flow

## Index

1. [Topologies](#topologies)
2. [Network Management Models](#network-management-models)
3. [Ways to Connecting to the Network](#ways-to-connecting-to-the-network)
4. [Internet vs. Intranet vs. Extranet](#internet-intranet-extranet)

## Topologies

1. [Full Mesh](#full-mesh)
2. [Partial Mesh](#partial-mesh)
3. [Bus](#bus)
4. [Ring](#ring)
5. [Star](#star)
6. [Hybrid](#hybrid)
7. [Point to Point](#point-to-point)
8. [Point to Multipoint](#point-to-multipoint)


### Full Mesh

- all devices directly connected to all other devices
- full redundancy
- most expensive
- requires multiple NICs & Cables
- WAN environment (not LAN)


### Partial Mesh

- all devices directly connected to at least 2 other
- strong but not full redundancy
- not as expensive,
- requires multiple NICs & Cables
- requires multiple NICs & Cable (WAN)


### Bus

- one of oldest topologies
- all nodes connect directly to main cable (bus)
- simple to put together
- only one signal at a time
- contention used to determine which node sends signals
- more active nodes == more collisions on network (cancel out each other)
- too many collisions bring down network
- only for 30 nodes or less
- Cheapest network
- 1 bad node or cable brings down all the network
- not part of the TIA/EIA 568-C Standard


### Ring

- one of the oldest topologies
- similar to Bus but connected in a circle
- packets move in ring around (nodes decide if they need or pass packets)
- each node gets opportunity to send a signal
- no contention between nodes
- heavy traffic slows down network (not down)
- 1 bad node or cable brings down all the network
- not part of the TIA/EIA 568-C Standard


### Star

- most common used in LAN
- more expensive than bus because it needs more cables
- all nodes connect to central hub or switch
- easy to troubleshoot
- if everything is down the central device is at fault
- if single node goes down on the the node is at fault
- part of the TIA/EIA 568-C Standard (only accepted in LAN)


### Hybrid

- combines star topology with other
- different types: physical-hybrid star, physical-logical hybrid
- functions like a ring but is a star network


### Point to Point

- connect 2 nodes directly to each other no intervening device
- connect 2 end of a WAN connection
- connect computer directly to switch
- connect switches and routers to each other


### Point to Multipoint

- similar to a point to point topology
- one devices connects to more than one device


## Network Management Models

|Peer to peer                                     |Client Server |
|-------------------------------------------------|---------------------------------------------------|
| computer responsible for its security management|all devices access resources through central server|
| each computer managed as separate device        |devices that need access to server are clients     |
| usually for small networks                      |devices controlling access are called servers      |
| Microsoft limits to 10 systems per network      |management is overseen by central server           |
| Home group and Workstation are P2P              |security is build around central server            |
| Used in small business of 2-3 computers         |server allows/restricts access to network          |
| most home networks                              |if server goes down no one can connect to network  |


## Ways to Connecting to the Network

> (NA = Network Access)

> (CSMA/CD = Carrier Sensing Media Access/Collision Detection)

> (CSMA/CA = Carrier Sensing Media Access/Collision Avoidance)

__3 types of Connecting to the Network:__

1. Contention based NA
2. CSMA/CD
3. CSMA/CA

### Contention based NA

computers compete for Network Access

__2 types of contention based NA:__

- CSMA/CD: commonly used by wired ethernet
- CSMA/CA: commonly used by wifi network


### CSMA/CD

- each node/computer listens for traffic
- if node hears no traffic it releases a packet on the network
- if node release packets at the same time, a collision occurs
- collisions cause power spike, all nodes can hear
- during collision the data packages are destroyed
- if no collision, transmission is successful and network is freed up
- if collision, all nodes start internal clock (rand #s), attempt new


### CSMA/CA

- similar to CSMA/CD
- releases warning packet before sending packet
- if other nodes hear warning they won’t transmit
- once data packet heard the rest can transmit
- two warning packets transmitted at same time cause collision
- collision is handled like CSMA/CD


## Internet, Intranet, Extranet

|Internet                               |Intranet                                 |Extranet                                  |
|---------------------------------------|-----------------------------------------|------------------------------------------|
|public accessible infrastructure       |privately accessible infrastructure      |privately held WAN infrastructure         |
|used to carry a variety of services    |limited to a single company, organization|owned by a company usually                |
|WWW, FTP, Email, VoIP, Streaming Video |carry a variety of services like Internet|may allow access to others for fee/purpose|
