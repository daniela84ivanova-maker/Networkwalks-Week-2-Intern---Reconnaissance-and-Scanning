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

[zenmap_local hosts scan_topology.pdf](https://github.com/user-attachments/files/34691209/zenmap_local.hosts.scan_topology.pdf)




# 9.Aditional task: FOOTPRINTING & RECONNAISSANCE ATTACKS WITH GHDB

GHDB Exploit-DB_live cam
No.	Link	Relevant Dork	Username / Password
(if any)
1	http://109.233.191.130:8080/
inurl:/ViewerFrame? intitle:"Network Camera NetworkCamera"	-
2	http://109.206.96.75:8080/ 
inurl:mobile.html intitle:webcamXP	-
3	http://www.insecam.org/en/view/414256/ 
inurl:mobile.html intitle:webcamXP	-
4	http://68.115.218.130:32479/multi.html 
inurl:/multi.html intitle:webcam	-
5	http://72.199.200.5:8080/ 
intitle:"webcamxp" "Flash JPEG Stream"	-
6	http://phildorian.hopto.org:8080/ 
intitle:"webcamxp" "Flash JPEG Stream"	-
7	http://myfishcam.homedns.org:444/ 
intitle:"webcamxp" "Flash JPEG Stream"	-
8	http://193.77.49.122/ 
inurl:"view.shtml" "Network Camera"	-
9	http://www.insecam.org/en/view/1010229/ 
inurl:"live/cam.html"	-
10	http://173.69.185.179:9001/cgi-bin/guestimage.html 
inurl:"live/cam.html" 	-


GHDB Exploit-DB_math_pdf

No.	Link	Relevant Dork	Username / Password
(if any)
1	http://erewhon.superkuh.com/library/Math/ 
intitle:index.of "parent
directory" mathematics pdf	-
2	https://ochicken.net/library/Mathematics/ 
intitle:index.of "parent
directory" mathematics pdf	-
3	https://netlib.org/math/docpdf/ 
intitle:index.of "parent
directory" mathematics pdf	-
4	https://jasoncantarella.com/downloads/?C=N;O=D 
intitle:index.of "parent
directory" mathematics pdf	-
5	https://math.ucr.edu/home/baez/mathematical/ 
intitle:index.of "parent
directory" mathematics pdf	-
6	https://www.jsoftware.com/books/pdf/ 
intitle:index.of "parent
directory" mathematics pdf	-
7	http://inis.jinr.ru/sl/vol2/Mathematics/Math.Encyclopedia/Pdf/ 
intitle:index.of "parent
directory" mathematics pdf	-
8	https://www.math.ias.edu/~goresky/pdf/ 
intitle:index.of "parent
directory" mathematics pdf	-
9	https://www.maher.org.uk/~math/teaching/2023/spring/tda/notes/ 
intitle:index.of "parent
directory" mathematics pdf	-
10	https://k4m.uk/beal/files/After%20School/?MD 
intitle:index.of "parent
directory" mathematics pdf	-


















