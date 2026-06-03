---
name: subnet-calc
description: Network subnet calculator for IP planning and pentest reconnaissance. Calculates network ranges, generates nmap scan commands, and visualizes subnet divisions.
---

# Subnet Calculator

Network subnet calculator for IP planning and pentest reconnaissance. Computes network details from CIDR notation, generates ready-to-use nmap commands, and supports VLSM subnetting.

## Features

- **CIDR Parsing**: Accepts standard CIDR notation (e.g., `192.168.1.0/24`).
- **Network Calculations**: Network address, broadcast address, first/last usable hosts, total hosts, wildcard mask.
- **nmap Command Generation**: Quick scan, full port scan, vulnerability scan, OS detection commands.
- **VLSM Subnetting**: Divide a network into smaller subnets with efficient address allocation.
- **Fully Offline**: No API calls required.

## Input

JSON object with:
- `cidr` (string): Network in CIDR notation (e.g., "192.168.1.0/24").
- `subnet_into` (optional number): Number of subnets to divide into (for VLSM).
- `target_subnet_prefix` (optional number): Target prefix length for VLSM division.

## Output

JSON with:
- Network details table (network, broadcast, gateway, hosts, mask)
- nmap scan commands
- VLSM division (if requested)
