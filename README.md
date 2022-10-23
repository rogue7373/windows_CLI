# windows_CLI
### Network Information
#### Find the IP address information
~~~
ipconfig
~~~
#### Find the IP address and all related information for all Network adapters
~~~
ipconfig /all
~~~
#### Find the DNS information for the Network Adapters
~~~
ipconfg /all | findstr DNS
~~~
#### Release the current IP addressing for ALL Network Adapters
~~~
ipconfig /release
~~~
- Releases current IP address from use
#### Renew All IP addressing for ALL Network Adapters
~~~
ipconfig /renew
~~~
- Refreshes the IP address with new IP address from the DHCP server
#### Release the current IP addressing for the selected Interface
~~~
ipconfig /release "INTERFACE"
~~~
- Specify which adapter to release the IP address for by using "INTERFACE" example: "Wi-Fi"
#### Display DNS information for all Network Adapters
~~~
ipconfig /displaydns
~~~
- Shows DNS server in use
#### Copy the DNS informatino for ALL Network Adapters and copy it directly to the clipboard. 
~~~
ipconfig /displaydns | clip
~~~
- Copies all DNS information to clip board
#### Flushes the DNS Cache for ALL Network Adapters
~~~
ipconfig /flushdns
~~~
- Flushes DNS cache 
### NSLOOKUP
#### Look up DNS information for a chosen Domain 
~~~
nslookup google.com
~~~
- Provide basic IP information for specified domain
#### Look up DNS information for a chosen Domain using a specified DNS Server
~~~
nslookup google.com 8.8.8.8
~~~
- Specifies the IP information for specified domain using a specific DNS server
#### Look up DNS Records information such as; MX, TXT, and PTR
~~~
nslookup -type=mx 
~~~
- you can use regular DNS record choices here
#### Clear your current screen in CMD/Terminal/Powershell
~~~
cls 
~~~
- clear screen
#### Find MAC address information 
~~~
getmac /v 
~~~
- Show MAC address

### Power
#### Power Config / Energy Check
~~~
powercfg /energy
~~~
- copy output html file back to cmd prompt and webpage will open with stats
#### Power Config / Battery Check
~~~
powercfg /batteryreport
~~~
- copy output html file back to cmd prompt and webpage will open with stats
#### Check File Type Assocatiated to an Application (Default applications)
~~~
assoc
~~~
- shows file type associations with programs 
- change file types with "assoc" | assoc .mp4=VLC.vlc
### Disc managment 
#### Check Disk
~~~
chkdsk /f
~~~ 
#### Check Disk Repair
~~~
chkdsk /r 
~~~
#### Scan 
~~~
sfc /scannnow
~~~
~~~
DISM /Online /Cleanup-Image /ScanHealth
~~~
~~~
DISM /Online /Cleanup-Image /RestoreHealth
~~~
~~~
tasklist | findstr script
~~~
~~~
taskkill /f /pid 
~~~

### NETSH
~~~
netsh wlan show wlanreport
~~~
~~~
netsh interface show interface
~~~
~~~
netsh interface ip show address | findstr "IP Address"
~~~
~~~
netsh interface ip show dnsservers 
~~~
~~~
netsh advfirewall set allprofiles state off
~~~
~~~
netsh advfirewall set allprofiles state on
~~~
### Network Troubleshooting 
~~~
ping google.com
~~~
~~~
ping -t google.com 
~~~
~~~
tracert google.com 
~~~
~~~
tracert -d google.com
~~~
~~~
netstat 
~~~
~~~
netstat -af
~~~
~~~
netstat -o 
~~~
~~~
netstat -e -t 5 
~~~
~~~
route print 
~~~
~~~
route add 192.1.1.1. mask 255.255.255.255 
~~~
~~~
route delete 192.1.1.1
~~~
~~~
shutdown /r /fw /f /t 0 
~~~
- restarts to system bios 
