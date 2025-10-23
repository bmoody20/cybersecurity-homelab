# cybersecurity-homelab
Personal cybersecurity learning environment - Infrastructure, security implementation and monitoring stack
## 🎯 Overview

This homelab serves as a hands-on learning platform for cybersecurity concepts, built as part of my career transition from Finance to Cybersecurity/Information Security.

**Current Focus Areas:**
- Infrastructure security hardening
- Network monitoring and analysis
- Intrusion detection and prevention
- Log analysis and SIEM concepts
- Secure service deployment

## 🏗️ Infrastructure

**Hypervisor:** Proxmox VE  
**Containers:** 7 LXC containers + 2 VMs  
**Storage:** ZFS pool with backup strategy  
**Network:** Segmented with Tailscale mesh VPN

### Services Deployed
- **Photo Management:** Immich (self-hosted Google Photos alternative)
- **File Storage:** Nextcloud + Collabora Office
- **DNS & Ad Blocking:** Pi-hole
- **Monitoring:** Prometheus + Grafana + Uptime Kuma
- **Security:** Crowdsec IDS/IPS, Fail2Ban, UFW firewall

## 🛡️ Security Implementation

**Multi-layered defense approach:**

1. **Perimeter:** Cloudflare Tunnel (zero open ports to internet)
2. **Network:** UFW firewall on all systems
3. **Detection:** Crowdsec community threat intelligence
4. **Application:** Fail2Ban brute force protection

**Metrics:**
- 14,000+ malicious IPs blocked
- Real-time threat monitoring
- Automated response to common attacks

## 📊 Monitoring

Full observability stack with:
- System metrics (CPU, RAM, disk, network)
- Service health checks
- Security event logging
- Custom Grafana dashboards
- Alerting via multiple channels

## 📚 Documentation

Detailed documentation available in the `/docs` folder:
- [Network Architecture](docs/architecture.md) *(coming soon)*
- [Security Implementation](docs/security.md) *(coming soon)*
- [Monitoring Setup](docs/monitoring.md) *(coming soon)*

## 🎓 Learning Objectives

This project helps me develop skills in:
- Linux system administration
- Container orchestration (Docker, LXC)
- Network security concepts
- Log analysis and correlation
- Incident detection and response
- Infrastructure as code principles

## 🔧 Technologies

**Infrastructure:** Proxmox, LXC, Docker, ZFS  
**Security:** Crowdsec, Fail2Ban, UFW, Cloudflare  
**Monitoring:** Prometheus, Grafana, Node Exporter  
**Networking:** Tailscale, DNS, reverse proxy  
**Applications:** Immich, Nextcloud, Pi-hole

## 📈 Project Status

🟢 **Active Development** - Continuously expanding and learning

**Next Steps:**
- Add SIEM solution (Wazuh)
- Implement vulnerability scanning
- Create incident response playbooks
- Document security procedures

- ## 📝 Notes

This is a personal learning project. All sensitive information has been sanitised from configurations. The focus is on demonstrating security concepts and infrastructure design skills.

---

**Last Updated:23 October 2025  
**Status:** In Active Development
