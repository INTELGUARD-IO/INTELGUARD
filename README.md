<p align="center">
  <a href="https://intelguard.io" target="_blank" rel="noopener">
    <img src="https://intelguard.io/logo.png" width="220" alt="IntelGuard logo"/>
  </a>
</p>

<h1 align="center">IntelGuard – True Threat Feed™</h1>

<p align="center">
  Analyst-validated threat intelligence for blocklists that actually block threats.
</p>

<p align="center">
  <a href="https://intelguard.io/join">
    <img alt="Join the Waitlist" src="https://img.shields.io/badge/Join%20the%20Waitlist-000"/>
  </a>&nbsp;
  <a href="https://intelguard.io/features">
    <img alt="Start Trial" src="https://img.shields.io/badge/Start%20Trial-1aa34a"/>
  </a>&nbsp;
  <a href="https://intelguard.io/integrations">
    <img alt="Docs & Integrations" src="https://img.shields.io/badge/Docs%20%26%20Integrations-0b5fff"/>
  </a>&nbsp;
  <a href="https://www.linkedin.com/company/intelguard">
    <img alt="Follow on LinkedIn" src="https://img.shields.io/badge/Follow%20on%20LinkedIn-0A66C2?logo=linkedin&logoColor=white"/>
  </a>&nbsp;
  <a href="#free-mini-feeds">
    <img alt="Free Mini Feeds" src="https://img.shields.io/badge/Free%20Mini%20Feeds-Demo-lightgrey"/>
  </a>&nbsp;
  <a href="https://github.com/INTELGUARD-IO/INTELGUARD/stargazers">
    <img alt="GitHub stars" src="https://img.shields.io/github/stars/INTELGUARD-IO/INTELGUARD?style=social"/>
  </a>
</p>

---

## Why IntelGuard
Security teams don’t need another giant list of noisy Indicators of Compromise. They need **confident, maintainable blocklists** they can trust in production.

**IntelGuard** combines multi-source telemetry with an **analyst-overseen scoring model** (our *True Threat Feed™* approach) to deliver compact, high-confidence IP/domain feeds.

> Our promise: *Fewer false positives, faster blocks, clearer evidence.*

---

## What makes it different
- **Analyst-validated scoring.** Data is processed by our model and **reviewed by analysts** before promotion to production feeds.
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

<a id="free-mini-feeds"></a>
## Free mini-feeds (demo)
Small, rotating samples to help you test your tooling.

- **IPv4 (text):** `https://feed.intelguard.io/feed/sample?type=ipv4&format=txt`
- **Domains (text):** `https://feed.intelguard.io/feed/sample?type=domain&format=txt`

> ⚠️ *Mini-feeds are a demonstration subset with stricter confidence thresholds and rate-limits. They are not a replacement for the full service.*

### Quick usage — IPv4 list
```bash
# Pull IPv4 demo blocklist (save to file)
curl -sSfL 'https://feed.intelguard.io/feed/sample?type=ipv4&format=txt' \
  -H 'Accept: text/plain' \
  -o /tmp/intelguard_ipv4.txt
