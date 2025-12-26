# ssh-bruteforce-detection-wireshark
Detected SSH brute-force login attempts by analyzing repeated TCP port 22 connections using Wireshark in a controlled lab environment.

## Overview
This project demonstrates how repeated failed SSH login attempts can be detected by analyzing network traffic using Wireshark.

Lab Setup

Attacker: Kali Linux

Target: Metasploitable

Tool: Wireshark

Procedure

Started packet capture in Wireshark

Generated multiple failed SSH login attempts to the target

Captured and filtered SSH traffic using:

tcp.port == 22


Analyzed repeated connections using Statistics → Conversations → TCP

Verified SSH sessions using Follow → TCP Stream

Findings

Multiple SSH connection attempts from a single source IP

Repeated authentication failures in a short time period

Clear brute-force login pattern observed on TCP port 22

Skills Demonstrated

Network traffic analysis

SSH brute-force detection

Wireshark filtering and statistics

SOC-style investigation workflow

Screenshots

All screenshots related to the analysis are included in the screenshots/ directory.

Disclaimer

This project was conducted in a controlled lab environment for educational purposes only.
