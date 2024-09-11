# SIP-DVWA
## DVWA(Damn Vulnerable Web App) - Home Lab Setup
The Damn Vulnerable Web Application (DVWA) is a PHP/MySQL-based platform designed to help security professionals hone their skills in a safe, legal environment. It also serves as a learning tool for web developers, students, and educators to better understand web application security.

DVWA allows users to explore common web vulnerabilities at varying difficulty levels through an intuitive interface. While the platform has both documented and undocumented flaws, this is by design, encouraging users to uncover and exploit as many issues as possible to enhance their learning experience.

## Tools Used In Lesson
- Kali Linux
- Burp Suite
- Foxy Proxy Standard

## Links

- Web App
  - DVWA Repository - https://github.com/digininja/DVWA
- Operating System
  - Kali Linux - https://www.kali.org/get-kali/#kali-platforms
- Applications
  - Burp Suite - https://portswigger.net/burp/communitydownload
  - Foxy Proxy - https://getfoxyproxy.org/downloads/
- Hypervisor Platform
  - Virtual Box - https://www.virtualbox.org/
  - Vm Ware - https://www.vmware.com/

## DVWA Install

sudo bash -c "$(curl --fail --show-error --silent --location https://raw.githubusercontent.com/IamCarron/DVWA-Script/main/Install-DVWA.sh)"

## Foxy Proxy Install

1. Open Firefox download and install the Foxy Proxy Standard Browser Exstension https://getfoxyproxy.org/downloads/
2. Configure proxy for burpsuite
   1. Click on exstension and select options
      - ![2024-09-11_14-45](https://github.com/user-attachments/assets/3ae3511e-5d6c-461a-a751-99242181359d)
   3. click on proxies tab
      - ![2024-09-11_14-46](https://github.com/user-attachments/assets/b8aca22f-c2e2-4a4a-b07a-97b832318c4a)
   4. configure proxy to match aove screeshot

## Brute Force DVWA

Brute forcing web applications involves repeatedly attempting to guess login credentials or access sensitive areas by systematically trying different combinations of usernames and passwords. It can exploit weak or common passwords and is often mitigated by rate-limiting, CAPTCHAs, or account lockouts after multiple failed attempts. Effective defenses against brute force attacks include strong password policies, multi-factor authentication, and monitoring for suspicious login patterns.
