
**Absolute Path VS Relative Path:**
Absolute Path: 
- /c/devops/daws-82s/daws-82s.pem --> Absolute path
Relative path:
- you are in devops folder
- daws-82s/daws-82s.pem --> Relative path

$ --> denotes normal user 

sudo su ==> root access in the current user folder

\# --> denotes admin/root user 

/home/<user-name>

sudo su - ==> root access, lands in root user home directory i.e. /root

/root --> root user home folder 


Commands in Linux: 

**uname:**
- prints the kernel name
- EX:
  - Linux
- uname -a
- uname --all


<command-name> <options> <inputs>
- \- ==> we can give single char
- -- ==> we need to give word


/ --> root of the server


**ls:**
- list the sub directories

ls -l: 
- long listing format with more details 

ls -lr: 
- reverse alphabatical order

ls -lt: 
- new files on top

ls -ltr: 
- old files on top

ls -ltrh: 
- human readable

ls -la: 
- display all files including hidden files and folders

drwx------ ==> d means directory
-rw-r--r-- ==> - means file 
lrw-r--r-- ==> l Link files 

**touch:**
- to create empty file
- touch <file-name>
- EX:
  - touch devops.txt


**cat:**
- cat > devops.txt ==> enter the text, once done Enter and press ctrl+d
- cat devops.txt ==> to display the text in the file
- cat >> devops.txt ==> append, adds to the current text
- \> ==> replaces the existing text with new text
- \>> ==> append, adds to the current text


**mkdir:**
- Creates directory
- mkdir <name>

**rmdir:**
- removes only empty directory
- rmdir devops/

**rm -r:**
- rm -r devops
- \-r means recursively delete everything inside devops

**rm:**
- rm devops.txt --> deletes the file

**rm -rf**: 
- rm -rf Devops.txt --> removes the file forcefully, even when the file is open 


cp <source-file> <destination>
- cp DevSecOps.txt devops
- copying DevSecOps.txt file to devops folder


**curl and wget:**
- wget <URL> --> downloads the file
- curl <URL> --> Shows the content on the screen 
- curl <URL> -o <path> --> downloads the file with name given




**Piping:** 


**grep:** 
- grep <word-to-search> <file>
- EX:
  - grep ec2-user passwd

- Piping with grep:
  - cat passwd | grep ec2-user
  - | ==> pipe


**cut:**
https://github.com/chandu08ai/DevSecOps/3.3 Linux 18-December Session 03/README.md
/ ==> **seperator/delimiter/fragments**

echo "https://github.com/chandu08ai/DevSecOps/3.3 Linux 18-December Session 03/README.md" | cut -d "/" -f1
- https:


echo "https://github.com/chandu08ai/DevSecOps/3.3 Linux 18-December Session 03/README.md" | cut -d "/" -f2
- 

echo "https://github.com/chandu08ai/DevSecOps/3.3 Linux 18-December Session 03/README.md" | cut -d "/" -f3
- github.com

echo "https://github.com/chandu08ai/DevSecOps/3.3 Linux 18-December Session 03/README.md" | cut -d "/" -f4
- chandu08ai


**awk:**
echo "https://github.com/chandu08ai/DevSecOps/3.3 Linux 18-December Session 03/README.md" | awk -F "/" '{print $1F}'
- https:

echo "https://github.com/chandu08ai/DevSecOps/3.3 Linux 18-December Session 03/README.md" | awk -F "/" '{print $NF}'
- README.md


How can i get all the users in Linux Server? 
- awk -F ":" '{print $1F}' passwd
- <img width="747" height="642" alt="image" src="https://github.com/user-attachments/assets/89d29257-dde7-4fcc-bc1b-7f8cd9b98ec4" />
<img width="748" height="635" alt="image" src="https://github.com/user-attachments/assets/1e403b2f-9b8c-4eaa-bc8f-835617347c77" />


**head:**
- head passwd --> top 10 lines from top
- cat passwd | head -n 3
- head -n 3 passwd

**tail:**
- tail passwd --> last 10 lines from bottom
- tail -n 4 passwd --> last 4 lines from bottom

4-10 lines: 
- head -n 10 passwd | tail -n 7


**find:**
- find <which-location> -name "<file-name>"
- find / -name "passwd"
- find / type -d -name "ec2-user"









