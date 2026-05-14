<h1 align="center">Juwon Bang &nbsp;<sub><sup>(優心)</sup></sub></h1>
<p align="center">
  <em>DFIR &amp; Detection Engineering · Tokyo, Japan</em>
</p>

<p align="center">
  <a href="mailto:juwon1405.jp@gmail.com">
    <img src="https://img.shields.io/badge/contact-juwon1405.jp%40gmail.com-555?style=flat-square&logo=gmail&logoColor=white" alt="email"></a>
</p>

---

Building autonomous detection systems and architectural security guarantees.
Currently exploring **agentic DFIR** &mdash; MCP-based forensic agents that
encode the reasoning pattern of a senior analyst as architecture, not as a prompt.

### 🔍 Focus

- **Digital Forensics &amp; Incident Response** &nbsp;·&nbsp; Windows / macOS / Linux
- **Detection Engineering** &nbsp;·&nbsp; MITRE ATT&amp;CK coverage modeling, Sigma
- **DevSecOps &amp; Security Automation**
- **Agentic AI for Security** &nbsp;·&nbsp; MCP, audit-chained reasoning loops

### 🛠️ Stack

<p>
  <img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white">
  <img src="https://img.shields.io/badge/Bash-4EAA25?style=flat-square&logo=gnubash&logoColor=white">
  <img src="https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black">
  <img src="https://img.shields.io/badge/macOS-000000?style=flat-square&logo=apple&logoColor=white">
  <img src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white">
  <img src="https://img.shields.io/badge/Splunk-000000?style=flat-square&logo=splunk&logoColor=white">
  <img src="https://img.shields.io/badge/Volatility-1F1F1F?style=flat-square">
  <img src="https://img.shields.io/badge/SANS%20SIFT-CC0000?style=flat-square">
  <img src="https://img.shields.io/badge/MITRE%20ATT%26CK-4F46E5?style=flat-square">
  <img src="https://img.shields.io/badge/Sigma-FF6B35?style=flat-square">
  <img src="https://img.shields.io/badge/MCP-1A73E8?style=flat-square">
</p>

### 📌 Featured Projects

#### 🎯 Agentic-DART &nbsp;<sub><sup>*flagship — SANS FIND EVIL! 2026*</sup></sub>

