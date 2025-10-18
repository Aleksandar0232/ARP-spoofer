ARP Spoofer

A small, educational Python tool to demonstrate ARP spoofing / ARP poisoning on a local network using Scapy.
This repository is intended only for learning and for use on networks you own or where you have explicit written permission to test.

⚠️ Legal & ethical notice: ARP spoofing can intercept network traffic and may be illegal or against policy on networks you do not own. Only run this in a controlled lab environment or with explicit authorization.


What it does
The script repeatedly sends forged ARP replies to:
Tell a target machine that we are the gateway.
Tell the gateway that we are the target.
That causes traffic between the target and the gateway to pass through the attacker's machine — a classic Man-in-the-Middle technique. The script attempts to restore ARP tables when interrupted.

Requirements
Python 3.8+ recommended.
scapy library.
Root/Administrator privileges (required to craft and send raw packets).
Tested on Linux; other platforms may require additional setup.
