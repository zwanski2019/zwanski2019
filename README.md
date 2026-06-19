<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=0,2,2,5,30&height=140&section=header&text=&animation=fadeIn" width="100%"/>

<img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=900&size=48&duration=2800&pause=1200&color=00FF41&center=true&vCenter=true&multiline=false&width=900&height=90&lines=ZWANSKI" />

<img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=300&size=16&duration=3500&pause=1500&color=00CC33&center=true&vCenter=true&width=800&height=28&lines=OFFENSIVE+SECURITY+%2F%2F+WEB+EXPLOITATION+%2F%2F+RECON+AUTOMATION;BUG+BOUNTY+HUNTER+%2F%2F+SECURITY+RESEARCHER+%2F%2F+TOOL+DEVELOPER" />

<br/>

<img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&size=13&duration=3000&pause=800&color=00AA22&center=true&vCenter=true&width=750&height=24&lines=%5B+SYSTEM+ONLINE+%E2%96%B8+RECON+ENGINE+INITIALIZED+%5D;%5B+PASSIVE+INTELLIGENCE+%E2%96%B8+GATHERING+...+%5D;%5B+SUBDOMAIN+ENUMERATION+%E2%96%B8+EXPANDING+...+%5D;%5B+VULNERABILITY+SCAN+%E2%96%B8+PROCESSING+...+%5D;%5B+EXPLOIT+CHAIN+%E2%96%B8+VALIDATING+...+%5D;%5B+CRITICAL+FINDING+%E2%96%B8+DOCUMENTING+...+%5D;%5B+REPORT+SUBMITTED+%E2%96%B8+AWAITING+TRIAGE+%5D" />

<br/><br/>