[![Agentic-DART](https://raw.githubusercontent.com/Juwon1405/agentic-dart/main/agentic-dart-hero.png)](https://github.com/Juwon1405/agentic-dart)

> Autonomous DFIR agent that thinks like a senior analyst. Architecture-first,
> not prompt-first. **61 typed forensic MCP tools** (36 native + 25 SIFT
> Workstation adapters) across **10 / 12 MITRE ATT&amp;CK enterprise tactics**
> (TA0009 Collection and TA0011 C2 are Phase 2 roadmap), **43 / 43 tests passing**
> on a fresh clone (CI green on Python 3.10/3.11/3.12/3.13), **1182-line
> senior-analyst playbook v3** synthesizing Mandiant + Bianco + Diamond +
> Palantir ADS + MaGMa UCF + TaHiTI hunt cycle (42 references).
> Read-only MCP boundary makes destructive ops impossible by construction.
> Three evaluation tiers: synthetic reference (recall=1.0), noise-injected
> realistic at ~1:30 IOC:benign (recall=1.0), and **NIST CFReDS Hacking
> Case** (community-trusted external benchmark) — v0.6.0 scores 0.50/0.80
> strict/lenient on 10 sampled NIST findings, up from v0.5.3's 0.10/0.40 (supply-chain sweeps + collector adapter added in v0.6.0),
> after `parse_registry_hive` (issue #52) shipped. Remaining CFReDS gaps
> (#53/#54/#55) are explicit Phase 2 deliverables. Starts as agentic DFIR;
> designed to expand toward agentic SOC and beyond.

<sub>→ [github.com/Juwon1405/agentic-dart](https://github.com/Juwon1405/agentic-dart) &nbsp;·&nbsp; [Submission to SANS FIND EVIL! 2026](https://findevil.devpost.com/) &nbsp;·&nbsp; MIT</sub>

#### Other projects

<table>
<tr>
<td width="50%" valign="top">

#### 🔌 [agentic-dart-collector-adapter](https://github.com/Juwon1405/agentic-dart-collector-adapter) &nbsp;<sub><sup>*new — Phase 1.3*</sup></sub>

<a href="https://github.com/Juwon1405/agentic-dart-collector-adapter">
<img src="https://img.shields.io/github/stars/Juwon1405/agentic-dart-collector-adapter?style=flat-square&color=f5b400" alt="stars">
<img src="https://img.shields.io/github/last-commit/Juwon1405/agentic-dart-collector-adapter?style=flat-square&color=1A73E8" alt="last commit">
<img src="https://img.shields.io/badge/lang-python-3776AB?style=flat-square" alt="python">
<img src="https://img.shields.io/badge/license-MIT-blue?style=flat-square" alt="MIT">
</a>

> **Velociraptor → evidence_root adapter** &mdash; stdlib-only Python
> layer that converts Velociraptor offline-collector ZIPs into the
> `evidence_root` layout Agentic-DART consumes. Seeds chain-of-custody
> (manifest.json + SHA-256 index). 27/27 tests, CI Linux+macOS × py3.10/11/12.

</td>
<td width="50%" valign="top">

#### 🍎 [yushin-mac-artifact-collector](https://github.com/Juwon1405/yushin-mac-artifact-collector)

<a href="https://github.com/Juwon1405/yushin-mac-artifact-collector">
<img src="https://img.shields.io/github/stars/Juwon1405/yushin-mac-artifact-collector?style=flat-square&color=f5b400" alt="stars">
<img src="https://img.shields.io/github/last-commit/Juwon1405/yushin-mac-artifact-collector?style=flat-square&color=1A73E8" alt="last commit">
<img src="https://img.shields.io/badge/lang-shell-4EAA25?style=flat-square" alt="shell">
</a>

> **macOS DFIR Artifact Collector** &mdash; single-file, zero-dep,
> modular collection script. Originated the supply-chain IOC sweeps
> (litellm PyPI 2026-03 + generic) now ported into `agentic-dart` as
> cross-platform MCP functions (`dart_mcp._v05_supply_chain`).

</td>
</tr>
<tr>
<td width="50%" valign="top">

#### 🔬 [yushin-mac-forensics-platform](https://github.com/Juwon1405/yushin-mac-forensics-platform) &nbsp;<sub><sup>*to be repositioned*</sup></sub>

<a href="https://github.com/Juwon1405/yushin-mac-forensics-platform">
<img src="https://img.shields.io/github/stars/Juwon1405/yushin-mac-forensics-platform?style=flat-square&color=f5b400" alt="stars">
<img src="https://img.shields.io/github/last-commit/Juwon1405/yushin-mac-forensics-platform?style=flat-square&color=1A73E8" alt="last commit">
<img src="https://img.shields.io/badge/lang-python-3776AB?style=flat-square" alt="python">
</a>

> **macOS DFIR Forensics Platform** &mdash; Flask-based platform that
> ingests collector ZIPs &amp; disk images, parses 30+ artifact
> categories. Planned for repositioning as the Agentic-DART web UI
> (read findings.json + audit.jsonl, render in browser) once SANS
> submission window closes.

</td>
<td width="50%" valign="top">

#### 📓 [GitNote](https://github.com/Juwon1405/GitNote)

<a href="https://github.com/Juwon1405/GitNote">
<img src="https://img.shields.io/github/stars/Juwon1405/GitNote?style=flat-square&color=f5b400" alt="stars">
<img src="https://img.shields.io/github/last-commit/Juwon1405/GitNote?style=flat-square&color=1A73E8" alt="last commit">
<img src="https://img.shields.io/badge/lang-markdown-555555?style=flat-square" alt="markdown">
</a>

> **GitNote** &mdash; curated personal knowledge base in InfoSec &amp;
> computer science. A long-running collection of notes, references,
> and code snippets from years of DFIR / detection engineering work.

</td>
</tr>
</table>

<details>
<summary><sub>📦 Archived projects</sub></summary>

<br/>

#### 🧪 [yushin-gendfir-rag](https://github.com/Juwon1405/yushin-gendfir-rag) &nbsp;<sub><sup>*archived*</sup></sub>

Unofficial Python replication of Loumachi, Ghanem &amp; Ferrag (2024). RAG + LLM pipeline for DFIR cyber-incident timeline analysis. The work in this repository served as a foundation that informed the design of [agentic-dart](https://github.com/Juwon1405/agentic-dart), which supersedes it with agentic (rather than pure RAG) reasoning and a hardened MCP surface. Kept public as a reference artifact.

#### 🍎 [yushin-mac-artifact-collector](https://github.com/Juwon1405/yushin-mac-artifact-collector) &nbsp;<sub><sup>*archived*</sup></sub>

Single-file bash DFIR artifact collector for macOS hosts where Velociraptor is not an option. Originator of the supply-chain IOC sweep patterns (litellm PyPI 2026-03, npm typosquat detection) now ported and generalized into [agentic-dart](https://github.com/Juwon1405/agentic-dart). Kept public as a supply-chain reference.

#### 🍎 [yushin-mac-forensics-platform](https://github.com/Juwon1405/yushin-mac-forensics-platform) &nbsp;<sub><sup>*archived*</sup></sub>

Flask-based platform that ingested collector ZIPs &amp; disk images (DD/RAW/E01/AFF/DMG), parsed 30+ artifact categories, and produced searchable evidence + PDF incident reports. Analysis layer superseded by [agentic-dart](https://github.com/Juwon1405/agentic-dart); planned revival as Agentic-DART web UI in a future roadmap phase.

</details>

### 📖 Published Work

- ***Network Attack Packet Analysis for Security Practitioners* &nbsp;·&nbsp; 보안 실무자를 위한 네트워크 공격 패킷 분석** &nbsp;<sub>(co-author, lead)</sub><br>
  Freelec, 2019.11 &nbsp;·&nbsp; ISBN 9788965402589 &nbsp;·&nbsp; ~370 pp.<br>
  A practitioner's reference covering DDoS, web exploitation, malicious traffic, wireless intrusion, system exploitation, and large-volume packet analysis.<br>
  <sub>→ [Yes24](https://www.yes24.com/Product/Goods/83538369) &nbsp;·&nbsp; [Aladin](https://www.aladin.co.kr/shop/wproduct.aspx?ItemId=217703927) &nbsp;·&nbsp; [Kyobo](https://product.kyobobook.co.kr/detail/S000001019678) &nbsp;·&nbsp; [Google Books](https://books.google.com/books?id=SIrIywEACAAJ)</sub>

### 🏆 Selected Recognition

- **🥇 Gold Prize**, 2017 Korea Open-Source Software Developer Contest &nbsp;<sub>(NIPA, *national OSS award*)</sub>
- **📜 Patent (filed)**: *Security Event Correlation Analysis Apparatus* &nbsp;<sub>(2018, Netmarble Corp.)</sub>
- **🎯 4th place**, 2017 CCE National Cyber Defense Competition &nbsp;<sub>(National Intelligence Service of Korea)</sub>
- **🐛 Special Prize**, 2015 LINE Bug Bounty Program &nbsp;<sub>(LINE Corp.)</sub>

### 🎥 Community

- **YouTube**: [DoubleS1405](https://www.youtube.com/c/DoubleS1405) &mdash; long-running Korean-language information-security lecture channel (2014&ndash;present)

### 📚 Curated lists

- [**Awesome Stars** (GitNote)](https://github.com/Juwon1405/GitNote/blob/main/Resources/awesome-stars.md) ⭐ &mdash; **Starred repos categorized into curated buckets** (DFIR / Blue Team / AI / Red Team / Malware / OSINT / etc.), regenerated periodically after curation passes.
- [**DFIR**](https://github.com/stars/Juwon1405/lists/dfir) &mdash; Digital Forensics &amp; Incident Response
- [**BlueTeam**](https://github.com/stars/Juwon1405/lists/blueteam) &mdash; Defensive operations &amp; SOC
- [**Tools &amp; Tips**](https://github.com/stars/Juwon1405/lists/tools-tips) &mdash; Analysis utilities
- [**DevSecOps**](https://github.com/stars/Juwon1405/lists/devsecops) &mdash; Security automation &amp; AI
- [**Gist**](https://gist.github.com/Juwon1405) &mdash; Code snippets

### 🤝 Open to

Research collaboration · CTF · CSIRT exchange · Open-source security tooling

---

<p align="center">
  <a href="https://github.com/Juwon1405?tab=repositories">
    <img src="https://img.shields.io/github/followers/Juwon1405?style=flat-square&label=Followers&color=1A73E8" alt="followers">
  </a>
  &nbsp;
  <a href="https://github.com/Juwon1405?tab=stars">
    <img src="https://img.shields.io/github/stars/Juwon1405?style=flat-square&label=Stars&color=f5b400" alt="stars">
  </a>
  &nbsp;
  <a href="https://github.com/Juwon1405/agentic-dart">
    <img src="https://img.shields.io/github/stars/Juwon1405/agentic-dart?style=flat-square&label=agentic-dart&color=DD2C00" alt="agentic-dart stars">
  </a>
  &nbsp;
  <a href="https://github.com/Juwon1405/agentic-dart/actions/workflows/ci.yml">
    <img src="https://github.com/Juwon1405/agentic-dart/actions/workflows/ci.yml/badge.svg?branch=main" alt="agentic-dart CI">
  </a>
</p>
