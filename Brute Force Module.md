# SIP-DVWA - Brute Force Module

## Brute Force DVWA

Brute forcing web applications involves repeatedly attempting to guess login credentials or access sensitive areas by systematically trying different combinations of usernames and passwords. It can exploit weak or common passwords and is often mitigated by rate-limiting, CAPTCHAs, or account lockouts after multiple failed attempts. Effective defenses against brute force attacks include strong password policies, multi-factor authentication, and monitoring for suspicious login patterns.

## Tools Used In Lesson
- Kali Linux
- Burp Suite
- Hydra
- wfuzz
- Foxy Proxy Standard
- Seclists
- DVWA (Damn Vulnerable Web App)

## Links

- Applications
  - Burp Suite - https://portswigger.net/burp/communitydownload
  - Foxy Proxy - https://getfoxyproxy.org/downloads/
  - Hydra - https://www.kali.org/tools/hydra/
  - wFuzz - https://www.kali.org/tools/wfuzz/
- Web App
  - DVWA Repository - https://github.com/digininja/DVWA
- Wordlist
  - Seclists- https://www.kali.org/tools/seclists/

## Foxy Proxy Install

1. Open Firefox download and install the Foxy Proxy Standard Browser Exstension https://getfoxyproxy.org/downloads/
2. Configure proxy for burpsuite
   1. Click on exstension and select options
      - ![2024-09-11_14-45](https://github.com/user-attachments/assets/3ae3511e-5d6c-461a-a751-99242181359d)
   3. click on proxies tab
      - ![2024-09-11_14-46](https://github.com/user-attachments/assets/b8aca22f-c2e2-4a4a-b07a-97b832318c4a)
   4. configure proxy to match aove screeshot
  
## Brute Force Methods

### Low

## Hydra

- Get PHPSESSID by inspecting the brute force login page. ID is found under network tab
- login with known credentials and follow the URL for the user picture to find the directory of users profile image. Use the names to make a user list .txt file
- Use this command and replace the PHPSESSID with your ID

...
hydra -L '/home/kali/Documents/users.txt'  -P '/usr/share/seclists/Passwords/darkweb2017-top100.txt'  'http-get-form://127.0.0.1/DVWA/vulnerabilities/brute/:username=^USER^&password=^PASS^&Login=Login:H=Cookie\:PHPSESSID=vu38odo9072l1dpa1b7l64nn0m; security=low:F=Username and/or password incorrect'
```
function test() {
  console.log("hydra -L '/home/kali/Documents/users.txt'  -P '/usr/share/seclists/Passwords/darkweb2017-top100.txt'  'http-get-form://127.0.0.1/DVWA/vulnerabilities/brute/:username=^USER^&password=^PASS^&Login=Login:H=Cookie\:PHPSESSID=vu38odo9072l1dpa1b7l64nn0m; security=low:F=Username and/or password incorrect'");
}
```

-L provides list of users
-P provides list of passwords
- http-get-form uses the http get method to insert the user and password from your lists

### Medium

## Coming Soon

### High

## Coming Soon

### Impossible

## Coming Soon

## Links to learn more

- https://owasp.org/www-community/attacks/Brute_force_attack
- https://www.symantec.com/connect/articles/password-crackers-ensuring-security-your-password
- https://www.golinuxcloud.com/brute-force-attack-web-forms

