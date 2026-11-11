Week 2: Reconnaissance and Network Scanning

A report on authorized reconnaissance of `networkwalks.com` and host discovery on my local network, completed during my Networkwalks internship.

> All activities were performed within an authorized scope. No exploitation or vulnerability validation was performed.

## Website reconnaissance

I used WHOIS, WhatWeb, `nslookup`, `curl -I`, Wafw00f, DNSRecon and Maltego to review publicly available domain, DNS, web technology and certificate information.

Findings recorded during the exercise:

- WhatWeb identified WordPress 7.0.4 and WP Download Manager 3.3.58.
- `networkwalks.com` resolved to `192.232.216.135` at the time of the scan.
- The HTTP response exposed the `/wp-json/` endpoint.
- Wafw00f identified ModSecurity (SpiderLabs).
- DNSRecon returned name server, mail, TXT/SPF and service record information.
- Maltego displayed SSL certificate-related information. This does not establish that a private key was exposed.

These are observations, not confirmed vulnerabilities. Software versions, DNS records and HTTP details alone do not show that a system is vulnerable.

## Local network discovery

I used Windows `ipconfig` to identify my local subnet, then ran a Zenmap Ping Scan and reviewed its Topology view. Two live hosts were observed:

- `10.**.***.35`
- `10.**.***.194`

![Zenmap local network topology](https://github.com/user-attachments/assets/83a0dda2-09ee-4c4c-864c-bec398a3160b)

The host addresses are partially masked. The topology was saved as a PDF for the practical exercise.

## Additional GHDB exercise

As a separate exercise, I reviewed Google Hacking Database (GHDB) search examples, including searches related to live cameras and PDF files. These are search techniques, not exploits. Any testing must remain within an authorized scope and respect privacy.

## Recommendations

- Keep the CMS and plugins updated.
- Review public HTTP details and DNS records periodically.
- Maintain and monitor WAF configuration.
- Scan internal networks periodically, investigate unexpected devices and keep network documentation current.
- Perform reconnaissance and scanning only with authorization.

## Tools

**Kali Linux:** WHOIS, WhatWeb, `nslookup`, `curl`, Wafw00f, DNSRecon, Maltego and the GHDB exercise.  
**Windows:** `ipconfig` and Zenmap (Nmap GUI).

## Evidence

### WHOIS

![WHOIS results for networkwalks.com](https://github.com/user-attachments/assets/d6b51de2-3912-438b-aa06-4cc990ff099f)

![WHOIS results, second screenshot](https://github.com/user-attachments/assets/28e35b59-3018-4ce7-8abb-04f39369be45)

### Website and DNS reconnaissance

![WhatWeb results](https://github.com/user-attachments/assets/b09d800d-663e-4471-b1c4-adf9db0d05d0)

![nslookup results](https://github.com/user-attachments/assets/50a31468-8f71-4881-92c2-781d11d58b54)

![curl response headers](https://github.com/user-attachments/assets/f3a5adf1-a7f1-4afc-9372-7c703a7a69f4)

![Wafw00f results](https://github.com/user-attachments/assets/6115ae8c-0999-4c5b-9862-78615f965832)

![DNSRecon results](https://github.com/user-attachments/assets/36a980ef-e621-4f63-9570-dbe9a81f2576)

### Other exercise evidence

TheHarvester screenshot from a separate Microsoft.com exercise:

![TheHarvester results for microsoft.com](https://github.com/user-attachments/assets/f1e7005c-87bd-4b70-8020-451bf5f0a815)

![Maltego graph](https://github.com/user-attachments/assets/c520cb48-c4e0-4623-81c9-e72d06e82ce7)

GHDB search example: live cameras:

![GHDB live camera search example](https://github.com/user-attachments/assets/d0423fb3-eb36-4ef7-bdb6-89c1d5c36cb1)

GHDB search example: PDF files:

![GHDB PDF search example](https://github.com/user-attachments/assets/4e70b22b-d7a2-494b-a0e8-58dacd0a933a)


















