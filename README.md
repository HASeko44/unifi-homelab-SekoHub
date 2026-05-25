# UniFi Multi-Site Home Network Lab

Personal network infrastructure for learning enterprise networking, security best practices, and hands-on experience with Ubiquiti UniFi platform.

> **Note**: This is a personal learning lab. I also have commercial network deployment experience but cannot share client details due to confidentiality.

---

## 🏠 Equipment

### Site 1 - Primary Location
- **Router/Controller**: UniFi Dream Machine SE (UDM SE)
- **Switch**: UniFi Switch Pro 24 PoE (24 ports)
- **Access Points**: 2x UniFi U6 Pro (WiFi 6)
- **Security**: UniFi G4 Instant Camera
- **Clients**: ~30+ devices (computers, phones, tablets, smart home)

### Site 2 - Secondary Location
- **Router**: UniFi Dream Router
- **Switch**: UniFi Switch 16
- **Clients**: ~15+ devices

**Total Investment**: ~$2000 USD in professional-grade equipment

---

## 🌐 Network Architecture

Multi-site deployment managed through centralized UniFi Network Controller.

![Network Topology](diagrams/network-topology.png)
*(Network diagram coming soon)*

### VLAN Structure

| VLAN | Name | Subnet | Purpose |
|------|------|--------|---------|
| 10 | Trusted | 192.168.10.0/24 | Work computers, personal devices |
| 20 | Guest | 192.168.20.0/24 | Visitor WiFi, isolated |
| 30 | IoT | 192.168.30.0/24 | Smart home devices |
| 40 | Security | 192.168.40.0/24 | Cameras, NVR |
| 99 | Management | 192.168.99.0/24 | Network equipment |

---

## 📚 Projects

### 1. [VLAN Segmentation & Security Zones](projects/01-vlan-segmentation.md)
Network isolation strategy with firewall rules between zones. Separates trusted devices from IoT and guest networks for improved security.

### 2. [Multi-Site Network Management](projects/02-multi-site.md)
Centralized controller managing two separate locations. Remote monitoring, configuration sync, and performance tracking.

### 3. [Smart Home Integration](projects/03-smart-home.md)
Apple HomeKit network with Thread and Bluetooth mesh. Cross-VLAN communication for automation while maintaining security isolation.

---

## 💡 Skills Demonstrated

- **VLANs & Routing**: Advanced segmentation, inter-VLAN routing, firewall policies
- **WiFi 6 Deployment**: Professional AP placement, channel planning, seamless roaming
- **PoE Management**: Power delivery, planning, and optimization
- **Security**: Zone-based firewall, network isolation, IoT security
- **Monitoring**: UniFi Controller, traffic analysis, troubleshooting
- **Multi-Site**: Centralized management, remote configuration, scalability

---

## 🎯 Why This Lab?

I'm passionate about network engineering and use this lab to:
- Practice real-world enterprise scenarios
- Test new configurations safely before production
- Learn Ubiquiti platform (also experienced with Cisco)
- Prepare for professional network engineering roles
- Continuously improve my technical skills

This isn't just a hobby - it's serious preparation for building reliable, secure networks professionally.
