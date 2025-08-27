# Static Routing Between Two Different Networks

This project demonstrates how to configure **static routing** between two different networks using Cisco Packet Tracer. The setup involves two routers, switches, and four PCs across two different subnets.

## 🖧 Network Topology Overview

- **Router 1 (R1)** connects the 192.168.1.0/24 network.
- **Router 2 (R2)** connects the 192.168.2.0/24 network.
- **A static route is configured on both routers** to enable communication between the two networks.
- Each network is connected via switches, with two end devices (PCs) in each subnet.

## 🛠️ Configuration Summary

### Router R1 (ISR4331)
**Interfaces**:
- `Gig0/0/0`: 192.168.3.1 (connects to R2)
- `Gig0/0/1`: 192.168.1.1 (LAN side)

**Static Route**:

### Router R2 (ISR4331)
**Interfaces**:
- `Gig0/0/0`: 192.168.3.2 (connects to R1)
- `Gig0/0/1`: 192.168.2.1 (LAN side)

**Static Route**:

### End Devices
- **Network A (192.168.1.0/24)**:
  - PC0: 192.168.1.2
  - PC1: 192.168.1.3
- **Network B (192.168.2.0/24)**:
  - PC2: 192.168.2.2
  - PC3: 192.168.2.3

## 🧪 Testing

From **PC0 (192.168.1.2)**:
- Successful ping to **PC2 (192.168.2.2)** after initial ARP-related timeout.
- All subsequent pings succeed with 0% packet loss.

## ✅ Requirements

- Cisco Packet Tracer (version 7.2 or higher recommended)
- Basic knowledge of:
  - IP addressing
  - Static routing
  - Cisco IOS command line

## 📁 Files

- `.pkt` file with full topology setup (not included here)
- Screenshot of topology and ping results:  
  `Screenshot 2025-08-27 182449.png`

## 📸 Topology Preview

![Static Routing Topology](Screenshot%202025-08-27%20182449.png)

## 🚀 How to Use

1. Open the Packet Tracer file.
2. Review static routing configurations on both routers.
3. Use the command prompt on the PCs to test cross-network connectivity.
4. Observe successful routing between networks.

## 📚 License

This project is for educational use only.
