# SIP-DVWA - Intro & Install

## DVWA(Damn Vulnerable Web App) - Home Lab Setup
The Damn Vulnerable Web Application (DVWA) is a PHP/MySQL-based platform designed to help security professionals hone their skills in a safe, legal environment. It also serves as a learning tool for web developers, students, and educators to better understand web application security.

DVWA allows users to explore common web vulnerabilities at varying difficulty levels through an intuitive interface. While the platform has both documented and undocumented flaws, this is by design, encouraging users to uncover and exploit as many issues as possible to enhance their learning experience.

## Tools Used In Lesson
- Kali Linux
- DVWA (Damn Vulnerable Web App)

## Links

- Web App
  - DVWA Repository - https://github.com/digininja/DVWA
- Operating System
  - Kali Linux - https://www.kali.org/get-kali/#kali-platforms
- Hypervisor Platform
  - Virtual Box - https://www.virtualbox.org/
  - Vm Ware - https://www.vmware.com/

## DVWA Install

    sudo bash -c "$(curl --fail --show-error --silent --location https://raw.githubusercontent.com/IamCarron/DVWA-Script/main/Install-DVWA.sh)"

- Paste into terminal and hit enter and this script will install DVWA
- Navigate to http://localhost/DVWA/login.php
- Login - User=admin Password=password

