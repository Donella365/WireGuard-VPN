# WireGuard-VPN
This project demonstrates the implementation of a self-hosted VPN using WireGuard on a DigitalOcean VPS. The VPN provides secure remote access, encrypted communication, and private tunneling for client devices.

## Objectives
- Deploy a VPS on DigitalOcean as the VPN server.  
- Install and configure WireGuard.  
- Generate and manage server/client key pairs.  
- Enable IP forwarding and NAT for outbound traffic.  
- Create reusable configuration templates for multiple clients.  
- Document the setup for reproducibility and portfolio demonstration.

  ## Architecture
- **Server:** DigitalOcean Droplet (Ubuntu 22.04 LTS)  
- **VPN Protocol:** WireGuard (UDP, port 51820)  
- **Addressing Scheme:** `10.0.0.0/24` subnet for VPN clients  
- **Clients:** Configured via WireGuard app

## ⚙️ Step-by-Step Setup

### Deploy VPS on Digital Ocean
  Log into Digital Ocean (https://www.digitalocean.com/) Spin up a virtual machine/create droplet. 
  <img width="670" height="329" alt="Screenshot 2025-08-21 153337" src="https://github.com/user-attachments/assets/34cf2bf3-2345-455d-aa70-c87e03b15548" />

  

