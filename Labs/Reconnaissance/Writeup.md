# Reconnaissance & OSINT — Passive Footprinting (Mini Project)

**Target:** example-target.com (used for demonstration).  
**Objective:** Demonstrate passive information gathering (OSINT) techniques to map external attack surface and identify publicly exposed assets.  
**Authorization:** Educational / lab exercise — only passive techniques used.

---

## Tools
- nslookup, dig  
- whois  
- crt.sh (Certificate Transparency)  
- archive.org (Wayback Machine)  
- ipinfo.io (reverse IP)  
- Google Dorking  
- Browser / manual inspection

---

## Steps Taken
1. **DNS discovery** – `nslookup example-target.com` → captured A records and name servers.  
2. **Whois lookup** – collected registrar, registration dates.  
3. **Certificate transparency** – searched `crt.sh` for subdomains.  
4. **Wayback Machine** – viewed historical versions for hidden content.  
5. **Reverse IP** – found other domains on same host.  
6. **Google Dorking** – `site:example-target.com filetype:pdf` to locate exposed files.

---

## Key Findings
- crt.sh returned additional subdomains not on main site.  
- Wayback showed old pages exposing sensitive endpoints.  
- SSL certificates used strong ciphers (TLS 1.3 + AES-GCM).  

---

## Impact & Recommendations
- Remove/secure forgotten subdomains; monitor cert transparency logs.  
- Limit public document exposure.  
- Perform periodic attack-surface reviews.

---

## Learnings
- Passive OSINT reveals valuable data without active scanning.  
- Regular documentation helps track changes over time.
