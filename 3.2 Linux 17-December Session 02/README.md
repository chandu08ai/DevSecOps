What is Computer? 

What is Client Server Architecture? 

To buy a Phone, Computer, etc. we check
- RAM
- Storage
- OS
- Processor


**Server:**
- To host an Application

Port Forwarding: 
- You can deploy application in your laptop and open it in internet

facebook.com --> facebook application in fb servers 
browser: --> client software 


**AWS:** 
- Region: Hyderabad, Mumbai, Singapore, US, EU, etc
- AZ: North Hyderabad, South Hyderabad --> minimum 2 AZ --> High Availability


- Instance == Server == Node
- Firewall == Security Group
- Allow everyone through firewall
- Inbound --> incoming traffic
- Outbound --> Outgoing traffic
- 0.0.0.0/0 --> All Traffic


devops-practice --> AMI --> Amazon Machine Image --> ISO 

.iso --> it will create entire operating system --> C:/Windows 

Redhat Enterprise Linux == Centos == Amazon Enterprise Linux == Fedora == AlmaLinux 


Kernel == Brain of OS == C language 
- User Interface

Linus Torvalds 
- Inventor of Linux
- Mac --> Hardware Locking --> you are buying both hardware and Mac OS
- 1980's, Servers uses Unix OS, Laptops uses IBM BIOS 
- He developed Linux from the scratch from C language, which is called Kernel
- Kernel --> used to connect with Hardware
- OS == Kernel + User Interface
- He made it Open source

**Linux Implementations:** == **Distributions** == **Flavours**
- RHEL --> Commercial 
- IBM AIX
- Ubuntu
- Fedora
- Solaries
- Suse
- Android

**Opensource VS Enterprise:**


AWS Instance: 
- AWS Linux 2023 AMI
- t3.micro/t2.micro

**Authentication:**
- What you know --> Username and Password
- What you have --> Username and token/OTP
- What you are --> Fingerprints, Retina, Palm, etc

**Public key and Private Key:**
- Lock and Key
  - Lock --> Public
    - Server IP (Publickey will be placed here) 
  - Key --> Private
    - Provided to authorized people

Creating Public and Private key: 
- ssh-keygen -f <file-name> --> it will create public and private key 

Git bash: 
- To run the above command, we need to install Git bash

pwd: 
- Present Working Directory
- C:\Users\<your-username> --> Windows
- /c/Users/siva --> Linux

Git Bash == SSH Client == Git Clinet == Mini Linux 

~ --> Home Directory 

ls -l --> List sub directory 

ssh-rsa
ssh-ed25519
- both are public keys

.pub --> public key 
.pem --> private key 

pubic IP --> 184.72.71.255 
AWS Linux 2023 AMI --> ec2-user
password --> our private key

To connect to an instance we need 
- IP
- Username
- Password
- Protocol
- Port
EX: facebook.com
- HTTPS, facebook.com/IP, username, password, 443
- Linux Server/IP, Username, Password/Privatekey, SSH, 22
- SSH --> SecureShell 22 --> it will give full access to the server

To Connect to the instance: 
- ssh -i daws-82.pem ec2-user@184.72.71.255
- 











