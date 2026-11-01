# 🛜🐧 A streamlined utility for capturing 4-way handshakes and executing wordlist attacks.

### INTRODUCTION

* As a Class 11 student, navigating the engineering landscape, This repository is based on how to Capture a 4-Way Handshake of **IEEE 802.11i (WPA2-PSK)** Architecture and Analysing it through Wireshark and proceed with a **BRUTE-FORCE** Dictionary attack to get the Password !!!

* Rather than Showing how to Execute Command, this Documentary Ensures a deep Understanding of the approach of the Attack to the Reader of this Repository, With the prerequisites needed too !!!

* This project is a definitive piece of my portfolio for the **B.Cyber selection program hosted by IIT Kanpur and IIT Madras**, serving as explicit, documented evidence of my prior foundational work in network infrastructure analysis and practical security engineering.

🚫 ### DISCLAIMER !!!!

**IMPORTANT NOTICE:**  The contents, code snippets, methodologies, and technical documentation in this repository are solely and strictly for **educational purposes, defensive research, and academic evaluation** ONLY !!!!!
* **Authorized Testing Only:** The entire wireless auditing sequence including interface monitoring, packet sniffing, frame injection, and cryptographic dictionary attacks was executed inside a isolated, private laboratory environment the AUTHOR OWNS !!
*  All network infrastructure, access points, and client devices utilized during this project are owned entirely by the ME
* **Compliance with Legal Frameworks:** Unauthorized interception of wireless data networks, executing deauthentication frame injection against third-party hardware, or attempting to crack security credentials without explicit owner consent is illegal.
* **In India, such actions violate the **Information Technology Act, 2000 (Section 43 and Section 66)** and can lead to severe criminal prosecution and financial liabilities.**
* **Zero Liability:** The author assumes absolutely no responsibility or liability for any misuse, damage, systemic disruption, or illegal deployment of the technical information documented within this repository.
***NOthing here is AI-GENERATED, it,s my sole hand typing and my Knowledge and practical Documentary rather than Copy pasting.....However , the Law Details and Disclaimer are searched for in the google....***
  
                    ---
***LET,S BEGIN !!!!***

**TOOLS-NEEDED**
* [WIFI-ADAPTER](https://www.tp-link.com/in/home-networking/adapter/tl-wn725n/) (Supports, Monitor Mode & Packet Injection with proper DKMS drivers !!!)

* [KALI LINUX](https://www.kali.org/) (Not Necessary!!, But i love this, as Kali is Built for ETHICAL HACKING !!!)
* [Aircrack-ng](www.aircrack-ng.org)
* [Airodump-ng](https://www.aircrack-ng.org/doku.php?id=airodump-ng)
* [Aireplay-ng](https://www.aircrack-ng.org/doku.php?id=aireplay-ng)
* [Wireshark](https://www.wireshark.org/)
* [ROCK-YOU WORDLIST](https://weakpass.com/wordlists/rockyou.txt) (YOU CAN CREATE YOUR OWN WORDLIST TOO!!! ENSURE YOUR WORDLIST CONTAINS THE PASSWORD!! THAT SHOULD BE THE QUALITY OF THE WORDLIST YOU CHOOSE!!)
  
### THE FLOW....
* I will be using 2 Wifi adapters of kind i mentioned before as i believe **DEAUTH-ATTACK** is far more Successful when i dedicate one for the attack while the other one to listen for the Handshake !!!
* Firstly, we would be Enabling the **MONITOR MODE** for the tools we use to spit out HUMAN READABLE data instead of machine code which the tools can,t interpret..
* Secondly, we would launch the **Airodump-ng** tool to first get the necessary informations (ESSID, CHANNEL, Captured file,s name for easy access)
* Thirdly we would be again launching the same tool, but this time, we would be forcing the tool to listen and capture the Handshake because of the attack and save as a file we need later for Wireshark tool
* Next, we would open the captured handshake in wireshark for checking whether the handshake captured is healthy in order to further get it into the Dictionary Attack
* Lastly we would be launching a Dictionary Attack against the Rockyou.txt Wordlist for matching the keys and successfully getting the password
* And HENCE WE WOULD ACHIEVE WHAT WE NEED !!!

### STEP 1 (Configuring INTERFACES to MONITOR MODE)
* firstly check whether the Devices are connected to the Operating system...this can be done in linux by entering "lsusb" in the terminal



