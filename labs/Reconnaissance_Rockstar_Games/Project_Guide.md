# Project Guide: Rockstar Games - Passive Reconnaissance & AI Integration

## 1. Project Overview

This project showcases a full-cycle reconnaissance effort, from initial data collection to professional report delivery. The primary goal was to conduct **OSINT (Open Source Intelligence)** on `rockstargames.com` to map its full attack surface and identify high-value targets, such as internal development systems and APIs.

### Key Skills Demonstrated

* **OSINT & Footprinting:** Expertise in passive data collection using DNS, WHOIS, and SSL certificate analysis.
* **Vulnerability Prioritization:** Ability to classify raw data into actionable security findings (e.g., Critical, High).
* **AI Integration for Reporting:** Strategic use of the Gemini LLM to rapidly synthesize raw technical notes into a polished, industry-standard formal report.

## 2. Report Division and Audience

This project is divided into three distinct reports, each tailored for a different audience:

| Report File | Target Audience | Primary Focus |
| :--- | :--- | :--- |
| `Formal_Report.md` | Non-Technical Management, Executives | Risk, Impact, and high-level Remediation Strategy. |
| `Technical_Report.md` | Security Engineers, Developers | Detailed command outputs, specific vulnerabilities, and proof of concept (PoC) references. |
| `Project_Guide.md` (This file) | Peers, Hiring Managers | Project scope, methodology, and demonstration of AI-leveraged efficiency. |

## 3. Critical Methodology Highlight

The most effective technique utilized was **SSL Certificate Analysis (SAN Extraction)**. By analyzing the public security certificate of the main domain, we were able to legally and passively discover **30+ unlisted subdomains**, including sensitive internal-facing systems (`cms-prod`, `www-eaa`) which represent high-risk attack vectors.
