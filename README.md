<p align="center">
<a href="https://intelguard.io" target="_blank" rel="noopener">
<img src="https://intelguard.io/logo.png" width="220" alt="IntelGuard logo"/>
</a>
</p>


<h1 align="center">IntelGuard – True Threat Feed™</h1>


<p align="center">
Analyst‑validated threat intelligence for blocklists that actually block threats.
</p>


<p align="center">
<a href="https://intelguard.io/join"><img alt="Join the waitlist" src="https://img.shields.io/badge/Join%20the%20Waitlist-black"/></a>
<a href="#free-mini-feeds"><img alt="Free mini feeds" src="https://intelguard.io/true-threat-feeds"/></a>
<a href="https://github.com/ORG/REPO/stargazers"><img alt="GitHub stars" src="https://img.shields.io/github/stars/ORG/REPO?style=social"/></a>
</p>


---


## Why IntelGuard
Security teams don’t need another giant list of noisy Indicators of Compromise. They need **confident, maintainable blocklists** they can trust in production.


**IntelGuard** combines multi‑source telemetry with an **analyst‑overseen scoring model** (our *True Threat Feed™* approach) to deliver compact, high‑confidence IP/domain feeds.


> Our promise: *Fewer false positives, faster blocks, clearer evidence.*


---


## What makes it different
- **Analyst‑validated scoring.** Data is processed by our model and **reviewed by analysts** before promotion to production feeds.
- **Signal over noise.** We prioritize quality and freshness over volume, so your controls stay lean and effective.
- **Context included.** Each indicator carries useful context (e.g., confidence, family/category, country/ASN where applicable) to speed up decisions.
- **Ready for ops.** Lightweight text/CSV/JSON outputs work with firewalls, SIEM/SOAR, and network controls.


---


## How it works (at a glance)
1. **Aggregate** – We continuously ingest from vetted intel sources.
2. **Validate** – Indicators are tested across multiple lenses and scored.
3. **Curate** – **Human analysts** apply promotion gates and sanity checks.
4. **Deliver** – Only the **validated** set lands in the public/tenant feeds.


*We do not publish raw or unverified data.*


---


## Free mini‑feeds (demo)
Small, rotating samples to help you test your tooling.


- **IPv4 (text):** `https://feed.intelguard.io/feed/sample?type=ipv4&format=txt`
- **Domains (text):** `https://feed.intelguard.io/feed/sample?type=domain&format=txt`


> ⚠️ *Mini‑feeds are a demonstration subset with stricter confidence thresholds and rate‑limits. They are not a replacement for the full service.*


**Quick usage — IPv4 list**
# Pull IPv4 demo blocklist (and save to file)
curl -sSfL 'https://feed.intelguard.io/feed/sample?type=ipv4&format=txt'

**Quick usage — Domain list**
# Pull Domain demo blocklist (and save to file)
curl -sSfL 'https://feed.intelguard.io/feed/sample?type=domain&format=txt'
