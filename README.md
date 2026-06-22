# UniFi Multi-Site Home Network Lab

Personal network infrastructure for learning enterprise networking, security best practices, and hands-on experience with Ubiquiti UniFi platform.

> **Note**: This is a personal learning lab. I also have commercial network deployment experience but cannot share client details due to confidentiality.

---

## 🏠 Equipment

### Site 1 - Poland (House)
- **Router/Controller**: UniFi Dream Machine SE (UDM SE)
- **Switch**: UniFi Switch Pro 24 PoE (24 ports)
- **Access Points**: 2x UniFi U6 Pro (WiFi 6)
- **Security**: UniFi G4 Instant Camera, 3x G5 Bullet (planned), UniFi Protect NVR, UPS
- **Clients**: ~30+ devices (computers, phones, tablets, smart home)


### Site 2 - Norway (Apartment)
- **Router**: UniFi Dream Router
- **Switch**: UniFi Switch 16
- **Clients**: ~15+ devices


---

## 🌐 Network Architecture

Multi-site deployment managed through centralized UniFi Network Controller.


*(Network diagram coming soon)*

### VLAN Structure

| VLAN | Purpose | Access Level |
|------|---------|---------------|
| Trusted | Personal devices, computers, phones | Full network access |
| Guest | Visitor WiFi | Internet-only, time-limited |
| IoT | Smart home devices | Restricted, internet-blocked except HomeKit gateways |
| Test/Lab | New device/config testing | Isolated from production |

*Specific IP ranges are anonymized for security purposes.*

---

## 📚 Projects

### 1. [VLAN Segmentation & Security Zones](projects/01-vlan-segmentation.md)
Network isolation strategy with firewall rules between zones. Separates trusted devices from IoT and guest networks for improved security.

### 2. [Multi-Site Network Management](projects/02-multi-site.md)
Centralized controller managing two separate locations. Remote monitoring, configuration sync, and performance tracking.

### 3. [Smart Home Integration](projects/03-smart-home.md)
Apple HomeKit network with Thread and Bluetooth mesh. Cross-VLAN communication for automation while maintaining security isolation.

### 4. [Security Camera System & Backup Strategy](projects/04-security-surveillance.md)
Local NVR storage with offsite cloud backup for disaster recovery, with a scalable storage expansion plan.
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
