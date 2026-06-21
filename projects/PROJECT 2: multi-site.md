# Multi-Site Network Management (Norway & Poland)

## Overview
Two physically separate networks - one in an apartment in Norway, one in a standalone house in Poland - managed centrally through a single UniFi cloud controller.

| Site | Location | Equipment |
|------|----------|-----------|
| Site 1 | Norway (apartment) | UDM SE, Switch Pro 24 PoE, 2x U6 Pro |
| Site 2 | Poland (house) | Dream Router, Switch 16 |

## Why Centralized Management
- Single pane of glass for both networks regardless of location
- Consistent VLAN structure and security policy across both sites
- Remote troubleshooting and configuration without traveling
- Real-time visibility into uptime and client activity at both locations

## Cross-Border Considerations
Managing networks across two countries introduces practical challenges:
- Different ISPs with different reliability and routing characteristics
- No shared local network between sites - each operates independently but follows the same configuration standards
- Remote access secured through UniFi's built-in VPN, avoiding direct exposure of services to the internet

## Remote Support Experience
Because Site 2 is used by family members with limited technical knowledge, this setup has also given me practical experience supporting non-technical users remotely - diagnosing issues, applying fixes, and explaining changes in simple terms without being physically present. This mirrors the kind of remote troubleshooting expected when supporting customers across different locations.

---
[Back to main README](../README.md)
