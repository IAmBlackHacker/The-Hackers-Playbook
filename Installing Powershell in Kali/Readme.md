# Installing Powershell in Kali

```
apt-get install libunwind8
wget http://security-cdn.debian.org/debian-security/pool/updates/main/o/openssl/libssl1.0.0_1.0.1t-1+deb8u12_amd64.deb
dpkg -i libssl1.0.0_1.0.1t-1+deb8u12_amd64.deb
wget http://security.ubuntu.com/ubuntu/pool/main/i/icu/libicu55_55.1-7ubuntu0.4_amd64.deb
dpkg -i libicu55_55.1-7ubuntu0.4_amd64.deb
wget https://github.com/PowerShell/PowerShell/releases/download/v6.0.0-beta.5/powershell_6.0.0-beta.5-1ubuntu1.16.04.1_amd64.deb
dpkg -i ./powershell_6.0.0-beta.5-1ubuntu1.16.04.1_amd64.deb
powershell
```