[![HackerOne](https://img.shields.io/badge/HackerOne-000000?style=for-the-badge&logo=hackerone&logoColor=white)](https://hackerone.com/zwanski)
[![Bugcrowd](https://img.shields.io/badge/Bugcrowd-F26822?style=for-the-badge&logo=bugcrowd&logoColor=white)](https://bugcrowd.com/zwanski)
[![HackTheBox](https://img.shields.io/badge/HackTheBox-9FEF00?style=for-the-badge&logo=hackthebox&logoColor=black)](https://hackthebox.com/zwanski)
[![GitHub](https://img.shields.io/badge/@zwanski2019-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/zwanski2019)

<br/>


</div>

---


```bash
┌─[✗]─[zwanski@kali-linux]─[~/recon/target-corp]
└──╼ $ whoami && id
zwanski
uid=1000(zwanski) gid=1000(zwanski) groups=1000(zwanski),27(sudo)

┌─[✗]─[zwanski@kali-linux]─[~/recon/target-corp]
└──╼ $ cat banner.txt

 ███████╗██╗    ██╗ █████╗ ███╗   ██╗███████╗██╗  ██╗██╗
 ╚══███╔╝██║    ██║██╔══██╗████╗  ██║██╔════╝██║ ██╔╝██║
   ███╔╝ ██║ █╗ ██║███████║██╔██╗ ██║███████╗█████╔╝ ██║
  ███╔╝  ██║███╗██║██╔══██║██║╚██╗██║╚════██║██╔═██╗ ██║
 ███████╗╚███╔███╔╝██║  ██║██║ ╚████║███████║██║  ██╗██║
 ╚══════╝ ╚══╝╚══╝ ╚═╝  ╚═╝╚═╝  ╚═══╝╚══════╝╚═╝  ╚═╝╚═╝
 
        [ RECONNAISSANCE AUTOMATION FRAMEWORK v3.7 ]
        [ STATUS: OPERATIONAL | MODE: AGGRESSIVE  ]
        [ NETWORK: TOR ENABLED | VPN: ACTIVE       ]

┌─[✗]─[zwanski@kali-linux]─[~/recon/target-corp]
└──╼ $ ./recon-master.sh example-corp.com

[22:47:13] [INFO] Target acquired: example-corp.com
[22:47:13] [INFO] Initializing reconnaissance modules...
[22:47:14] [✓] Module loaded: passive_intel
[22:47:14] [✓] Module loaded: subdomain_enum
[22:47:14] [✓] Module loaded: port_scanner
[22:47:14] [✓] Module loaded: vuln_scanner
[22:47:15] [WARN] Engaging aggressive mode - may trigger IDS/IPS

[22:47:15] [>] PHASE 1: PASSIVE INTELLIGENCE GATHERING
[22:47:15] [*] Querying WHOIS database...
[22:47:16] [+] Organization: Example Corp Ltd.
[22:47:16] [+] Registrar: GoDaddy.com, LLC
[22:47:16] [+] Creation Date: 2015-03-21
[22:47:16] [+] Email: admin@example-corp.com

[22:47:17] [*] Searching Certificate Transparency logs...
[22:47:18] [+] CT Log: crt.sh - 247 certificates found
[22:47:19] [+] Extracted 458 unique subdomains

[22:47:20] [*] Mining historical DNS records...
[22:47:22] [+] SecurityTrails: 89 additional subdomains
[22:47:22] [+] Total unique assets: 547 subdomains

[22:47:23] [*] Searching GitHub for exposed secrets...
[22:47:25] [!] WARNING: Found potential API key in repo: example-corp/mobile-app
[22:47:25]     └─ File: /config/production.js
[22:47:25]     └─ Pattern: AWS_SECRET_ACCESS_KEY="wJalrXUtn..."

[22:47:27] [>] PHASE 2: ACTIVE SUBDOMAIN ENUMERATION
[22:47:27] [*] Launching multi-source enumeration...
[22:47:28] [*] Subfinder ━━━━━━━━━━━━━━━━━━━━ 189/189 [100%]
[22:47:31] [*] Amass    ━━━━━━━━━━━━━━━━━━━━ 312/312 [100%]
[22:47:33] [*] Assetfinder ━━━━━━━━━━━━━━━━ 156/156 [100%]

[22:47:35] [>] PHASE 3: HOST DISCOVERY & PROBING
[22:47:35] [*] Probing 547 subdomains for live hosts...
[22:47:36] [*] HTTPX ━━━━━━━━━━━━━━━━━━━━━━━━━━━ 547/547 [100%]
[22:47:42] [+] Live hosts discovered: 127
[22:47:42] [+] HTTP services: 89
[22:47:42] [+] HTTPS services: 38

[22:47:43] [>] PHASE 4: PORT SCANNING
[22:47:43] [*] Scanning 127 live hosts...
[22:47:44] [*] NMAP ━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 127/127 [100%]
[22:48:12] [!] Open port found: api.example-corp.com:8080
[22:48:12]     └─ Service: Apache Tomcat/9.0.31
[22:48:13] [!] Open port found: admin.example-corp.com:3306
[22:48:13]     └─ Service: MySQL 5.7.28
[22:48:14] [!] Open port found: dev.example-corp.com:22
[22:48:14]     └─ Service: OpenSSH 7.4

[22:48:18] [>] PHASE 5: TECHNOLOGY FINGERPRINTING
[22:48:18] [*] Analyzing web technologies...
[22:48:22] [+] Main site: React 17.0.2, nginx/1.18.0
[22:48:23] [+] API: Express.js, MongoDB
[22:48:24] [+] Admin panel: PHP 7.4, MySQL

[22:48:25] [✓] RECONNAISSANCE COMPLETE
[22:48:25] [+] Total subdomains: 547
[22:48:25] [+] Live hosts: 127
[22:48:25] [+] Open ports: 342
[22:48:25] [+] Vulnerabilities detected: 23
[22:48:25] [!] High-value targets identified: 7
[22:48:25] [*] Results saved: ./output/example-corp_recon_20240216.json

┌─[✗]─[zwanski@kali-linux]─[~/recon/target-corp]
└──╼ $ cat high_value_targets.txt

╔═══════════════════════════════════════════════════════════╗
║              HIGH-VALUE TARGETS IDENTIFIED                 ║
╠═══════════════════════════════════════════════════════════╣
║ [1] api.example-corp.com:8080                             ║
║     └─ Exposed API with weak authentication               ║
║                                                            ║
║ [2] admin.example-corp.com                                ║
║     └─ Admin panel accessible without VPN                 ║
║                                                            ║
║ [3] dev.example-corp.com                                  ║
║     └─ Development server with directory listing          ║
║                                                            ║
║ [4] backup.example-corp.com                               ║
║     └─ Backup files publicly accessible                   ║
║                                                            ║
║ [5] staging-api.example-corp.com                          ║
║     └─ Same credentials as production                     ║
║                                                            ║
║ [6] internal-docs.example-corp.com                        ║
║     └─ Confluence with guest access enabled               ║
║                                                            ║
║ [7] s3.amazonaws.com/example-corp-uploads                 ║
║     └─ Public S3 bucket with PII                          ║
╚═══════════════════════════════════════════════════════════╝

┌─[✗]─[zwanski@kali-linux]─[~/recon/target-corp]
└──╼ $ echo "Moving to exploitation phase..."
Moving to exploitation phase...
```

---


---

## `// 10 — PROFESSIONAL NETWORKS`

<div align="center">

```
╔════════════════════════════════════════════════════════════╗
║                      CONNECT WITH ME                       ║
╠════════════════════════════════════════════════════════════╣
║                                                            ║
║  📱  Telegram     →  @zwanski                              ║
║  🔐  Signal       →  xzwnsk2019.01                         ║
║  🌐  Portfolio    →  zwanski-store.pages.dev               ║
║  💻  GitHub       →  github.com/zwanski2019                ║
║  🐦  Twitter/X    →  @zwanski_m                            ║
║  📧  Email        →  [LOoodingggg :)]                      ║
║                                                            ║
║  🤝  Collaboration: Open to team-ups & knowledge sharing   ║
║  💼  Consultancy: Available for security assessments       ║
║                                                            ║
╚════════════════════════════════════════════════════════════╝
```

[![Telegram](https://img.shields.io/badge/Telegram-2CA5E0?style=for-the-badge&logo=telegram&logoColor=white)](https://t.me/zwanski)
[![Signal](https://img.shields.io/badge/Signal-3A76F0?style=for-the-badge&logo=signal&logoColor=white)](#)
[![Website](https://img.shields.io/badge/Website-00FF41?style=for-the-badge&logo=google-chrome&logoColor=black)](https://zwanski-store.pages.dev)

</div>

---

## `// 11 — CODE OF CONDUCT`

<details>
<summary><b>⚖️ Click to view ethical hacking principles</b></summary>

<br>

<div align="center">

```
┌──────────────────────────────────────────────────────────────────┐
│  ETHICAL HACKING PRINCIPLES                                      │
├──────────────────────────────────────────────────────────────────┤
│  ✓  Always operate within legal boundaries                      │
│  ✓  Only test authorized targets with explicit permission       │
│  ✓  Report vulnerabilities responsibly through proper channels  │
│  ✓  Respect privacy and data protection laws                    │
│  ✓  Never cause harm to systems or data                         │
│  ✓  Maintain confidentiality of discovered vulnerabilities      │
│  ✓  Collaborate and share knowledge with the community          │
│  ✓  Continuous learning and skill improvement                   │
└──────────────────────────────────────────────────────────────────┘
```

</div>

</details>

---

<div align="center">

<br/>

<img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&size=13&duration=6000&pause=1200&color=00FF41&center=true&vCenter=true&width=850&height=30&lines=authorized+access+only.+always.;report+first.+patch+fast.+secure+tomorrow.;the+best+vulnerabilities+are+the+ones+nobody+expected.;ethical+hacking+%7C+responsible+disclosure+%7C+continuous+improvement;if+it%27s+online%2C+it%27s+testable+%E2%80%94+with+permission.;security+is+not+a+product%2C+but+a+process." />

<br/>

```
╔═══════════════════════════════════════════════════════════════╗
║  "The quieter you become, the more you can hear."            ║
║                                        — Ram Dass             ║
╚═══════════════════════════════════════════════════════════════╝
```

<br/>

![Profile Views](https://komarev.com/ghpvc/?username=zwanski2019&color=00FF41&style=flat-square&label=PROFILE+VIEWS)
[![GitHub Followers](https://img.shields.io/github/followers/zwanski2019?style=flat-square&color=00FF41&labelColor=0a0a0a&logo=github)](https://github.com/zwanski2019)
[![Last Commit](https://img.shields.io/github/last-commit/zwanski2019/zwanski2019?style=flat-square&color=00FF41&labelColor=0a0a0a)](https://github.com/zwanski2019)

<br/>

<img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=0,2,2,5,30&height=100&section=footer" width="100%"/>

</div>
