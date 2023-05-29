# Netcat-NMAP-Lab
Virtual lab for practicing netcat and NMAP in the course "CEG 3585 Communications de données et réseautage" (Data Communications and Networking) for the Summer 2023 academic term with Professor Miguel Garzon. 

The followings tools were used.
- **Hypervisor:** Oracle Virtual Box
- **Linux Distribution:** Kali Linux
- **Vulnerable Machine:** Metasploitable

NOTE: The following instructions were written by me, Kien Do, in May 2023, as a self-note for learning purposes. These instructions may not be applicable in the future.

## Installation instructions
- Install VirtualBox: https://www.virtualbox.org/wiki/Downloads
- Install Kali Linux VirtualBox image: https://www.kali.org/get-kali/#kali-virtual-machines
  - Download 7-zip: https://www.7-zip.org/
  - Extract the .7z file
  - <img src="https://github.com/kienmarkdo/Netcat-NMAP-Lab/assets/67518620/7bd16831-1e26-4bac-9f47-2785c9ab86f9" width="45%"> <img src="https://github.com/kienmarkdo/Netcat-NMAP-Lab/assets/67518620/133a6f3b-30ca-4f00-93fe-3c58165907d1" width="45%">
- Install Metasploitable VirtualBox image: https://sourceforge.net/projects/metasploitable/ 
  - Extract the ZIP file

## Setup Instructions
- Add Kali Linux VM
  - Open Oracle Virtual Box (Oracle VM VirtualBox Manager)
  - Click Add
  - Select "kali-linux-2023.1-virtualbox-amd64"
  - Double click on the newly added Kali Linux VM on the left column to open it
  - To resize the window, go to the View tab -> Auto-resize Guest Display
  - Username: kali
  - Password: kali
- Add Metasploitable2 VM
  - Open Oracle Virtual Box (Oracle VM VirtualBox Manager)
  - Click New
  - Select Expert Mode
    - Name: Metasploitable -- Type: Linux -- Version: Ubuntu (64-bit)
    - Under Hard Disk, select "Use an Existing Virtual Hard Disk File"
    - Click the folder icon, navigate to your Metasploitable2 folder and select it
    - Click Finish
  - Username: msfadmin
  - Password: msfadmin
- Additional Configurations
  - On Oracle VM VirtualBox Manager
    - Tools -> 3 buttons on the right -> Network (see image below) -> NAT Networks -> Create
    - <img src="https://github.com/kienmarkdo/Netcat-NMAP-Lab/assets/67518620/0b1d2350-0d8f-45c1-adbe-d3bbf03b0f5f" width="80%">
  - Click the Kali Linux VM (kali-linux-<Version>-virtualbox-amd64) on the left column -> Settings -> Network -> Attached to: NAT Network -> Name: NatNetwork -> Ok
  - Click the Metasploitable VM on the left column -> Settings -> Network -> Attached to: NAT Network -> Name: NatNetwork - > Ok
  - <img src="https://github.com/kienmarkdo/Netcat-NMAP-Lab/assets/67518620/50f9ac7d-28d2-46e5-92da-45f44d4c910c" width="80%">

<!-- <img src="https://github.com/kienmarkdo/Netcat-NMAP-Lab/assets/67518620/a91570af-9d90-42bc-85fe-290d1207068c" width="500px"> -->
