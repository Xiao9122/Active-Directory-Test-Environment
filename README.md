# Active-Directory-Test-Environment
Built a Windows-based Active Directory test environment using Windows Server 2019, Windows 11, and Oracle VirtualBox to simulate a small business network. Configured Active Directory Domain Services, DNS, domain-joined client computers, organizational units (OUs), users, groups, and shared folders with role-based permissions.

### **Technologies Used**
+ Windows Server 2019
+ Windows 11
+ Oracle VirtualBox
+ Active Directory Domain Services
+ DNS
+ SMB File Sharing
+ Group Policy

### **Environment Overview** 
+ Domain: mylab.local
+ Domain Controller: Directory (192.168.20.10)
+ Client Workstation: Client01 (192.168.20.11)
+ Internal virtual network configured for client-server communication

### New Hire: Create user account
Right click HR then click user, add new user and fill out the information
<img width="795" height="547" alt="Screenshot 2026-06-08 194007" src="https://github.com/user-attachments/assets/1daaa52f-0be0-41a8-a803-1d48a1eb51e6" />
### Create a temporary password for the user and select user must change password at next login
<img width="797" height="555" alt="Screenshot 2026-06-08 194052" src="https://github.com/user-attachments/assets/d2ec4415-9481-4fb6-bdc9-ea57300934fc" />

### Confirm everything is correct and press finish
<img width="795" height="547" alt="Screenshot 2026-06-08 194127" src="https://github.com/user-attachments/assets/f952e495-453f-41b0-818b-e36c9db5d4da" />

### Go into Client VM and enter the temporary password and username
<img width="1007" height="842" alt="Screenshot 2026-06-08 194240" src="https://github.com/user-attachments/assets/5fd84d88-0721-4eef-8f46-7ef8a51093de" />

### Now you need to set your own password
<img width="1007" height="846" alt="Screenshot 2026-06-08 194249" src="https://github.com/user-attachments/assets/aac4f6d1-1d71-4ae4-9024-f0cca5d21b3d" />

### Set your own password and make sure it's a strong password
<img width="1005" height="842" alt="Screenshot 2026-06-08 194308" src="https://github.com/user-attachments/assets/647a04c5-02cf-40a2-814e-49d3fed35035" />

### After logging in, press Windows + R to open to the main network called Directory
<img width="966" height="785" alt="Screenshot 2026-06-08 194431" src="https://github.com/user-attachments/assets/e530190e-ea73-466d-91c1-fed08ac1e14d" />

### Try to open HR_General, Ashely does not have access to the file
<img width="970" height="787" alt="Screenshot 2026-06-08 194441" src="https://github.com/user-attachments/assets/883d3f30-e560-4bb1-9de7-1af423b32d9b" />

### Go back to Admin VM and go to Server Manager.
<img width="1351" height="637" alt="Screenshot 2026-06-08 194516" src="https://github.com/user-attachments/assets/4cbc1064-a580-4385-8736-af626d74db8e" />

### Click task and create a new share. Press next twice and create share name. Cusomize permission and disable the inheritance. Remove both the Users so only SYSTEM, Admin, and CREATOR OWNER is in Principal. Lastly, Press Create. Then press Add, Select a principal and add Ashely Baker inside
<img width="1318" height="697" alt="Screenshot 2026-06-08 194600" src="https://github.com/user-attachments/assets/9134960e-a902-4615-8e16-8c96aaf9e2ab" />

### Give Ashely the permissions that is needed and press apply
<img width="952" height="692" alt="Screenshot 2026-06-08 232859" src="https://github.com/user-attachments/assets/827df666-0ed7-47be-b390-1b8e060d6f82" />

### Going back to Ashley's VM, she now has permission to view the file <img width="920" height="737" alt="Screenshot 2026-06-08 194726" src="https://github.com/user-attachments/assets/fde5805b-48c7-43ca-b445-f3a2a1c6a165" />

### Ashely cannot access other files since she does not have permission to do so, it could be for a different department
<img width="958" height="767" alt="Screenshot 2026-06-08 194738" src="https://github.com/user-attachments/assets/08c6fc57-76d1-4ebd-85cb-8a1b5d77f74a" />









