# Wireless LAN

[__<= GO BACK__](README.md)

## Overview:

1. [Wireless LAN Types](#wireless-lan-types)
2. [Frequency Used](#frequency-used)
3. [Current Standards](#current-standards)
4. [Future Standards](#future-standards)


## Wireless LAN Types

|Consumer Wi-Fi             |Enterprise Wi-Fi           |
|---------------------------|---------------------------|
|consumer grade hardware    |higher end hardware        |
|independent configuration  |centralized configuration  |
|limited area coverage      |smooth hardware transition |


## Wireless Standards
- 802.11:
  - legacy: A, B
  - current: G, N
  - future: AC
- Modulation:
  - DSSS: Direct Sequence Spread Spectrum (legacy, many bits in single parallel stream)
  - OFDM: Orthogonal Frequency Division Multiplexing (creates multiple subcarriers and sends across all at once)

> __OFDM:__ Used by all standards except 801.11B


## Frequency Used
- 2.4GHz:
  - 14 channels
  - each channel is spaced every 5Mhz (channel 1 = 2.412GHz, channel 2 = 2.217Ghz)
  - Wi-Fi uses 20Mhz channels each
  - 3 non overlapping Channels are 1,6 and 11
- 5GHz:
  - 165 channels
  - each channel is spaced every 20Mhz (channel 1 = 5.180Ghz, channel 2 = 5.200Ghz)
  - Wi-Fi uses 20Mhz channels each
  - 25 non overlapping channels


## Current Standards
- 802.11G:
  - support B clients
- 802.11N:
  - widest deployment
  - 600Mb of throughput
  - 2.4GHz and 5GHz
  - uses 3 techniques:
    - MIMO: Multiple In and Multiple Out, up to 4 antennas
    - Frame Aggregation: send more than 1 frame in a transmission
    - Wider Transmission Channels


## Future Standards
- 802.11AC:
  - speed greater than 1GB per second
  - more antennas up to 8
  - larger channels up to 160Mhz
  - MU-MIMO (Multi User MIMO)
  - 5GHz only
