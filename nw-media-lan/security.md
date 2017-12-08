# Wireless LAN Security

[__<= GO BACK__](README.md)

## Overview:

1. [WEP](#wep-wired-equivalency-privacy-)
2. [WPA & WPA2](#wpa-wpa2-wi-fi-protected-access-)
3. [Ethernet Protection](#ethernet-protection)

## WEP (Wired Equivalency Privacy)
- introduced 1997 & deprecated in 2004
- 40 bit key + 24 bit initialization vector = 64 bits total (later extended to 128)
- IV is 24 bits long and has a 50% likelihood of repeating after 5,000 packets

## WPA & WPA2 (Wi-Fi protected Access)

### WPA
- released 2003 & replaced WEP
- WEP Wi-Fi cards can be upgraded to WPA with a software update
- uses TKIP: Temporal Key Integrity Protocol (deprecated in 2009)

### WPA2
- released 2004 to replace WPA
- supports TKIP but prefers AES
- initial authentication via TKIP or CCMP
- 4 way group Key handshake: provides mutual key authentication
- group key handshake: prevents disconnected clients from receiving broadcast

## Ethernet Protection
- 802.1X
  - authenticates wired and wireless
  - consists of 3 pieces:
    - Supplicant: support OSs
    - Authenticator: takes authentication from supplicant and passes to authentication server
    - Authentication Server: checks credentials via EAP
