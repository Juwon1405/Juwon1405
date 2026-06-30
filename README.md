<!-- Profile banner — adapts to the viewer's light/dark theme -->
<p align="center">
  <!-- Single dark banner: GitHub's <picture> theme-swap follows the browser's
       prefers-color-scheme, not the GitHub theme, so a light banner can land on
       a dark profile (and look stark). A dark banner reads well on both. -->
  <img alt="Juwon Bang — DFIR &amp; Detection Engineering, Tokyo" src="./assets/banner-dark.svg" width="100%">
</p>

<p align="center">
  <a href="https://juwon1405.github.io/"><img src="https://img.shields.io/badge/Website-juwon1405.github.io-0d0d0e?style=flat-square&labelColor=0d0d0e&color=b8311f" alt="website"></a>
  &nbsp;
  <a href="mailto:juwon1405.jp@gmail.com"><img src="https://img.shields.io/badge/Email-juwon1405.jp-1c1c20?style=flat-square&logo=gmail&logoColor=e2ddd2&labelColor=1c1c20" alt="email"></a>
  &nbsp;
  <a href="https://www.youtube.com/c/DoubleS1405"><img src="https://img.shields.io/badge/YouTube-DoubleS1405-1c1c20?style=flat-square&logo=youtube&logoColor=e2ddd2&labelColor=1c1c20" alt="youtube"></a>
  &nbsp;
  <a href="https://github.com/Juwon1405?tab=followers"><img src="https://img.shields.io/github/followers/Juwon1405?style=flat-square&label=Follow&labelColor=1c1c20&color=8b6914" alt="followers"></a>
</p>

---

Building autonomous detection systems and architectural security guarantees.
Currently exploring **agentic DFIR** &mdash; MCP-based forensic agents that
encode the reasoning pattern of a senior analyst as *architecture, not as a prompt*.

> The interesting problem in "AI for security" isn't the model &mdash; it's the
> **architecture**: tool boundaries, deterministic correlation, evidence chains,
> audit trails. Guardrails belong in the surface, not the system prompt.

### &#9670;&nbsp; Focus

- **Digital Forensics &amp; Incident Response** &nbsp;&middot;&nbsp; Windows / macOS / Linux
- **Detection Engineering** &nbsp;&middot;&nbsp; MITRE ATT&amp;CK coverage modeling, Sigma
- **DevSecOps &amp; Security Automation**
- **Agentic AI for Security** &nbsp;&middot;&nbsp; MCP, audit-chained reasoning loops
- **Personal Agentic Systems** &nbsp;&middot;&nbsp; trading, market intelligence, operator dashboards

### &#9670;&nbsp; Stack

<p>
  <img src="https://img.shields.io/badge/Python-1c1c20?style=flat-square&logo=python&logoColor=4584b6&labelColor=1c1c20">
  <img src="https://img.shields.io/badge/Bash-1c1c20?style=flat-square&logo=gnubash&logoColor=89e051&labelColor=1c1c20">
  <img src="https://img.shields.io/badge/Linux-1c1c20?style=flat-square&logo=linux&logoColor=fcc624&labelColor=1c1c20">
  <img src="https://img.shields.io/badge/macOS-1c1c20?style=flat-square&logo=apple&logoColor=e2ddd2&labelColor=1c1c20">
  <img src="https://img.shields.io/badge/Docker-1c1c20?style=flat-square&logo=docker&logoColor=2496ed&labelColor=1c1c20">
