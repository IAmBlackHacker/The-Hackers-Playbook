# PowerShell Empire
```
PowerShell Empire is a post-exploitation framework for computers and servers running Microsoft Windows, Windows Server operating systems, or both.
```

## Empire
* https://github.com/EmpireProject/Empire

## Running Empire
Strting up Empire
```
>> cd /opt/Empire && ./setup/reset.sh
```
Exit
```
>> exit
```
Setup Up Cert
```
>> ./setup/cert.sh
```
Start Empire
```
>> ./empire
```
Start a listners
```
>> listners
```
Pick your listners
```
userlistners [tab twice]
uesrlistners http
```
View all configuration for the listners
```
info
```
Execute
```
execute
```
Go tot the main menu
```
main
```
Create stager
```
usertager [tab twice]
usertager windows/launcher_bat
```
Create Payload
```
generate
```
Review your payload in another terminal window
```
cat /tmp/launcher.bat
```
