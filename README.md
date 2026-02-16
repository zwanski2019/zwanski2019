<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=0,2,2,5,30&height=140&section=header&text=&animation=fadeIn" width="100%"/>

<img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=900&size=48&duration=2800&pause=1200&color=00FF41&center=true&vCenter=true&multiline=false&width=900&height=90&lines=ZWANSKI" />

<img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=300&size=16&duration=3500&pause=1500&color=00CC33&center=true&vCenter=true&width=700&height=28&lines=WEB+SECURITY+%2F%2F+BUG+BOUNTY+%2F%2F+RECON+AUTOMATION" />

<br/>

<img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&size=13&duration=3000&pause=800&color=00AA22&center=true&vCenter=true&width=650&height=24&lines=%5B+INITIALIZING+RECON+FRAMEWORK+...+%5D;%5B+PASSIVE+RECON+%3A+COMPLETE+............+%5D;%5B+SUBDOMAIN+EXPANSION+%3A+DONE+..........+%5D;%5B+ENDPOINT+DISCOVERY+%3A+RUNNING+.......+%5D;%5B+EXPLOIT+WINDOW+IDENTIFIED+..........+%5D;%5B+REPORT+SUBMITTED+TO+TRIAGE+..........+%5D" />

<br/><br/>

[![HackerOne](https://img.shields.io/badge/HackerOne-000000?style=for-the-badge&logo=hackerone&logoColor=white)](https://hackerone.com/zwanski)
[![Bugcrowd](https://img.shields.io/badge/Bugcrowd-F26822?style=for-the-badge&logo=bugcrowd&logoColor=white)](https://bugcrowd.com/zwanski)
[![HackTheBox](https://img.shields.io/badge/HackTheBox-9FEF00?style=for-the-badge&logo=hackthebox&logoColor=black)](https://hackthebox.com/zwanski)
[![GitHub](https://img.shields.io/badge/@zwanski2019-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/zwanski2019)

<br/>

<pre>
┌──────────────────────────────────────────────────┐
│  HANDLE  ▸  ZWANSKI        MODE    ▸  LIVE HUNT  │
│  ORIGIN  ▸  TN / REMOTE    RANK    ▸  ASCENDING  │
│  TARGET  ▸  WEB·API·CLOUD  STATUS  ▸  ██████ ON  │
│  SCOPE   ▸  H1 · BC        REPORTS ▸  GROWING    │
└──────────────────────────────────────────────────┘
</pre>

</div>

---

## `// 01 — STACK`

<div align="center">

![Burp Suite](https://img.shields.io/badge/Burp_Suite-FF6633?style=flat-square&logo=burpsuite&logoColor=white)
![Nuclei](https://img.shields.io/badge/Nuclei-00D1B2?style=flat-square&logo=go&logoColor=white)
![Amass](https://img.shields.io/badge/Amass-0078D4?style=flat-square&logoColor=white)
![Katana](https://img.shields.io/badge/Katana-7B2FBE?style=flat-square&logoColor=white)
![Subfinder](https://img.shields.io/badge/Subfinder-00ADD8?style=flat-square&logoColor=white)
![Ffuf](https://img.shields.io/badge/Ffuf-CC0000?style=flat-square&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![Bash](https://img.shields.io/badge/Bash-4EAA25?style=flat-square&logo=gnu-bash&logoColor=white)
![Shodan](https://img.shields.io/badge/Shodan-AA0000?style=flat-square&logoColor=white)
![Caido](https://img.shields.io/badge/Caido-6C3483?style=flat-square&logoColor=white)

</div>

---

## `// 02 — EXPERTISE`
```yaml
# ══════════════════════════════════════════════════════
#  ZWANSKI — ATTACK SURFACE MAP
# ══════════════════════════════════════════════════════

recon:
  passive:    [ OSINT · shodan · censys · fofa · spyse ]
  active:     [ subdomain brute · port scan · tech fingerprint ]
  automated:  [ zwan-recon pipeline — custom built ]

web:
  injections: [ XSS · SQLi · SSTI · XXE · CRLF ]
  server:     [ SSRF · path traversal · open redirect ]
  logic:      [ IDOR · race conditions · priv escalation ]

auth:
  sessions:   [ JWT abuse · cookie manipulation · fixation ]
  oauth:      [ misconfigured flows · token leakage ]
  mfa:        [ bypass · brute · fallback abuse ]

api:
  recon:      [ endpoint enum · JS analysis · spec leak ]
  attacks:    [ BOLA · mass assignment · injection ]
  mobile:     [ APK reverse · traffic intercept ]

custom_tools:
  - zwan-recon    # full recon pipeline
  - dir-hydra     # smart directory bruteforcer
  - auth-breaker  # auth flow stress tester
```

---

## `// 03 — METHODOLOGY`
```
 PHASE 01 — PASSIVE RECON          PHASE 02 — ACTIVE RECON
 ─────────────────────────         ───────────────────────
  OSINT ──┐                         HTTPX (alive check)
  Shodan ─┼──▶ SUBFINDER                  │
  Censys ─┘    AMASS               PORT SCAN
               FOFA                       │
               │                    TECH FINGERPRINT
               ▼                          │
          SUBDOMAIN LIST ────────────────▶┤
                                          │
 PHASE 03 — CRAWL & FUZZ          PHASE 04 — EXPLOIT
 ────────────────────────          ──────────────────
  KATANA (js/link crawl)            MANUAL DEEP DIVE
       │                                 │
  FFUF (param/path fuzz)           CHAINING BUGS
       │                                 │
  NUCLEI (auto templates)          WRITING POC
       │                                 │
       └──────────────────────────────▶ REPORT
```

---

## `// 04 — STATS`

<div align="center">

<img height="160" src="https://github-readme-stats.vercel.app/api?username=zwanski2019&show_icons=true&count_private=true&bg_color=0a0a0a&border_color=00FF41&title_color=00FF41&text_color=aaaaaa&icon_color=00cc33&hide_border=false&rank_icon=github" />
<img height="160" src="https://github-readme-stats.vercel.app/api/top-langs/?username=zwanski2019&layout=compact&bg_color=0a0a0a&border_color=00FF41&title_color=00FF41&text_color=aaaaaa&hide_border=false&langs_count=6" />

<br/>

<img width="70%" src="https://github-readme-streak-stats.herokuapp.com?user=zwanski2019&theme=matrix&background=0A0A0A&border=00FF41&ring=00FF41&fire=FF6600&currStreakLabel=00FF41&sideLabels=00AA22&dates=666666" />

<br/>

<img src="https://github-profile-trophy.vercel.app/?username=zwanski2019&theme=matrix&no-frame=true&no-bg=true&column=6&margin-w=8" />

</div>

---

## `// 05 — ACTIVITY`

<div align="center">

<img src="https://github-readme-activity-graph.vercel.app/graph?username=zwanski2019&bg_color=0a0a0a&color=00FF41&line=00cc33&point=00FF41&area=true&area_color=001a00&hide_border=true" width="95%" />

</div>

---

## `// 06 — CONTACT`

<div align="center">

<pre>
┌────────────────────────────────────────────┐
│  telegram  →  @zwanski                     │
│  signal    →  xzwnsk2019.01                │
│  web       →  zwanski-store.pages.dev      │
│  github    →  github.com/zwanski2019       │
└────────────────────────────────────────────┘
</pre>

</div>

---

<div align="center">

<br/>

<img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&size=13&duration=6000&pause=1000&color=00FF41&center=true&vCenter=true&width=700&height=30&lines=authorized+access+only.+always.;report+first.+patch+fast.;the+best+bugs+are+the+ones+no+one+expected.;if+it%27s+online%2C+it%27s+in+scope+%28with+permission%29." />

<br/><br/>

<img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=0,2,2,5,30&height=100&section=footer" width="100%"/>

</div>
