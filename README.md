## Hack Captive portals script

This script is using MAC-spoofing technique. This method is the only one which is present in all wireless and some wired  
Captive portals by design. Once a host is authorized by the Captive portal, its MAC and IP address are allowed  
unrestricted access.  
All we need to do is sniff traffic on the network, find a host that is authorized, and spoof its IP and MAC address.  
Spoofing a MAC is dependent on your network card and driver but most modern network devices today support it.  
The downside of course is that you have to observe someone already authenticated, but in places such as a crowded airport  
lobby this may be less difficult than it seems.  

<p align="center">
    <img src="./screenshot.png" alt="Hack Captive portal">
</p>

### Installation and usage
You need `sipcalc` and `nmap` for this script. Then download .sh script and run it. 
```
sudo apt -y install sipcalc nmap
wget https://raw.githubusercontent.com/systematicat/hack-captive-portals/master/hack-captive.sh
sudo chmod u+x hack-captive.sh
sudo ./hack-captive.sh
```

> Tested in Ubuntu 16.04 with different Captive portals in airports and hotels all over the world.

### How to run the Bash file in Window
Open Command Prompt or powershell and navigate to the folder where the script file is available.
Type 
```
curl https://raw.githubusercontent.com/systematicat/hack-captive-portals/master/hack-captive.sh -O script-filename.sh
Bash script-filename.sh 

#Change the "script-filename" to the name of the .sh file.
```
and then hit the enter key.


### [**How to run the Bash file in Android Device**](https://github.com/Isomkevin/Running-Shell-Script-in-Android)



### With Help from:
> https://en.kali.tools/?p=724

> https://kalitut.com/how-to-bypass-captive-portal-hotspot/
