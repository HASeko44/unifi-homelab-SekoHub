# Smart Home Network Integration

## Equipment
- Apple TV (HomeKit hub)
- HomePod mini (Thread border router)
- Various HomeKit-compatible accessories

## Network Placement
All smart home devices sit in the IoT VLAN, separate from trusted devices. Access to this VLAN is restricted to authorized household members only.

## Gateway Exception
By default, IoT devices have no outbound internet access. The HomeKit hub devices (Apple TV, HomePod mini) are the only explicitly whitelisted exceptions, since they act as bridges for Thread and Bluetooth mesh accessories and need connectivity to function correctly.

## Manual Firmware Management
Rather than letting smart devices auto-update over the internet, firmware and app updates are applied manually. This gives control over:
- When updates are applied (avoiding unexpected downtime)
- What changes are introduced (reviewing release notes first)
- Compatibility with the existing network setup before rolling out

## Access Control
Only authorized users have credentials to the IoT network and HomeKit administration. This prevents unauthorized control of smart devices (locks, cameras, etc.) even if a guest is on the property.

---
[Back to main README](../README.md)
