# windows_CLI
### Network Information
#### ipconfig
#### ipconfig /all
#### ipconfg /all | findstr DNS
#### ipconfig /release
#### ipconfig /renew
#### ipconfig /release "INTERFACE"
#### ipconfig /displaydns
#### ipconfig /displaydns | clip
#### ipconfig /flushdns
#### nslookup google.com
#### nslookup google.com 8.8.8.8
#### nslookup -type=mx 
- you can use regular DNS record choices here
#### cls 
- clear screen 
#### getmac /v 
- Show MAC address
### Power
#### powercfg /energy
- copy output html file back to cmd prompt and webpage will open with stats
#### powercfg /batteryreport
- copy output html file back to cmd prompt and webpage will open with stats
#### assoc
- shows file type associations with programs 
- change file types with "assoc" | assoc .mp4=VLC.vlc

### Disc managment 
#### chkdsk /f 
#### chkdsk /r 
#### sfc /scannnow
#### DISM /Online /Cleanup-Image /ScanHealth
#### DISM /Online /Cleanup-Image /RestoreHealth
#### tasklist | findstr script
#### taskkill /f /pid 

### NETSH
#### netsh wlan show wlanreport
#### netsh interface show interface
#### netsh interface ip show address | findstr "IP Address"
#### netsh interface ip show dnsservers 
#### netsh advfirewall set allprofiles state off
#### netsh advfirewall set allprofiles state on

### Network Troubleshooting 

#### ping google.com
#### ping -t google.com 
#### tracert google.com 
#### tracert -d google.com
#### netstat 
#### netstat -af
#### netstat -o 
#### netstat -e -t 5 
#### route print 
#### route add 192.1.1.1. mask 255.255.255.255 
#### route delete 192.1.1.1

#### shutdown /r /fw /f /t 0 
- restarts to system bios 