</p>
<p>
  <img src="https://img.shields.io/badge/MCP-1c1c20?style=flat-square&logo=anthropic&logoColor=e2ddd2&labelColor=1c1c20">
  <img src="https://img.shields.io/badge/Splunk-1c1c20?style=flat-square&logo=splunk&logoColor=ed0080&labelColor=1c1c20">
  <img src="https://img.shields.io/badge/Volatility-1c1c20?style=flat-square&labelColor=1c1c20&color=1c1c20">
  <img src="https://img.shields.io/badge/SANS%20SIFT-1c1c20?style=flat-square&labelColor=1c1c20&color=1c1c20">
  <img src="https://img.shields.io/badge/MITRE%20ATT%26CK-1c1c20?style=flat-square&labelColor=1c1c20&color=1c1c20">
  <img src="https://img.shields.io/badge/Sigma-1c1c20?style=flat-square&labelColor=1c1c20&color=1c1c20">
</p>

### &#9670;&nbsp; Featured Projects

#### Pinned reading order

| Order | Repository | Signal |
| --- | --- | --- |
| 1 | [agentic-dart](https://github.com/Juwon1405/agentic-dart) | Flagship agentic DFIR system. |
| 2 | [yushin-trade-showcase](https://github.com/Juwon1405/yushin-trade-showcase) | Private autonomous trading cockpit, public operator surface. |
| 3 | [yushin-watch-showcase](https://github.com/Juwon1405/yushin-watch-showcase) | Private market-intelligence monitor for luxury watches. |
| 4 | [yushin-mac-forensics-platform](https://github.com/Juwon1405/yushin-mac-forensics-platform) | Archived DFIR intelligence platform with evidence review and reporting surfaces. |
| 5 | [yushin-mac-artifact-collector](https://github.com/Juwon1405/yushin-mac-artifact-collector) | Archived macOS triage collector and supply-chain IOC reference. |
| 6 | [yushin-gendfir-rag](https://github.com/Juwon1405/yushin-gendfir-rag) | Archived DFIR research replication behind the agentic intelligence direction. |

#### 🎯 Agentic-DART &nbsp;<sub><sup>*flagship — SANS FIND EVIL! 2026*</sup></sub>

[![Agentic-DART](https://raw.githubusercontent.com/Juwon1405/agentic-dart/main/agentic-dart-hero.png)](https://github.com/Juwon1405/agentic-dart)

> Autonomous DFIR agent. Architecture-first, not prompt-first. Read-only MCP
> surface (native pure-Python + SIFT adapters) makes destructive ops impossible
> by construction — a typed, read-only toolset built from native Python plus
> SIFT adapters, a full passing test suite, and ground-truth-scored case studies
> on real-world images. External case-study slots
> include NIST CFReDS, Ali Hadi, and Digital Corpora M57. SANS FIND EVIL! 2026
> entry.

<sub>→ [github.com/Juwon1405/agentic-dart](https://github.com/Juwon1405/agentic-dart) &nbsp;·&nbsp; [Submission to SANS FIND EVIL! 2026](https://findevil.devpost.com/) &nbsp;·&nbsp; MIT</sub>

<sub>Supporting module: [agentic-dart-collector-adapter](https://github.com/Juwon1405/agentic-dart-collector-adapter) converts Velociraptor offline-collector ZIPs into the `evidence_root` layout Agentic-DART consumes.</sub>

#### 🧭 Personal Agentic Systems &nbsp;<sub><sup>*private runtime · public showcase*</sup></sub>

Not everything I build is DFIR. I also run personal agentic systems where the same engineering idea shows up in a different domain: deterministic runtime first, database-backed evidence, LLMs as supervisors, and dashboards/Telegram as the operator surface.

<table>
<tr>
<td width="50%" valign="top">

##### [YuShin Trade Showcase](https://github.com/Juwon1405/yushin-trade-showcase)

[![YuShin Trade live dashboard](https://raw.githubusercontent.com/Juwon1405/yushin-trade-showcase/main/assets/live-dashboard.png)](https://github.com/Juwon1405/yushin-trade-showcase)

Private Bithumb KRW spot trading cockpit. The trading loop is deterministic; the LLM supervisor reviews evidence, rejected entries, market context, and policy history without becoming the runtime dependency.

<sub>→ [dashboard](https://yushin.trade) · [showcase repo](https://github.com/Juwon1405/yushin-trade-showcase)</sub>

</td>
<td width="50%" valign="top">

##### [YuShin Watch Showcase](https://github.com/Juwon1405/yushin-watch-showcase)

[![YuShin Watch live dashboard](https://raw.githubusercontent.com/Juwon1405/yushin-watch-showcase/main/assets/live-dashboard.png)](https://github.com/Juwon1405/yushin-watch-showcase)

Private luxury-watch market-intelligence monitor. It combines sold-price baselines, active listings, reference extraction, catalog context, and vision-assisted review while keeping purchase decisions human-controlled.

<sub>→ [dashboard](https://yushin.watch) · [showcase repo](https://github.com/Juwon1405/yushin-watch-showcase)</sub>

</td>
</tr>
</table>

#### 🧠 DFIR Intelligence Systems &nbsp;<sub><sup>*public archive · still useful*</sup></sub>

These repositories are archived intentionally. They show the security-intelligence building blocks behind Agentic-DART: collection, evidence normalization, analyst review, reporting, and research-backed retrieval.

<table>
<tr>
<td width="50%" valign="top">

##### 🔬 [yushin-mac-forensics-platform](https://github.com/Juwon1405/yushin-mac-forensics-platform)

<a href="https://github.com/Juwon1405/yushin-mac-forensics-platform">
<img src="https://img.shields.io/github/stars/Juwon1405/yushin-mac-forensics-platform?style=flat-square&labelColor=1c1c20&color=8b6914" alt="stars">
<img src="https://img.shields.io/github/last-commit/Juwon1405/yushin-mac-forensics-platform?style=flat-square&labelColor=1c1c20&color=5a5a60" alt="last commit">
</a>

> **macOS DFIR web platform** — ingests collector ZIPs and disk images,
> parses artifact categories, and produces searchable evidence plus PDF
> incident reports. Archived as a reference for future Agentic-DART web/reporting
> surfaces.

</td>
<td width="50%" valign="top">

##### 🍎 [yushin-mac-artifact-collector](https://github.com/Juwon1405/yushin-mac-artifact-collector)

<a href="https://github.com/Juwon1405/yushin-mac-artifact-collector">
<img src="https://img.shields.io/github/stars/Juwon1405/yushin-mac-artifact-collector?style=flat-square&labelColor=1c1c20&color=8b6914" alt="stars">
<img src="https://img.shields.io/github/last-commit/Juwon1405/yushin-mac-artifact-collector?style=flat-square&labelColor=1c1c20&color=5a5a60" alt="last commit">
</a>

> **Single-file macOS collector** — zero-dependency collection script with
> selective module execution and supply-chain IOC sweeps. Archived as a portable
> triage and collection reference.

</td>
</tr>
<tr>
<td width="50%" valign="top">

##### 🧪 [yushin-gendfir-rag](https://github.com/Juwon1405/yushin-gendfir-rag)

<a href="https://github.com/Juwon1405/yushin-gendfir-rag">
<img src="https://img.shields.io/github/stars/Juwon1405/yushin-gendfir-rag?style=flat-square&labelColor=1c1c20&color=8b6914" alt="stars">
<img src="https://img.shields.io/github/last-commit/Juwon1405/yushin-gendfir-rag?style=flat-square&labelColor=1c1c20&color=5a5a60" alt="last commit">
</a>

> **DFIR RAG replication** — unofficial Python replication of Loumachi,
> Ghanem &amp; Ferrag (2024), kept as the research artifact that preceded
> the shift from pure RAG to agentic, tool-grounded DFIR.

</td>
<td width="50%" valign="top">

##### 🔌 [agentic-dart-collector-adapter](https://github.com/Juwon1405/agentic-dart-collector-adapter)

<a href="https://github.com/Juwon1405/agentic-dart-collector-adapter">
<img src="https://img.shields.io/github/stars/Juwon1405/agentic-dart-collector-adapter?style=flat-square&labelColor=1c1c20&color=8b6914" alt="stars">
<img src="https://img.shields.io/github/last-commit/Juwon1405/agentic-dart-collector-adapter?style=flat-square&labelColor=1c1c20&color=5a5a60" alt="last commit">
</a>

> **Velociraptor to evidence_root adapter** — supporting module for
> Agentic-DART. It belongs beside the flagship project rather than above it.

</td>
</tr>
</table>

### &#9670;&nbsp; Published Work

- ***Network Attack Packet Analysis for Security Practitioners* &nbsp;·&nbsp; 보안 실무자를 위한 네트워크 공격 패킷 분석** &nbsp;<sub>(co-author, lead)</sub><br>
  Freelec, 2019.11 &nbsp;·&nbsp; ISBN 9788965402589 &nbsp;·&nbsp; ~370 pp.<br>
  A practitioner's reference covering DDoS, web exploitation, malicious traffic, wireless intrusion, system exploitation, and large-volume packet analysis.<br>
  <sub>→ [Yes24](https://www.yes24.com/Product/Goods/83538369) &nbsp;·&nbsp; [Aladin](https://www.aladin.co.kr/shop/wproduct.aspx?ItemId=217703927) &nbsp;·&nbsp; [Kyobo](https://product.kyobobook.co.kr/detail/S000001019678) &nbsp;·&nbsp; [Google Books](https://books.google.com/books?id=SIrIywEACAAJ)</sub>

### &#9670;&nbsp; Selected Recognition

- **🥇 Gold Prize**, 2017 Korea Open-Source Software Developer Contest &nbsp;<sub>(NIPA, *national OSS award*)</sub>
- **📜 Patent (filed)**: *Security Event Correlation Analysis Apparatus* &nbsp;<sub>(2018, Netmarble Corp.)</sub>
- **🎯 4th place**, 2017 CCE National Cyber Defense Competition &nbsp;<sub>(National Intelligence Service of Korea)</sub>
- **🐛 Special Prize**, 2015 LINE Bug Bounty Program &nbsp;<sub>(LINE Corp.)</sub>

### &#9670;&nbsp; Curated &amp; Community

- [**Awesome Stars** (GitNote)](https://github.com/Juwon1405/GitNote/blob/main/Resources/awesome-stars.md) ⭐ &mdash; starred repos sorted into curated buckets (DFIR / Blue Team / AI / Red Team / Malware / OSINT), regenerated after curation passes.
- Lists: [DFIR](https://github.com/stars/Juwon1405/lists/dfir) &middot; [BlueTeam](https://github.com/stars/Juwon1405/lists/blueteam) &middot; [Tools &amp; Tips](https://github.com/stars/Juwon1405/lists/tools-tips) &middot; [DevSecOps](https://github.com/stars/Juwon1405/lists/devsecops) &middot; [Gist](https://gist.github.com/Juwon1405)
- **YouTube** &mdash; [DoubleS1405](https://www.youtube.com/c/DoubleS1405), a long-running Korean-language information-security lecture channel (2014–present).

### &#9670;&nbsp; Open to

Research collaboration &middot; CTF &middot; CSIRT exchange &middot; Open-source security tooling

<br/>

<p align="center">
  <a href="https://juwon1405.github.io/"><img src="https://img.shields.io/badge/%E5%84%AA%E5%BF%83-read%20the%20full%20site%20%E2%86%92-0d0d0e?style=flat-square&labelColor=0d0d0e&color=b8311f" alt="full site"></a>
  &nbsp;
  <a href="https://github.com/Juwon1405/agentic-dart/actions/workflows/ci.yml"><img src="https://github.com/Juwon1405/agentic-dart/actions/workflows/ci.yml/badge.svg?branch=main" alt="agentic-dart CI"></a>
</p>

<p align="center"><sub><em>Juwon Bang &middot; 방주원 &middot; 優心 (YuShin)</em></sub></p>
