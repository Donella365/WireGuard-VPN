# WireGuard-VPN
This project demonstrates the implementation of a self-hosted VPN using WireGuard on a DigitalOcean VPS. The VPN provides secure remote access, encrypted communication, and private tunneling for client devices.

## Objectives
- Deploy a VPS on DigitalOcean as the VPN server.  
- Install and configure WireGuard.  
- Generate and manage server/client key pairs.  
- Enable IP forwarding and NAT for outbound traffic.  
- Create reusable configuration templates for multiple clients.  
- Document the setup for reproducibility and portfolio demonstration.

  

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

  Made SSH key using the terminal (could also use puTTY)

  <img width="620" height="283" alt="Screenshot 5" src="https://github.com/user-attachments/assets/65b35f37-bf3e-4ead-bacf-ea381d35321c" />

  Added SSH key (recommended) (could also use a strong root password)

  <img width="597" height="169" alt="Screenshot 6" src="https://github.com/user-attachments/assets/b49cfbdf-9a16-4530-a242-40c358d0ebbf" />

  <img width="588" height="406" alt="Screenshot 7" src="https://github.com/user-attachments/assets/0df061b9-0024-410e-a7d1-cca9ff439864" />

  Opened the pub file with notepad as my preferred text editor
  
  <img width="620" height="297" alt="Screenshot 8" src="https://github.com/user-attachments/assets/dad4d046-c4e0-45c5-863f-afc7826e8fc3" />

  Copy the text and inserted it on digital ocean. Gave it a name.
  
  <img width="611" height="539" alt="Screenshot 9" src="https://github.com/user-attachments/assets/1b783d41-df1d-4b29-8aaa-0e71babd860c" />

  <img width="595" height="204" alt="Screenshot 10" src="https://github.com/user-attachments/assets/a73a4003-2133-4811-b7d5-93011d65cb92" />

  Added payment method and created droplet. 

  <img width="661" height="121" alt="Screenshot 11" src="https://github.com/user-attachments/assets/0704d8cb-8460-4f6d-88ab-27a7c7e6f0cc" />

  Once it finished loading I got the external IPv4 address. Then SSH into the droplet. Ssh root@your_droplet_ip
  
  <img width="880" height="179" alt="Screenshot 13" src="https://github.com/user-attachments/assets/052c55ec-8a58-4463-a0a8-3d5caa761ba9" />

  Updated & installed wireguard. 

  <img width="259" height="39" alt="Screenshot 14" src="https://github.com/user-attachments/assets/a0c2c606-1d52-4b0b-84f0-6f91b3bd15cf" />

  Made server and client keys.

  <img width="626" height="40" alt="Screenshot 15" src="https://github.com/user-attachments/assets/6306ef09-274a-4e58-b03c-2cf34c9c324f" />

  <img width="579" height="42" alt="Screenshot 16" src="https://github.com/user-attachments/assets/87d64bc4-1b66-43cb-88c5-62784ea0d72a" />

  Configured the Server:
    Create WireGuard config file at 
    /etc/wireguard/wg0.conf:

    
    <img width="940" height="464" alt="Screenshot 17" src="https://github.com/user-attachments/assets/094cf5d6-e90f-4145-8556-e89a65489e2a" />

  Configured iptables: 
  
  Configured the Client:

  <img width="585" height="494" alt="Screenshot 12" src="https://github.com/user-attachments/assets/469c243b-f2ef-41a4-8e9c-3bd69501b8f8" />

  Upped the wireguard interface in the command line:


  Turned on the VPN:


  Tested the VPN on the clinet to confirm everything is working

  

