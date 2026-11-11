# Networkwalks-Week-2-Intern-Reconnaissance-and-Scanning
# PENETRATION TESTING REPORT
### Footprinting & Network Scanning Phases

A brief report on authorized web reconnaissance of `networkwalks.com` and host discovery on my local network, completed during my Networkwalks internship.

> All activity was limited to systems I own or had permission to assess. No exploitation or vulnerability validation was performed.

## Activities and findings

### Website footprinting

Using WHOIS, WhatWeb, `nslookup`, `curl -I`, Wafw00f and DNSRecon, I reviewed registration, web technology, DNS, HTTP header and WAF information. The results included:

- WordPress 7.0.4 and WP Download Manager 3.3.58 identified by WhatWeb.
- `networkwalks.com` resolved to `192.232.216.135` during the exercise.
- HTTP headers exposed the `/wp-json/` endpoint.
- Wafw00f identified ModSecurity (SpiderLabs).
- DNSRecon returned name server, mail, TXT/SPF and service record information.

These are observations from the exercise, not confirmed vulnerabilities. Software versions and DNS or HTTP details alone do not establish that a system is vulnerable.

### Local network discovery

I used Windows `ipconfig` to identify my local subnet, then ran a Zenmap Ping Scan and reviewed its Topology view. Two live hosts were observed:

- `10.**.***.35`
- `10.**.***.194`

The addresses are partially masked. The topology was saved as a PDF for the practical exercise.

## Risk and recommendations

Public technology and DNS details can help inform further reconnaissance; unexpected live hosts may warrant review. These findings indicate exposure or visibility, not confirmed weaknesses.

- Keep CMS platforms and plugins current.
- Review exposed HTTP details and DNS records periodically.
- Maintain and monitor WAF configuration.
- Scan internal networks periodically; verify unexpected devices and update network documentation.
- Test only within an authorized scope.

## Tools

Kali Linux: WHOIS, WhatWeb, `nslookup`, `curl`, Wafw00f and DNSRecon. Windows: `ipconfig` and Zenmap (Nmap GUI).


# 8. Evidences Collected
<img width="637" height="552" alt="whois networkwalks com1_2" src="https://github.com/user-attachments/assets/d6b51de2-3912-438b-aa06-4cc990ff099f" />
<img width="647" height="907" alt="whois networkwanks com 2_2" src="https://github.com/user-attachments/assets/28e35b59-3018-4ce7-8abb-04f39369be45" />
<img width="642" height="476" alt="whatweb networkwalks com_screenshot" src="https://github.com/user-attachments/assets/b09d800d-663e-4471-b1c4-adf9db0d05d0" />
<img width="640" height="276" alt="nslookup networkwalks com_screenshot" src="https://github.com/user-attachments/assets/50a31468-8f71-4881-92c2-781d11d58b54" />
<img width="644" height="454" alt="curl -I" src="https://github.com/user-attachments/assets/f3a5adf1-a7f1-4afc-9372-7c703a7a69f4" />
<img width="645" height="500" alt="wafw00f networkwalks com_screenshot" src="https://github.com/user-attachments/assets/6115ae8c-0999-4c5b-9862-78615f965832" />
<img width="648" height="854" alt="dnsrecon -d networkwalks com_screenshot" src="https://github.com/user-attachments/assets/36a980ef-e621-4f63-9570-dbe9a81f2576" />
<img width="644" height="657" alt="theHarvester -d microsoft com -l 1000 -b baidu_screenshot" src="https://github.com/user-attachments/assets/f1e7005c-87bd-4b70-8020-451bf5f0a815" />

(https://github.com/user-attachments/files/34691209/zenmap_local.hosts.scan_topology.pdf)




# 9.Aditional task: FOOTPRINTING & RECONNAISSANCE ATTACKS WITH GHDB

GHDB Exploit-DB_live cam

<img width="796" height="522" alt="1" src="https://github.com/user-attachments/assets/d0423fb3-eb36-4ef7-bdb6-89c1d5c36cb1" />

GHDB Exploit-DB_math_pdf

<img width="700" height="793" alt="2" src="https://github.com/user-attachments/assets/4e70b22b-d7a2-494b-a0e8-58dacd0a933a" />


















