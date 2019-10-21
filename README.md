![image](https://travis-ci.com/BrashEndeavours/hotwax.svg?branch=master)

# HOTWAX

Hotwax is a script to provision a set of extra pentesting tools onto a Kali Linux machine in a consistent manner.

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for deployment AND development purposes.

### Prerequisites

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
 - [AutoRecon](https://github.com/Tib3rius/AutoRecon) - AutoRecon is a multi-threaded network reconnaissance tool which performs automated enumeration of services.
 - [chisel](https://github.com/jpillora/chisel) - A fast TCP tunnel over HTTP
 - [evil-winrm](https://github.com/Hackplayers/evil-winrm) - The ultimate WinRM shell for hacking/pentesting.
 - [gobuster](https://github.com/OJ/gobuster) - Directory/File, DNS and VHost busting tool written in Go
 - [LinEnum](https://github.com/rebootuser/LinEnum) - Local Linux Enumeration & Privilege Escalation Script 
 - [nishang](https://github.com/samratashok/nishang) - Framework and collection of scripts and payloads which enables usage of PowerShell for penetration testing.
 - [One-Lin3r](https://github.com/D4Vinci/One-Lin3r) - On demand one-liners that aid in penetration testing operations, privilege escalation and more
 - [Powerless](https://github.com/M4ximuss/Powerless) - A Windows privilege escalation (enumeration) script designed with OSCP labs (i.e. legacy Windows machines without Powershell) in mind.
 - [PowerSploit](https://github.com/PowerShellMafia/PowerSploit) - Collection of Microsoft PowerShell modules that can be used to aid penetration testers during all phases of an assessment.
 - [proxychains-ng](https://github.com/rofl0r/proxychains-ng) - proxychains ng (new generation) - a preloader which hooks calls to sockets in dynamically linked programs and redirects it through one or more socks/http proxies. continuation of the unmaintained proxychains project.
 - [pspy](https://github.com/DominicBreuker/pspy) - Monitor linux processes without root permissions.
 - [SecLists](https://github.com/danielmiessler/SecLists) - Collection of usernames, passwords, URLs, sensitive data patterns, fuzzing payloads, web shells, and more.
 - [sherlock](https://github.com/sherlock-project/sherlock) - Find usernames across social networks.
 - [sshuttle](https://github.com/sshuttle/sshuttle) - Transparent proxy server that works as a poor man's VPN. Forwards over ssh. Doesn't require admin. Works with Linux and MacOS. Supports DNS tunneling.
 - [webshell](https://github.com/tennc/webshell) - This is a webshell open source project.
 - [Windows PHP Reverse Shell](https://github.com/Dhayalanb/windows-php-reverse-shell) - Simple php reverse shell implemented using binary, based on an webshell.
 - [XSStrike](https://github.com/s0md3v/XSStrike) - Advanced XSS scanner
 - [OSCP Exam Report Template](https://github.com/whoisflynn/OSCP-Exam-Report-Template) - Modified template for the OSCP Exam

## Contributing

Please read [CONTRIBUTING.md](https://github.com/BrashEndeavours/hotwax/blob/master/CONTRIBUTING.md) for details on the code of conduct, and the process for submitting pull requests.

## Authors

* **Blake Mackey (@BrashEndeavours)** - *Initial work* - [BrashEndeavours](https://github.com/BrashEndeavours)

## Contributors

* Want your name here? See CONTRIBUTING.md for details.

* **Alec Mather-Shapiro (whoisflynn)** - *Added AutoRecon, Windows PHP Reverse Shell, and OSCP Exam Template** - [whoisflynn](https://github.com/whoisflynn)

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

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details

