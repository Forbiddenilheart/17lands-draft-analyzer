# 🃏 17Lands Draft Analyzer

<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=11,2,24&height=210&section=header&text=17Lands%20Draft%20Analyzer&fontSize=48&fontColor=ffffff&animation=fadeIn&fontAlignY=36&desc=Master%20Your%20MTG%20Drafts%20with%20Data&descAlignY=56&descSize=19" width="100%"/>

<br/>

[![Version](https://img.shields.io/badge/version-4.3.0-6A4C93?style=for-the-badge&logo=semanticrelease&logoColor=white)](https://github.com)
[![Platform](https://img.shields.io/badge/Web%20%7C%20Desktop%20%7C%20CLI-8B5CF6?style=for-the-badge&logo=magic-the-gathering&logoColor=white)](https://17lands.com)
[![License](https://img.shields.io/badge/license-MIT-C4B5FD?style=for-the-badge&logo=opensourceinitiative&logoColor=black)](LICENSE)
[![Data](https://img.shields.io/badge/data-millions%20of%20drafts-A78BFA?style=for-the-badge&logo=databricks&logoColor=white)](https://17lands.com)

<br/>

### 🧠 An advanced analytics tool for Magic: The Gathering Arena draft data

*📊 Win Rates • 🎯 Pick Analysis • 🎨 Color Breakdown • 🏆 Tier Lists*

<br/>

<a href="https://share.google/BJmKgGfjlqJco89Bm">
  <img src="https://img.shields.io/badge/🚀_OPEN_ANALYZER-6A4C93?style=for-the-badge&logo=googlechrome&logoColor=white&labelColor=4F3870" alt="Open Analyzer" height="45"/>
</a>
&nbsp;&nbsp;
<a href="https://share.google/BJmKgGfjlqJco89Bm">
  <img src="https://img.shields.io/badge/📥_GET_SOURCE-8B5CF6?style=for-the-badge&logo=github&logoColor=white&labelColor=6D46C4" alt="Get Source" height="45"/>
</a>
&nbsp;&nbsp;
<a href="https://share.google/BJmKgGfjlqJco89Bm">
  <img src="https://img.shields.io/badge/📚_DOCS-C4B5FD?style=for-the-badge&logo=readthedocs&logoColor=black&labelColor=9A8BD6" alt="Docs" height="45"/>
</a>

</div>

<img width="1672" height="941" alt="b6100939-dd8f-488d-b5c9-e0de82441190" src="https://github.com/user-attachments/assets/5abf6606-7a76-4c7c-83b3-5edd07e6ee13" />


<br/>

<img src="https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png" width="100%"/>

## 🌟 About

**17Lands Draft Analyzer** is a powerful analytics dashboard built on top of the official **17Lands** dataset — the largest public collection of MTG Arena draft data. It helps you understand **which cards win games**, **how to pick better**, and **which colors perform best** in every set.

Whether you're grinding the ladder, preparing for a Pro Tour qualifier, or just curious about your favorite set, this tool turns millions of drafts into clear, actionable insights.

> 💡 **Perfect for:** MTG Arena drafters, content creators, set reviewers, and data-driven Magic players.

<img src="https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png" width="100%"/>

## 🎯 Key Features

<div align="center">

| 📊 **Win Rates** | 🎯 **Pick Analysis** | 🎨 **Color Stats** |
|:---:|:---:|:---:|
| Per-card win rate<br/>with sample sizes | GIH WR, IWD,<br/>ALSA & ATA metrics | Archetype performance<br/>across all color pairs |

| 🏆 **Tier Lists** | 🔍 **Set Comparison** | 📈 **Custom Reports** |
|:---:|:---:|:---:|
| Auto-generated<br/>per set | Compare sets<br/>side-by-side | Filter by rank,<br/>date, or player |

</div>

<img src="https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png" width="100%"/>

## 🏆 Why This Analyzer

<div align="center">

| 💎 **Advantage** | 📝 **Description** |
|:---|:---|
| 📊 **Official Data** | Uses the exact 17Lands API — no scraping, no guessing |
| 🧠 **Deep Metrics** | GIH WR, IWD, ALSA, ATA and more, explained in plain English |
| ⚡ **Fast & Snappy** | Pre-computed aggregates load in milliseconds |
| 🎨 **Beautiful UI** | Clean, readable charts that don't overwhelm |
| 🏆 **Tier Automation** | Auto-generated S/A/B/C tier lists based on real win rates |
| 🔄 **Live Updates** | New data ingested daily as 17Lands publishes fresh drafts |

</div>

<img src="https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png" width="100%"/>

## 🎬 Analyzer Preview

<div align="center">

```ascii
╔══════════════════════════════════════════════════╗
║  🃏  17Lands Draft Analyzer  v4.3.0              ║
╠══════════════════════════════════════════════════╣
║  Set: Foundations (FDN)     Format: Premier      ║
║  ──────────────────────────────────────────      ║
║  🥇 Top Cards by GIH WR                          ║
║  1. Sunblade Samurai   🎨W   GIH 61.2%   +4.1pp  ║
║  2. Gloom Sower        🎨B   GIH 59.8%   +3.2pp  ║
║  3. Flametongue Kavu   🎨R   GIH 58.4%   +2.8pp  ║
║                                                  ║
║  🎨 Color Pair Win Rates                         ║
║  WU ████████████░░  55.2%                        ║
║  BR ██████████████  56.8%                        ║
║  GW █████████████░░  56.1%                       ║
║                                                  ║
║  📈 Your last 20 drafts: avg 5.4 wins            ║
║  🔥 Best archetype: BR Sacrifice                 ║
║                                                  ║
║  📊 Drafts analyzed: 2,847,192                   ║
╚══════════════════════════════════════════════════╝
```

</div>

<img src="https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png" width="100%"/>

## 🧩 Project Structure

```
🃏 17lands-draft-analyzer/
├── 🎯 src/
│   ├── api/                   # 17Lands API client
│   │   ├── client.ts
│   │   └── cache.ts
│   ├── analytics/             # Metric computations
│   │   ├── winrate.ts
│   │   ├── colors.ts
│   │   └── tiers.ts
│   ├── dashboard/             # UI components
│   │   ├── charts/
│   │   └── tables/
│   └── exporter/              # CSV & JSON exports
├── 🎨 themes/                 # Dashboard themes
├── 🧪 tests/                  # Mock & integration tests
└── 📖 docs/                   # Metrics glossary & usage
```

<img src="https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png" width="100%"/>

## 🛠️ Tech Stack

<div align="center">

![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
![React](https://img.shields.io/badge/React-61DAFB?style=for-the-badge&logo=react&logoColor=black)
![Chart.js](https://img.shields.io/badge/Chart.js-FF6384?style=for-the-badge&logo=chartdotjs&logoColor=white)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white)
![Vite](https://img.shields.io/badge/Vite-646CFF?style=for-the-badge&logo=vite&logoColor=white)

</div>

<img src="https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png" width="100%"/>

## 🤝 Community

Found a bug? Want to add a new metric or set?

<div align="center">

<a href="https://share.google/BJmKgGfjlqJco89Bm">
  <img src="https://img.shields.io/badge/💬_Join_Discord-5865F2?style=for-the-badge&logo=discord&logoColor=white" height="35"/>
</a>
<a href="https://share.google/BJmKgGfjlqJco89Bm">
  <img src="https://img.shields.io/badge/🐞_Report_Issue-6A4C93?style=for-the-badge&logo=github&logoColor=white" height="35"/>
</a>
<a href="https://share.google/BJmKgGfjlqJco89Bm">
  <img src="https://img.shields.io/badge/⭐_Star_Repo-C4B5FD?style=for-the-badge&logo=github&logoColor=black" height="35"/>
</a>

</div>

<img src="https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png" width="100%"/>

## 📜 License

Distributed under the **MIT License**. See [`LICENSE`](LICENSE) for details.

> **Note:** Magic: The Gathering and MTG Arena are trademarks of **Wizards of the Coast**. **17Lands** is an independent community data project. This tool is **not affiliated with Wizards of the Coast, 17Lands, or Daybreak Games**.

<br/>

<div align="center">

### 🃏 Made with 📊 by the 17Lands Analyzer Team

*If this tool improved your win rate — star the repo!*

<img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=11,2,24&height=120&section=footer" width="100%"/>

</div>
