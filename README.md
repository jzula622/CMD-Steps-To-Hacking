# CMD-Steps-To-Hacking

CMD:Changing your IP address can be useful for a variety of reasons. If you need to change yours, type:

ipconfig /release

ipconfig /renew

The first command releases your current IP address, the second command gets a new IP address for your machine.

Clearing your computer's DNS can be used whenever a site changes its IP address so you won't be misled. Write and enjoy a clean start.

ipconfig /flushdns

You can find out if packets can be delivered to a device with the ping command. Just type or change URL and IP ADDRESS in Command and packages will be sent. If you bring them back you will make sure everything works fine.

ping URL


ping IP ADDRESS

Pc  close:
If you want to shut down the other party's PC, type shutdown -f in the .txt file, write the file .bat and send it to the target, then the target's PC will shut down in 1 minute (there will be no reset, only one device will shut down

CMD hash operation:

Scanning and Repairing Files
To scan and repair files on your computer, type:

sfc /scannow

and press Enter. The time this task will take depends on how fast your computer is. This can easily take up to an hour.

Manage Your Computer's Energy
There are various things you can see on your computer with the powercfg command. For example, using the command

powercfg /a

You can view the sleep states of your computer.

Powercfg can also let you do things like:

powercfg /list – Shows all power schemes in the current user's environment

powercfg / energy – After observing your computer for 60 seconds, it will generate an HTML report with data about your computer's energy efficiency.

powercfg / sleepstudy – If your device supports InstantGo devices and applications, you can find out which ones wake your computer using this command.

powercfg / query – Returns a subset of power settings GUID.

Assoc
The files are associated with a specific program in Windows. When you open a program, certain files open automatically. If you want to associate these files with a program, you can use the assoc command.

By typing Assoc at the command prompt, you can see a list of program associations and filename extensions. Suppose you want text files to be associated with something else:

assoc.txt = “APPLICATION NAME”

(Replace “APPLICATION NAME” with the full application name.)

Hide Folders
If there is a folder with sensitive information, you can hide it using this simple command. Type the drive where this file is located and then type

attrib + h + h + r

Then enter the name of the folder you want to hide.

Get a List of Your Computer's Drivers
Find out if you have installed this driver using the driverquery command. Press Login once entered; you will see a list of every driver on your computer. You'll see information such as Connection date, Name, and Type.

Find Shared Folders
To see the folders you have shared, simply type the command

net share

and press Enter. The command will also show shared names

Running cmd commands as Administrator
Using this command you can run any command as an administrator even if the person using the computer does not have this privilege.

runas /user:yourdomain\admin cmd

and then make some changes.

Add your real domain name and add your admin to a Domain Admin's real username. Replace CMD with the command you want to try and you can run as administrator regardless of who is logged in.


Most Used (CMD) Hacker Codes
cmd commands
ping 192.168.0.2 ===> Tests the connection by sending and receiving small data packets to the other computer on the ip
ping client98
ping -a 192.168.0.2 ===> Tests the connection by sending and receiving small data packets to the other computer on the ip. With the “-a” parameter, the address of the computer on the ip is displayed.
ping -a -n 20 192.168.0.2 ===> It is tested by sending data packets equal to the value next to the -n parameter.
pathping ===> With this command, it is checked whether the data passing over the routers is lost or not.
ipconfig ===> shows the computer's ip address on the network.

ipconfig /all ===> shows the computer's ip address on the network and many extras.
ipconfig /all >sovereign.txt ===> dumps all spilled information into sovereign.txt file.
ipconfig /release ===> releases the computer's ip from the network
ipconfig /renew ===> renews the computer's ip on the network. During the renewal process, first “release”, then “renew” is applied.
ipconfig /registerdns ===> is used to register the computer name and ip to DNS.
ipconfig /flushdns ===> It deletes the information about name and ip address matches that DNS clients keep in their cache memory, frees cache memory. (Used to solve problems)
ipconfig /displaydns ===> If the computer you are using is also a DNS client, it allows the IP addresses in the DNS Cache memory and their DNS names to be displayed.
arp -a ===> shows the ip resolution in the cache. If there is no new ip resolution within 2 minutes, the cache will clear itself. If refreshed within 2 minutes, it will be held for another 10 minutes.
arp -a 192.168.0.2 ===>
arp -s 192.168.0.2 00-02-44-12-24-ad ===> Fixes the "mac" address of the computer whose ip si is given in ip resolution. cache also remains permanently, not deleted.
–
net use ===> shows the maps on the computer.
net use h: \\\\client98\\c ===> maps client 98 computer's C to H.
net use h: \\\\192.168.0.2\\cş ===> maps the hidden admin share of the given computer as h.
net use /delete h: ===> deletes the h mapped drive.
net use lpt1: \\\\server\\ibm /persistent ===> provides permanent printer connection.
netstat ===> shows connections made to the computer.
nbtstat ===> It allows to show NetBIOS API related data on TCP/IP. It enables Netbios name table to be shown both for the computer you use (local) and for other computers on the network (remote).
nbtstat -RR ===> If you are running the command on a WINS client, the WINS Client will first delete the self-registers on the WINS server; then it will re-register. (Used to fix the problem)
tracert 131.107.10.1 ===> Thanks to this command, ICMP packets are sent to the same destination using different TTL times. In this way, it is checked which paths our packets follow while reaching another destination from your computer.
With this command, a list of routers that determine the closest and shortest path between the target computer and you will be displayed.
tracert [-d][-h Maximum Hops][-J Hot List][-w Timeout][Target name]
route print ===> Dumps the routing table.
net helpmsg 52 ===> dumps the description of the error codes.
net view ===>
net view \\\\192.168.0.2 ===> Shows the shared objects of the computer with ip si.
net view \\\\client98 ===> shows the shared objects of the named computer.
net share ===> shows the shared drives and folders on the computer.
net share hoop=f:\\hoop ===> Shares the hoop folder we created on the f drive with the same name.
hostname ===> shows the name of the computer.
%username% ===> is the username with your computer logon.
%systemroot% ===> is the folder where the operating system is installed.
%userprofile% ===>
net time \\\\192.168.0.2 ===> Shows the date and time of the computer with the ip entered.
net time \\\\client98 ===> shows the date and time of the computer whose name is entered.
net time \\\\client98 /set /y ===> sets the machine we are using according to the date and time of the named computer.
convert c: /fs:ntfs ===> Converts drive C to NTFS system. The information in it is not deleted.
net help command ===> displays a description of all commands linked to the net command.
secedit /refreshpolicy user_policy ===> It is used to take effect immediately on the basis of the changes made in the policies.
secedit /refreshpolicy machine_policy ===> It is used to enable the changes made in the policies to take effect immediately on a computer basis.
secedit /refreshpolicy user_policy /enforce ===> Forces policy changes to take effect immediately.
secedit /refreshpolicy machine_policy /enforce ==> Forces policy changes to take effect immediately.
nslookup ===> Checks if DNS is working properly.
The nslookup command is entered and then:
ls -t SRV mcseankara.com (checks SRV records)
ls -t SRV mcseankara.com > sovereign.txt (It puts SRV records into sovereign.txt file and it should be 24 records)
192.168.0.1 (reverse lookup in

