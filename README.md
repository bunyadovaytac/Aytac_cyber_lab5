# Aytac_cyber_lab5
# 🛠️ System Hacking Lab Report – Gaining and Maintaining Access

## 🔍 Step 1: Host Discovery & Scanning
Screenshot 1 – The attacker machine (Kali) network configuration is shown to identify the local IP address.
<img width="653" alt="Screenshot 1" src="https://github.com/user-attachments/assets/5754ab45-5359-4526-af78-f007db5d0954" />

Screenshot 2 – The target machine (Metasploitable) IP address is confirmed using ifconfig.
<img width="699" alt="Screenshot 2" src="https://github.com/user-attachments/assets/d467f492-b067-4f3e-81ab-15a76374b14a" />

Screenshot 3 – Nmap scan reveals open ports and services such as FTP, SSH, Telnet, and Apache on the target system.
<img width="801" alt="screenshot 3" src="https://github.com/user-attachments/assets/1bb27154-979b-479f-99ef-6c90c855f313" />


## 💣 Step 2: Exploiting a Vulnerable Service with Metasploit
Screenshot 4 – Metasploit Framework is launched on the attacker machine.
<img width="653" alt="Screenshot 4" src="https://github.com/user-attachments/assets/8bbddf49-1a7f-4bcf-b848-1c2c45db13f0" />

Screenshot 5 – The vsftpd_234_backdoor exploit is found using Metasploit’s module search.
<img width="840" alt="Screenshot 5" src="https://github.com/user-attachments/assets/b992da0a-079a-47e1-bb5e-d1901d19f956" />

Screenshot 6 – The exploit is configured and successfully executed, giving a root shell on the target machine.
<img width="756" alt="Screenshot 6" src="https://github.com/user-attachments/assets/7f76b9eb-4358-4f05-8d16-71eedf08d2fa" />

## 🔍 Step 3: Post-Exploitation Enumeration
Screenshot 7 – Commands like whoami, id, and ls are run to gather information about the compromised system.
<img width="735" alt="Screenshot 7" src="https://github.com/user-attachments/assets/534387f0-510b-4cfb-9481-a14078cf0438" />

## ⬆️ Step 4: Privilege Escalation
Screenshot 8 – The attacker views the /etc/shadow file, confirming root-level access.
<img width="539" alt="Screenshot 8" src="https://github.com/user-attachments/assets/bd103a53-4a39-4ff3-9186-f05ce5f3be74" />

## 🪜 Step 5: Persistence
Screenshot 9 – A persistent user backdooruser is created with shell access and password.
<img width="533" alt="Screenshot 9" src="https://github.com/user-attachments/assets/f29914ce-9d09-4ed4-a7bd-8fe0c30aa7db" />

Screenshot 10 – Persistence is verified by logging in to the target via SSH as backdooruser.
<img width="648" alt="Screenshot 10" src="https://github.com/user-attachments/assets/1e09a887-a962-4bb9-b00c-b89425f86812" />
