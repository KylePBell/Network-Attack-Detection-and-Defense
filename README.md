# Network Attack Detection and Defense

## Objective

In this scenario, I'm using a home lab set up to monitor network traffic on Ubuntu OS and defend against a simulated attack coming from Kali OS.

### Skills Learned

- Monitoring network traffic using Wireshark.
- Simulating a TCP dump attack.
- Ability to generate and recognize attack signatures and patterns.
- Enhanced knowledge of network protocols and security vulnerabilities.

### Tools Used

- Wireshark
- Ubuntu
- Kali
- Oracle VM VirtualBox

## Steps

In this project, I simulated an attack using Kali a server. I then captured the network traffic using wireshark within the Ubuntu server. *Ref 1*

![Screenshot 2024-06-30 165200](https://github.com/KylePBell/Network-Attack-Detection-and-Defense/assets/174375217/3cd8df84-0983-4dee-b996-d397d94a9a83)
*Ref 1: Network Diagram*

1) The first step included finding the IP address of both servers using the command "ip a" *Ref 2&3*

![Screenshot 2024-07-01 150725](https://github.com/KylePBell/Network-Attack-Detection-and-Defense/assets/174375217/d46ae8fa-0f85-454a-8d35-cb656dd09d2a)
*Ref 2*
![Screenshot 2024-07-01 150807](https://github.com/KylePBell/Network-Attack-Detection-and-Defense/assets/174375217/35303f3a-4c0e-457b-9747-f575284cef89)
*Ref 3*

2) I then configured a simple Uncomplicated Firewall on Ubuntu and allowed incoming SSH connections. *Ref 4&5*

![Screenshot 2024-07-01 151702](https://github.com/KylePBell/Network-Attack-Detection-and-Defense/assets/174375217/4a50660c-1905-49ab-9c44-3f1902338cc6)
*Ref 4*
![Screenshot 2024-07-01 151749](https://github.com/KylePBell/Network-Attack-Detection-and-Defense/assets/174375217/59053d39-8dc4-4031-a904-080273e7585e)
*Ref 5*

3) Once the firewall was active, I simulated in attack in Kali using the command "nmap -A (IP address)". This command enables the TCP connection to the Ubuntu host. *Ref 6*

![Screenshot 2024-07-01 150913](https://github.com/KylePBell/Network-Attack-Detection-and-Defense/assets/174375217/c4bd68e0-f1f1-41fa-9be1-727f4540f138)
*Ref 6*

4) Finally, I open Wireshark in Ubuntu using the command "sudo wireshark" (after installing it) and capture the attack live. *Ref 7*

![Screenshot 2024-07-01 152016](https://github.com/KylePBell/Network-Attack-Detection-and-Defense/assets/174375217/43911de8-9b29-4a8f-82ee-bf3c9daff20c)
*Ref 7*

