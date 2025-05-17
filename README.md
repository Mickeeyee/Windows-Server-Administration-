# 🖥️ Windows Server Administration 
**Installing the AD DS and DNS Roles, and Promoting the Server to a Domain Controller (DC) and Implementing Hyper-V Replication**

---

## 🎯 Objective

The goal of this exercise was to set up and configure a Windows Server to act as a Domain Controller by installing **Active Directory Domain Services (AD DS)** and **DNS Server** roles, and then promoting the server to a DC.

---

## 🛠️ Steps Completed

### 1. **Add Roles and Features Wizard**
- Selected the appropriate local server from the server pool.
- ![image](https://github.com/user-attachments/assets/a98b468b-f807-4d2c-8fb6-4e16278de9d7) ![image](https://github.com/user-attachments/assets/ef398e19-655f-4871-af8a-712d6328e9f2)
- Select Server ![image](https://github.com/user-attachments/assets/9810af50-5db1-4042-b6cf-8d276a979ecd)
- AD DS![image](https://github.com/user-attachments/assets/ec89d5db-2d4d-4f8b-bb9d-2871453ea16e)
- Installed ![image](https://github.com/user-attachments/assets/c522fda5-7af9-4c60-8864-db79fa46fda6)


### 2. **Promoted the Server to a Domain Controller**
- ![image](https://github.com/user-attachments/assets/8ad2f2a7-89aa-4658-8e5f-7a0e0ef48fba)
- AD DS and DNS SERVICE added to the SERVER MANAGER and Promoted as a DOMAIN CONTROLLER ![image](https://github.com/user-attachments/assets/4ad2b7e8-a2e6-48d0-9580-c13b69fb039c)
- ![image](https://github.com/user-attachments/assets/700be8cd-c81f-416d-9c5e-b2a34b5b96df) 

### 3. **Implementing Hyper-V Replica and Win¬dows Server Backup**
---Remote Powershell Desktop by Commands ![image](https://github.com/user-attachments/assets/e4b8d7cf-0977-4125-b147-2c75a07b2717)
VMReplicationServer ![image](https://github.com/user-attachments/assets/fc2ac9c8-e778-439b-9b06-f293b0bca5f4) 
Hyper-v machine created on WINDOWS22 where I am reomote connected ![image](https://github.com/user-attachments/assets/27448602-8269-46dc-8748-9aafe67daa83)
Get-VM shows the vm Available on remote server we are connected to ![image](https://github.com/user-attachments/assets/89985436-24d5-4b2f-862d-308fcf1ae7f7)
Connected Remote desktop to my other SERVER (WINS22) from WINDOWS22 and ran commands:![image](https://github.com/user-attachments/assets/f9e9f39f-b670-4d8a-973b-a831e2954fa8) 
![image](https://github.com/user-attachments/assets/7e04c73c-909a-4c34-b9a7-d062d7afc1d6)
Start-VMInitialReplication n WINDOWS22 and Successfully Replicated the Hyperv Machine on my other Server WINS22 ![image](https://github.com/user-attachments/assets/3b553c26-02a0-4bc8-9aa5-b883907f396c)
Replicated Machine on WINS22: Replication Successful ![image](https://github.com/user-attachments/assets/0751512d-444d-462e-bb1e-115c63901561)
Enabled Replication from WINS22 to WINDOWS22 and Replicated New Machine Named MBB1 to WINDOWS22  ![image](https://github.com/user-attachments/assets/9656f102-8508-497f-a694-1b9e8099acc5)
![image](https://github.com/user-attachments/assets/78c57c06-c4e0-4efb-b4ee-b15135485ec3)














## 📂 Tools and Services Enabled

- ✅ **Active Directory Users and Computers**
- ✅ **DNS Manager**
- ✅ **Active Directory Domains and Trusts**
- ✅ **Group Policy Management**
- ✅ **Server Manager Dashboard Integration**
- ✅ **Hyper-v Replication**

---

## ✅ Outcome

The server was successfully transformed into a Domain Controller with both **AD DS** and **DNS roles** fully operational. All relevant administrative tools were made available, enabling full domain control, user management, and policy enforcement.


