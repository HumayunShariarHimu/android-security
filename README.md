# android-security

> A curated and organized collection of resources related to **android-security**.

**Humayun Shariar Himu**  
A Passionated Psychologist & Tech Lover!  
Based in Bangladesh  
[GitHub Profile](https://github.com/HumayunShariarHimu)

# android-security

> A curated and organized collection of resources related to **android-security**.

**Maintained by [Humayun Shariar Himu](https://github.com/HumayunShariarHimu)**

# Android Security

> Explore Android security: secure app development, reverse engineering, vulnerability testing, and best practices for data protection and encryption.

## Contents

1. [Tools](#tools)
2. [Academic / Research / Publications / Books](#academic--research--publications--books)
3. [Exploits / Vulnerabilities / Bugs](#exploits--vulnerabilities--bugs)
4. [Blogs, Write-ups & Research Feeds](#blogs-write-ups--research-feeds)
5. [Communities, Forums & Conferences](#communities-forums--conferences)

---

## Tools

### Online Analyzers

| Tool | Notes |
|---|---|
| [VirusTotal](https://www.virustotal.com/) | Multi-engine scanning, max 128MB per file |
| [Koodous](https://koodous.com) | Static/dynamic malware analysis against public & private YARA rules |
| [MobSF Cloud / Community Edition](https://mobsf.github.io/docs/) | Hosted version of the popular open-source MobSF scanner |
| [Oversecured](https://oversecured.com/) | Enterprise vulnerability scanner for Android & iOS, integrates into CI/CD (paid) |
| [AppSweep by Guardsquare](https://appsweep.guardsquare.com/) | Free, fast automated security testing for developers |
| [Appknox](https://www.appknox.com/) | Enterprise mobile app security testing platform (paid) |
| [NowSecure](https://www.nowsecure.com/) | Automated static/dynamic mobile app security testing (paid) |
| [Immuniweb Mobile](https://www.immuniweb.com/mobile/) | OWASP Mobile Top 10 test, privacy check, permissions test — free tier available |
| [Pithus](https://pithus.org/) | Open-source APK analyzer with YARA rule hunting |

### Static Analysis Tools

1. [Androguard](https://github.com/androguard/androguard) – powerful reverse engineering and static analysis library, integrates well with other tools
2. [MobSF (Mobile Security Framework)](https://github.com/MobSF/Mobile-Security-Framework-MobSF) – all-in-one static, dynamic, and API pentesting framework for Android/iOS
3. [FlowDroid](https://github.com/secure-software-engineering/FlowDroid) – precise, context/flow/field/object-sensitive taint analysis for Android apps
4. [Amandroid](http://amandroid.sireum.org/) – static analysis framework for security vetting of Android apps
5. [Quark-Engine](https://github.com/quark-engine/quark-engine) – obfuscation-neglect Android malware scoring system
6. [APKLeaks](https://github.com/dwisiswant0/apkleaks) – scans APKs for URIs, endpoints & hardcoded secrets
7. [Mobile Audit](https://github.com/mpast/mobileAudit) – web app for static analysis & malware detection in APKs
8. [ClassyShark](https://github.com/google/android-classyshark) – standalone binary inspection tool for any Android executable
9. [StaCoAn](https://github.com/vincentcox/StaCoAn) – cross-platform static code analysis with GUI guidance
10. [PSCout](https://github.com/martin-nunova/pscout) – extracts Android permission specification from AOSP source via static analysis
11. [SUPER](https://github.com/SUPERAndroidAnalyzer/super) – Secure, Unified, Powerful and Extensible Rust Android Analyzer
12. [Trueseeing](https://github.com/fsecurelabs/trueseeing) – fast, automated, static vulnerability scanner and pentesting workbench for Android apps

### App Vulnerability Scanners

1. [QARK](https://github.com/linkedin/qark/) – LinkedIn's tool for scanning apps for security issues
2. [AndroBugs Framework](https://github.com/AndroBugs/AndroBugs_Framework) – efficient Android vulnerability scanner
3. [MobSF](https://github.com/MobSF/Mobile-Security-Framework-MobSF) – also functions as a full vulnerability scanner (see above)
4. [Nogotofail](https://github.com/google/nogotofail) – network traffic security testing tool

### Dynamic Analysis Tools

1. [Frida](https://frida.re/) – dynamic instrumentation toolkit for injecting scripts into native apps; the industry-standard hooking/tracing tool
2. [Objection](https://github.com/sensepost/objection) – Frida-powered runtime mobile exploration toolkit; SSL pinning bypass, filesystem/keychain access, no jailbreak/root required
3. [MobSF Dynamic Analyzer](https://github.com/MobSF/Mobile-Security-Framework-MobSF) – dynamic analysis on emulator/device with API monitoring, traffic capture, and Frida integration
4. [Drozer](https://github.com/WithSecureLabs/drozer) – security testing framework for Android, assesses apps and devices for vulnerabilities
5. [Inspeckage](https://github.com/ac-pm/Inspeckage) – Android package inspector, dynamic analysis with API hooks (Xposed module)
6. [House](https://github.com/nccgroup/house) – runtime mobile application analysis toolkit with web GUI, powered by Frida
7. [Runtime Mobile Security (RMS)](https://github.com/m0bilesecurity/RMS-Runtime-Mobile-Security) – web UI for manipulating Android/iOS apps at runtime via Frida
8. [friTap](https://github.com/fkie-cad/friTap) – intercepts SSL/TLS via Frida, extracts keys and decrypted payload as PCAP in real time
9. [AppMon](https://github.com/dpnishant/appmon) – automated framework for monitoring/tampering with system API calls (Frida-based)
10. [MARA Framework](https://github.com/xtiankisutsa/MARA_Framework) – Mobile Application Reverse Engineering and Analysis Framework
11. [Xposed Framework](https://github.com/rovo89/Xposed) – module-based framework for modifying system/app behavior at runtime without touching APKs
12. [Android_application_analyzer](https://github.com/NotSoSecure/android_application_analyzer) – analyzes local storage content of Android apps
13. [Androl4b](https://github.com/sh4hin/Androl4b) – preconfigured VM for Android app assessment, RE, and malware analysis
14. [Decompiler.com](https://www.decompiler.com/) – online APK and Java decompiler

### Reverse Engineering

1. [Jadx / Jadx-GUI](https://github.com/skylot/jadx) – Dex-to-Java decompiler, the current de facto standard for reading Android bytecode as readable Java
2. [Apktool](https://ibotpeaches.github.io/Apktool/) – decompiles/rebuilds APK resources and Smali, essential for repackaging and resource-level edits
3. [Smali/Baksmali](https://github.com/JesusFreke/smali) – assembler/disassembler for the dex format
4. [Ghidra](https://github.com/NationalSecurityAgency/ghidra) – NSA's reverse engineering suite; strong for native (.so) library analysis alongside Java-layer tools
5. [Dex2Jar](https://github.com/pxb1988/dex2jar) – dex to jar converter
6. [Enjarify](https://github.com/google/enjarify) – dex to jar converter from Google, handles cases dex2jar struggles with
7. [Bytecode Viewer](https://github.com/Konloch/bytecode-viewer) – all-in-one Java/Android decompiler GUI (integrates CFR, Procyon, Krakatau, FernFlower, JD-GUI)
8. [CFR](https://www.benf.org/other/cfr/) – Java decompiler
9. [JD-GUI](https://github.com/java-decompiler/jd-gui) – Java decompiler with GUI
10. [Krakatau](https://github.com/Storyyeller/Krakatau) – Java decompiler/assembler
11. [radare2](https://github.com/radareorg/radare2) – reverse engineering framework, useful for native library analysis
12. [Simplify](https://github.com/CalebFenton/simplify) – virtual machine-based Android deobfuscator
13. [Obfuscapk](https://github.com/ClaudiuGeorgiu/Obfuscapk) – modular Python tool for obfuscating APKs without source code (useful for testing detection resilience)
14. [apk-mitm](https://github.com/niklasstich/apk-mitm) – automatically preps APKs for HTTPS traffic inspection (disables cert pinning, enables user CAs)
15. [MVT (Mobile Verification Toolkit)](https://github.com/mvt-project/mvt) – forensic toolkit to identify signs of compromise (e.g. spyware) on Android/iOS devices
16. [Androguard](https://github.com/androguard/androguard) – also a core RE library (see Static Analysis)
17. [Dwarf](https://github.com/iGio90/Dwarf) – GUI-based debugger built on Frida for reverse engineering

### Fuzz Testing

1. [Honggfuzz](https://github.com/google/honggfuzz) – general-purpose, feedback-driven fuzzer with Android support
2. [Radamsa](https://gitlab.com/akihe/radamsa) – general-purpose mutation fuzzer, usable against Android inputs/interfaces

### App Repackaging Detectors

1. [FSquaDRA2](https://github.com/andrey-git/FSquaDRA2) – detects repackaged Android applications via resource hash comparison

### Market Crawlers / APK Downloaders

1. [PlaystoreDownloader](https://github.com/ClaudiuGeorgiu/PlaystoreDownloader) – downloads APKs directly from Google Play by package name
2. [gplaycli](https://github.com/matlink/gplaycli) – command-line tool to search/download apps from Google Play

### Misc Tools

1. [mitmproxy](https://github.com/mitmproxy/mitmproxy) – interactive HTTPS proxy, standard for inspecting mobile app traffic
2. [AXMLPrinter2 / apktool built-in decoder](https://ibotpeaches.github.io/Apktool/) – converts binary AndroidManifest.xml to readable XML (now bundled in Apktool)
3. [Android Vulnerability Test Suite (android-vts)](https://github.com/AndroidVTS/android-vts) – scans a device for a set of known vulnerabilities
4. [Genymotion](https://www.genymotion.com/) – Android emulator widely used for security testing on virtual devices with root access
5. [nRF Connect / Bluetooth security tools](https://github.com/seemoo-lab/internalblue) – InternalBlue: Bluetooth experimentation framework based on RE of Broadcom BT controllers

### Vulnerable Applications for Practice

1. [Damn Insecure Vulnerable Application (DIVA)](https://github.com/payatu/diva-android)
2. [OWASP MASTG Hacking Playground (mastg-hacking-playground)](https://github.com/OWASP/mastg-hacking-playground) – official vulnerable apps companion to the OWASP MASTG
3. [InsecureShop](https://github.com/optiv/insecureshop)
4. [Android InsecureBankv2](https://github.com/dineshshetty/Android-InsecureBankv2)
5. [Oversecured Vulnerable Android App (OVAA)](https://github.com/oversecured/ovaa)
6. [GoatDroid](https://github.com/jackMannino/OWASP-GoatDroid-Project)
7. [Sieve (OWASP MASTG UnCrackable Apps)](https://github.com/OWASP/mastg-hacking-playground) – classic crackme-style targets for practicing RE and dynamic bypass techniques

---

## Academic / Research / Publications / Books

### Research Papers

1. [Exploit Database Papers](https://www.exploit-db.com/papers/)
2. [Android security-related presentations (jacobsoo/AndroidSlides)](https://github.com/jacobsoo/AndroidSlides)

### Books & Guides

1. [SEI CERT Android Secure Coding Standard](https://wiki.sei.cmu.edu/confluence/display/android/Android+Secure+Coding+Standard)
2. [OWASP Mobile Application Security Testing Guide (MASTG)](https://mas.owasp.org/MASTG/) – the current, actively maintained industry-standard manual for mobile app security testing and reverse engineering (successor to the older MSTG)
3. [OWASP Mobile Application Security Verification Standard (MASVS)](https://mas.owasp.org/MASVS/) – baseline security requirements checklist that MASTG test cases map to

### Others

1. [doridori/Android-Security-Reference](https://github.com/doridori/Android-Security-Reference)
2. [b-mueller/android_app_security_checklist](https://github.com/b-mueller/android_app_security_checklist)
3. [tanprathan/MobileApp-Pentest-Cheatsheet](https://github.com/tanprathan/MobileApp-Pentest-Cheatsheet)
4. [HackTricks – Android App Pentesting](https://book.hacktricks.wiki/en/mobile-pentesting/android-app-pentesting/index.html) – actively updated, practical Android pentesting reference (Frida, Objection, bypass techniques, etc.)

---

## Exploits / Vulnerabilities / Bugs

### Lists & Bulletins

1. [Android Security Bulletins](https://source.android.com/docs/security/bulletin) – official monthly patch and vulnerability disclosures from Google
2. [Android's reported CVEs (CVE Details)](https://www.cvedetails.com/vulnerability-list/vendor_id-1224/product_id-19997/Google-Android.html)
3. [OWASP Mobile Top 10](https://owasp.org/www-project-mobile-top-10/) – current version of the standard mobile vulnerability taxonomy
4. [Exploit Database – Android search](https://www.exploit-db.com/search?q=android)
5. [Google Android Security Team's PHA Classifications](https://developers.google.com/android/play-protect/phacategories) – official classification of Potentially Harmful Applications (malware)

### Malware Datasets & Research

1. [Android Malware Github repo (ashishb/android-malware)](https://github.com/ashishb/android-malware)
2. [AndroZoo](https://androzoo.uni.lu/) – large, growing collection of Android apps from multiple sources including Google Play, for research use
3. [Contagio Mobile Malware Mini Dump](http://contagiominidump.blogspot.com)
4. [CIC Android Adware and General Malware Dataset](https://www.unb.ca/cic/datasets/android-adware.html)
5. [Drebin Dataset](https://www.sec.tu-bs.de/~danarp/drebin/)
6. [Koodous](https://koodous.com) – community-driven malware sample repository with YARA rule hunting (also listed above as an analyzer)

### Bounty Programs

1. [Google Play Security Reward Program (GPSRP)](https://bughunters.google.com/about/rules/6291763456212992) – rewards for vulnerabilities found in popular Android apps
2. [Android and Google Devices Security Reward Program](https://bughunters.google.com/about/rules/android-and-google-devices)

### How to Report Security Issues

1. [Android – reporting security issues](https://source.android.com/docs/security/overview/updates-resources#report-issues)
2. [Google Bug Hunters – Android program](https://bughunters.google.com/)
3. [B3nac/Android-Reports-and-Resources](https://github.com/B3nac/Android-Reports-and-Resources) – curated list of disclosed Android HackerOne reports and RE resources

---

## Blogs, Write-ups & Research Feeds

Ongoing sources of technical write-ups, exploit analyses, and industry commentary — far more valuable long-term than any static tool list, since this is where new techniques actually surface first.

### Vendor & Platform Research Teams

1. [Google Project Zero](https://projectzero.google/) – in-depth, technical write-ups of real 0-day and n-day exploits, including a recurring "In-the-Wild" series specifically on Android exploit chains
2. [Android Offensive Security Team Blog](https://androidoffsec.withgoogle.com/) – Google's own Android red team publishing deep technical posts on kernel/GPU/Binder exploitation (e.g. Qualcomm KGSL, Binder fuzzing)
3. [Google Online Security Blog](https://security.googleblog.com/) – official announcements on Android platform security, Play Protect, and ecosystem-wide defenses
4. [Google Bug Hunters Blog](https://bughunters.google.com/blog) – write-ups and reward program updates from Google's vulnerability reward programs, including Android and Google Play
5. [NCC Group Research Blog](https://research.nccgroup.com/) – regular mobile app pentest write-ups and tooling releases from a long-running research team
6. [WithSecure Labs Blog](https://labs.withsecure.com/) – successor to MWR Labs/F-Secure Labs, frequent Android/mobile research

### Independent & Vendor Security Research

1. [Oversecured Blog](https://blog.oversecured.com/) – frequent, highly technical Android vulnerability-class write-ups (deep-links, exported components, custom permissions, etc.)
2. [NowSecure Blog](https://www.nowsecure.com/blog/) – mobile app security research, threat analysis, and testing guidance
3. [Guardsquare Blog](https://www.guardsquare.com/blog) – Android app hardening, obfuscation, and reverse-engineering-resistance research (maintainers of ProGuard/DexGuard)
4. [MobSF Blog / Docs Updates](https://mobsf.github.io/docs/) – release notes and technique write-ups tied to the MobSF framework
5. [HackTricks – Android App Pentesting](https://book.hacktricks.wiki/en/mobile-pentesting/android-app-pentesting/index.html) – continuously updated practical playbook, more like a living cheat-sheet than a one-off post
6. [Payatu Blog](https://payatu.com/blog/) – Android/IoT pentesting write-ups from the team behind DIVA

### CTF & Vulnerability Write-ups

1. [CVE Details – Google Android](https://www.cvedetails.com/vendor/1224/Google.html) – browse individual CVEs, many of which link out to the original researcher's write-up
2. [GitHub topic: android-exploitation](https://github.com/topics/android-exploitation) – community-maintained PoCs and write-ups for specific Android CVEs
3. [Exploit-DB – Android](https://www.exploit-db.com/search?q=android) – submitted PoC exploits and advisories

---

## Communities, Forums & Conferences

1. [r/AskNetsec](https://www.reddit.com/r/AskNetsec/) and [r/netsec](https://www.reddit.com/r/netsec/) – general security discussion, Android write-ups get shared regularly
2. [XDA Developers Security Forum](https://forum.xda-developers.com/) – long-running community around Android rooting, ROMs, and device-level security
3. [OWASP MAS Slack / Community](https://mas.owasp.org/contributing/) – official community channel for the MASVS/MASTG project, good place to ask testing methodology questions
4. [DEF CON Mobile/Android talks archive](https://media.defcon.org/) – recordings and slides from years of Android-focused DEF CON talks
5. [Black Hat Briefings Archive](https://www.blackhat.com/html/archives.html) – searchable archive of Black Hat talks, many with full Android exploitation papers/slides

---
