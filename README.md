## What is the Cyber Kill Chain?

## Overview
The Cyber Kill Chain, developed by Lockheed Martin, is a framework that outlines the steps attackers take during a cyberattack. By breaking an attack into stages—Reconnaissance, Weaponization, Delivery, Exploitation, Installation, Command & Control, and Actions on Objectives—it helps defenders detect, analyze, and disrupt threats effectively. For SOC Analysts and Threat Hunters, it’s a roadmap to understanding and stopping adversaries at any point in their attack lifecycle.

![image](https://github.com/user-attachments/assets/64b44440-c948-42fb-a1f8-4f0f716aae66)

## 2. Reconnaissance 
	
- Discovering and information gathering on the system and the victim. This is the planning phase for the attack.
- Open source intelligence (OSINT) is the act of gathering and analysing publicly available data for intelligence purposes.
- Email harvesting is the email gathering process in this stage (theHarvester, Hunter.io)
	
![image](https://github.com/user-attachments/assets/13635efe-4aeb-40f5-8081-a71aec8ce492)

## 3. Weaponization

- It is the next phase after successful recon. We learn about malware, exploit and payload. Malware is malicious software, can be purchased on the Dark web, design to do harm to the computer. 
- Exploit is a program, a code that takes advantage of the vulnerability gap, flaws in the system or apps. 
- A payload is a malicious code that attacker use to runs on the system.
- And we learn about the VBA and macros. 
	
![image](https://github.com/user-attachments/assets/72307908-9752-4b74-87f2-68ee05d4aaca)
	
To answer the question and get more understanding read [_here_](https://www.trustedsec.com/blog/intro-to-macros-and-vba-for-script-kiddies)
	
![image](https://github.com/user-attachments/assets/0ef62831-9a8d-4504-964c-6f57e981820b)
		
## 4. Delivery

- The phase when attacker choose the method for transmitting payload or malware. The options are:
	○ Phishing email
	○ Distributing infected USB in public. 
	○ Watering hole attack.

![image](https://github.com/user-attachments/assets/8f92562d-eec4-45f6-b409-0a668e2035f0)
	
## 5. Exploitation
	
- We learn attackers way to exploit the vulnerability. For example phishing email link to fake login page. And creat another macro attachment - execute ransomware when open.
- We also learn about lateral move in a network In 3 phases; reconnaissance, credential dumping and  privilege escalation and gaining access to move deeper in network. 
- Some of the techniques such as Pass the Hash (PtH), Pass the Ticket, Mimikatz, keylogging.
- Zero-day


![image](https://github.com/user-attachments/assets/ee06eb21-62fa-42b4-93ed-7e2409b9e2c8)

## 6. Installation

- Persistent backdoor let the attacker access the system he hack in the past. We know a backdoor is an access point, attacker can bypass security measures and hide the access.
- Check out the Windows Persistence Room tutorials and labs to get more understanding about it.
- Installing web shell on the webserver is a way to achieved persistent backdoor. Web shell attacks on windows. 
- Meterpreter used to install backdoor on the machines-remotely and malicious code.
- Check the Registry Run Keys / Startup Folder persistence on MITRE ATT&CK
	

![image](https://github.com/user-attachments/assets/a6ade0b5-394f-41e1-8063-0596635d5b84)
	
## 7. Command & Control
	
- C2 Beaconing refers to the attackers open up the C2 channel through malware - remote control and manipulating.
- Most common C2 channels used:
	○ HTTP port 80 and HTTPS port 443 - blends the beaconing traffic with legitimate traffic  - attacker can evade firewall.
	○ DNS - the infected machines makes constat DNS request to the DNS server from attacker - so called DNS Tunneling.
	

![image](https://github.com/user-attachments/assets/a68d4c42-1d4a-4ea4-af84-3329a581f9b8)

 ## 8. Actions on Objective (Exfiltration)
	
- Exfiltration is all about:
	○ Collect the credentials from users.
	○ Perform privilege escalation (gaining elevated access like domain administrator access from a workstation by exploiting the misconfiguration).
 	○ Internal reconnaissance (for example, an attacker gets to interact with internal software to find its vulnerabilities).
	○ Lateral movement through the company's environment.
	○ Collect and exfiltrate sensitive data.
	○ Deleting the backups and shadow copies. Shadow Copy is a Microsoft technology that can create backup copies, snapshots of computer files, or volumes. 
	○ Overwrite or corrupt data.
		

![image](https://github.com/user-attachments/assets/7dcbea34-d3c6-443d-9615-b8e4a0f3979a)
		
## 9. Practice analysis

- We need to find how data breach happen and apply to build the Cyber Kill Chain of the scenario. Visit the MITRE ATT&CK for each one of these
  	- Exploit public-facing application [_for example_](https://attack.mitre.org/techniques/T1190/)
  	- data from local system
  	- powershell
  	- dynamic linker hijacking
  	- spearphishign attachment
  	- fallback channels
Fill up the form and keep trying until got the flag.

![image](https://github.com/user-attachments/assets/bab49193-9cd2-495c-a354-076b0beeb04f)

	
![image](https://github.com/user-attachments/assets/2233bc6b-2bb2-4800-be5e-15b0bf2c83ec)


We did it. Congratulation!!


![image](https://github.com/user-attachments/assets/4e78afb3-0276-4d64-8079-e7bf75d470bf)


