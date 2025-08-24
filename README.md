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

### Deployed VPS on Digital Ocean
  Logged into Digital Ocean (https://www.digitalocean.com/) and spun up a virtual machine/droplet. 
  <img width="670" height="329" alt="Screenshot 2025-08-21 153337" src="https://github.com/user-attachments/assets/34cf2bf3-2345-455d-aa70-c87e03b15548" />
  
  Selected closest region
  
  <img width="652" height="154" alt="Screenshot 2" src="https://github.com/user-attachments/assets/9479934f-2619-45b0-ac81-4228b73cdceb" />

  Selected Ubuntu server
  
  <img width="633" height="245" alt="Screenshot 3" src="https://github.com/user-attachments/assets/ff6b35fd-3e97-40b7-ba83-3e5013515d15" />

  Basic size, regular CPU, $6/month for a droplet. 
  
  <img width="623" height="322" alt="Screenshot4" src="https://github.com/user-attachments/assets/312e734f-a6c9-4060-ad73-5c36d1e12772" />





