![image](https://travis-ci.com/BrashEndeavours/hotwax.svg?branch=master)

# HOTWAX

Hotwax is a script to provision a set of extra pentesting tools onto a Kali Linux machine in a consistent manner.

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for deployment AND development purposes.

### Prerequisites

* Kali Linux 2019.4 or older.  (Presently, will not work on Kali LInux 2020.1 or newer, due to change from default root account configuration to non-root user account configuration. To be fixed in near future.)

* Git
* Ansible

```
apt update -y
apt install -y git ansible
```

### Installing

Clone the HOTWAX repository.

```
cd ~
git clone https://github.com/BrashEndeavours/hotwax
```

Run the playbook

```
cd hotwax
ansible-playbook playbook.yml
```

## Tools updated:
 - [Samba 4.10.8 (smbclient,rpcclient,nmblookup](https://github.com/samba-team/samba) - Patched to fix issues with polenum, enum4linux, and restoring smbclient connection output.
 - [enum4linux](https://github.com/portcullislabs/enum4linux) - Fix minor parsing issues. Updates temporarily included by BrashEndeavours fork, until PR is merged.

## Tools installed:
 - [Arjun](https://github.com/s0md3v/Arjun) - Arjun is an HTTP parameter discovery suite.
 - [AutoRecon](https://github.com/Tib3rius/AutoRecon) - AutoRecon is a multi-threaded network reconnaissance tool which performs automated enumeration of services.
 - [BloodHound](https://github.com/BloodHoundAD/BloodHound) - Six Degrees of Domain Admin.
 - [chisel](https://github.com/jpillora/chisel) - A fast TCP tunnel over HTTP
 - [evil-winrm](https://github.com/Hackplayers/evil-winrm) - The ultimate WinRM shell for hacking/pentesting.
 - [gobuster](https://github.com/OJ/gobuster) - Directory/File, DNS and VHost busting tool written in Go
 - [LinEnum](https://github.com/rebootuser/LinEnum) - Local Linux Enumeration & Privilege Escalation Script 
 - [nishang](https://github.com/samratashok/nishang) - Framework and collection of scripts and payloads which enables usage of PowerShell for penetration testing.
 - [One-Lin3r](https://github.com/D4Vinci/One-Lin3r) - On demand one-liners that aid in penetration testing operations, privilege escalation and more
 - [OSCP Exam Report Template](https://github.com/whoisflynn/OSCP-Exam-Report-Template) - Modified template for the OSCP Exam
 - [Powerless](https://github.com/M4ximuss/Powerless) - A Windows privilege escalation (enumeration) script designed with OSCP labs (i.e. legacy Windows machines without Powershell) in mind.
 - [PowerSploit](https://github.com/PowerShellMafia/PowerSploit) - Collection of Microsoft PowerShell modules that can be used to aid penetration testers during all phases of an assessment.
 - [proxychains-ng](https://github.com/rofl0r/proxychains-ng) - proxychains ng (new generation) - a preloader which hooks calls to sockets in dynamically linked programs and redirects it through one or more socks/http proxies. continuation of the unmaintained proxychains project.
 - [pspy](https://github.com/DominicBreuker/pspy) - Monitor linux processes without root permissions.
 - [SecLists](https://github.com/danielmiessler/SecLists) - Collection of usernames, passwords, URLs, sensitive data patterns, fuzzing payloads, web shells, and more.
 - [sherlock](https://github.com/sherlock-project/sherlock) - Find usernames across social networks.
 - [sshuttle](https://github.com/sshuttle/sshuttle) - Transparent proxy server that works as a poor man's VPN. Forwards over ssh. Doesn't require admin. Works with Linux and MacOS. Supports DNS tunneling.
 - [webshell](https://github.com/tennc/webshell) - This is a webshell open source project.
 - [Windows PHP Reverse Shell](https://github.com/Dhayalanb/windows-php-reverse-shell) - Simple php reverse shell implemented using bina- https://github.com/ucki/zauberfeder, based on an webshell.
 - [XSStrike](https://github.com/s0md3v/XSStrike) - Advanced XSS scanner
 - [zauberfeder](https://github.com/ucki/zauberfeder) - A LaTex reporting template.
 - [crackmapexec](https://github.com/byt3bl33d3r/CrackMapExec) - A swiss army knife for pentesting networks.
 - [windows-kernel-exploits](https://github.com/SecWiki/windows-kernel-exploits) - Precompiled Windows Exploits.
 - [exiftool](https://github.com/exiftool/exiftool) - ExifTool meta information reader/writer.  Great for viewing and manipulating exif-data.
 - [html2text](https://github.com/Alir3z4/html2text/) - Convert HTML to clean, easy-to-read plain ASCII text.
 - [mingw-w64](http://mingw-w64.org/doku.php) - GCC for Windows 64 & 32 bits.
 - [msfpc](https://github.com/g0tmi1k/msfpc) - MSFvenom Payload Creator (MSFPC)
 - [wce](https://www.ampliasecurity.com/research/windows-credentials-editor/) - A security tool to list logon sessions and add, change, list and delete associated credentials.
 - [Windows-Exploit-Suggester](https://github.com/AonCyberLabs/Windows-Exploit-Suggester) - This tool compares a targets patch levels against the Microsoft vulnerability database in order to detect potential missing patches on the target.
 - [pyftpdlib](https://github.com/giampaolo/pyftpdlib) - Extremely fast and scalable Python FTP server library.  Spin up FTP Server with a one-liner.
 - [ssh-os](https://github.com/richlamdev/ssh-default-banners) - Nmap Script that identifies Debian, Ubuntu, FreeBSD version based on default SSH banner response.
 - [empire](https://github.com/EmpireProject/Empire) - Empire is a post-exploitation framework that includes a pure-PowerShell2.0 Windows agent, and a pure Python 2.6/2.7 Linux/OS X agent.
 - [medusa](http://foofus.net/goons/jmk/medusa/medusa.html) - Medusa is a speedy, parallel, modular login brute-forcer.  Similar to ncrack and Hydra.

## Contributing

Please read [CONTRIBUTING.md](https://github.com/BrashEndeavours/hotwax/blob/master/CONTRIBUTING.md) for details on the code of conduct, and the process for submitting pull requests.

## Authors

* **Blake Mackey (@BrashEndeavours)** - *Initial work* - [BrashEndeavours](https://github.com/BrashEndeavours)

## Contributors

* Want your name here? See CONTRIBUTING.md for details.

* **Alec Mather-Shapiro (whoisflynn)** - *Added AutoRecon, Windows PHP Reverse Shell, and OSCP Exam Template* - [whoisflynn](https://github.com/whoisflynn)
* **Richard Lam (richlamdev)** - *Added crackmapexec, windows-kernel-exploits, exiftool, html2text, mingw-w64, msfpc, wce, windows-exploit-suggester, pyftpdlib, ssh-os.nse, medusa* - [richhlamdev](https://github.com/richlamdev/)

## Acknowledgements

* **Rebootuser (@rebootuser)** - [LinEnum](https://github.com/rebootuser/LinEnum)
* **D4Vinci (@Seekurity)** - [One-Lin3r](https://github.com/D4Vinci/One-Lin3r)
* **PowerShellMafia** - [PowerSploit](https://github.com/PowerShellMafia/PowerSploit)
* **Daniel Miessler** - [SecLists](https://github.com/danielmiessler/SecLists)
* **Nikhil "SamratAshok" Mittal** - [nishang](https://github.com/samratashok/nishang)
* **Dominic Breuker** - [pspy](https://github.com/DominicBreuker/pspy)
* **sherlock-project** - [sherlock](https://github.com/sherlock-project/sherlock)
* **Tib3rius** - [AutoRecon](https://github.com/Tib3rius/AutoRecon)
* **Dhayalanb** - [Windows PHP Reverse Shell](https://github.com/Dhayalanb/windows-php-reverse-shell)
* **whoisflynn** - [OSCP Exam Report Template](https://github.com/whoisflynn/OSCP-Exam-Report-Template)
* **jpillora** - [chisel](https://github.com/jpillora/chisel)
* **OJ Reeves** - [gobuster](https://github.com/OJ/gobuster)
* **rofl0r** - [proxychains-ng](https://github.com/rofl0r/proxychains-ng)
* **Brian May** - [sshuttle](https://github.com/sshuttle/sshuttle)
* **tennc** - [webshell](https://github.com/tennc/webshell)
* **PortcullisLabs** - [enum4linux](https://github.com/portcullislabs/enum4linux)
* **M4ximuss** - [Powerless](https://github.com/M4ximuss/Powerless)
* **Somdev Sangwan** - [Arjun](https://github.com/s0md3v/Arjun)
* **ucki** - [zauberfeder](https://github.com/ucki)
* **BloodHoundAD** - [BloodHound](https://github.com/BloodHoundAD)
* **byt3bl33d3r** - [crackmapexec](https://github.com/byt3bl33d3r/CrackMapExec)
* **abatchy17** - [WindowsExploits](https://github.com/abatchy17/WindowsExploits)
* **exiftol** - [exiftool](https://github.com/exiftool/exiftool)
* **Alir3z4** - [html2text](https://github.com/Alir3z4/html2text/)
* **mingw-w64** - [mingw-w64](http://mingw-w64.org/doku.php)
* **g0tmi1k** - [msfpc](https://github.com/g0tmi1k/msfpc)
* **ampliasecurity.com** - [wce](https://www.ampliasecurity.com/research/windows-credentials-editor/)
* **AonCyberLabs** - [Windows-Exploit-Suggester](https://github.com/AonCyberLabs/Windows-Exploit-Suggester)
* **giampaolo** - [pyftpdlib](https://github.com/giampaolo/pyftpdlib)
* **richlamdev** - [ssh-os](https://github.com/richlamdev/ssh-default-banners)
* **harmj0y** - [empire](https://github.com/EmpireProject/Empire)
* **foofus** - [foofus.net](http://foofus.net/goons/jmk/medusa/medusa.html)

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details
