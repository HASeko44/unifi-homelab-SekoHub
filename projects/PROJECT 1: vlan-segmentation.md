# VLAN Segmentation & Security Zones

## Overview
Network segmented into 4 VLANs based on trust level and purpose:

| VLAN | Purpose | Access Level |
|------|---------|--------------|
| Trusted | Personal devices, computers, phones | Full network access |
| Guest | Visitor WiFi | Internet-only, time-limited |
| IoT/Smart Home | Smart home devices | Restricted, internet-blocked by default |
| Test/Lab | Testing new devices and configurations | Isolated, used before production rollout |

*Note: Specific IP ranges are anonymized for security purposes.*

## Design Philosophy
Default-deny between zones, with explicit allow rules only where needed. Each VLAN reflects a different trust level rather than just device type.

## IoT / Smart Home Isolation
Most smart home devices have no direct internet access. The only exceptions are the HomeKit hub devices (Apple TV, HomePod mini), which act as gateways for Thread and Bluetooth mesh accessories and are explicitly whitelisted.

A deliberate choice in this setup: **firmware updates for IoT devices are applied manually** rather than allowing automatic cloud-pushed updates. This reduces the attack surface, avoids unexpected behavior changes, and allows verifying compatibility and security advisories before applying updates - the same approach I'd want to apply in a professional environment with customer equipment.

## Guest Network
- Time-limited DHCP leases
- Client isolation enabled
- No access to other VLANs, internet-only

## Test/Lab VLAN
New devices, firmware, or configurations are validated here before being moved into Trusted or IoT VLANs. This minimizes risk of misconfiguration affecting production devices.

---
[Back to main README](../README.md)
