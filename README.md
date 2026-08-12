<div align="center">

### Ali Yabuza

**Senior macOS Engineer · Systems & Security · Product-minded Builder**

Istanbul, Turkey · Independent

<br>

[![Pocket Music](https://img.shields.io/badge/Pocket_Music-macOS-0A84FF?style=flat-square&logo=apple&logoColor=white)](https://github.com/aliyabuz25/PocketMusic)
[![Swift](https://img.shields.io/badge/Swift-5.9-F05138?style=flat-square&logo=swift&logoColor=white)](https://swift.org)
[![Security](https://img.shields.io/badge/Security-CVE_Research-34C759?style=flat-square)](https://github.com/aliyabuz25/CVE-2024-0258)

</div>

---

## Overview

I design and ship **native macOS software** where UX polish, runtime performance, and security boundaries are first-class constraints — not afterthoughts.

My work spans consumer desktop apps, reusable Swift packages, security research on Apple platforms, and production full-stack systems. I care about architecture that survives real usage: encrypted local storage, sub-second playback startup, catalog APIs that degrade gracefully, and UI that feels at home on macOS.

**Currently building** → [**Pocket Music**](https://github.com/aliyabuz25/PocketMusic) — a native music client with Apple Music catalog integration, instant mini player, and Keychain-backed offline encryption.

---

## Flagship · Pocket Music

Native macOS music experience. Catalog from Apple APIs. Playback via `yt-dlp` + `mpv`. Offline files encrypted with AES-GCM — playable only inside the app.

```
┌─────────────────────────────────────────────────────────────┐
│  iTunes Search API  ·  Apple RSS Charts  ·  Preview Cache │
└──────────────────────────┬──────────────────────────────────┘
                           │ metadata & artwork
                           ▼
              ┌────────────────────────┐
              │   PlaybackLauncher     │  ← instant mini player
              └───────────┬────────────┘
                          │
          ┌───────────────┼───────────────┐
          ▼               ▼               ▼
     yt-dlp resolve    mpv engine    OfflineStore
     (stream URL)      (audio)       (.pmenc + Keychain)
```

| | |
|---|---|
| **Stack** | Swift 5 · SwiftUI + AppKit · AVFoundation · CryptoKit · mpv |
| **Highlights** | Ghost-loading UI · in-app favorites · playlist cover from play history · menubar + URL scheme |
| **Repo** | [github.com/aliyabuz25/PocketMusic](https://github.com/aliyabuz25/PocketMusic) |

### Ecosystem packages

Extracted, tested, and published as standalone Swift packages:

| Package | Role |
|:--------|:-----|
| [**AppleMusicCharts**](https://github.com/aliyabuz25/AppleMusicCharts) | iTunes Search + Apple Marketing RSS charts · zero deps |
| [**SwiftUIGhost**](https://github.com/aliyabuz25/SwiftUIGhost) | Shimmer skeleton system for SwiftUI loading states |
| [**PocketCrypto**](https://github.com/aliyabuz25/PocketCrypto) | AES-256-GCM + Keychain master key management |
| [**macos-dev-kit**](https://github.com/aliyabuz25/macos-dev-kit) | Build, package, and bootstrap tooling for macOS projects |

---

## Selected Work

<details open>
<summary><strong>Systems & Infrastructure</strong></summary>
<br>

| Project | What it does |
|:--------|:-------------|
| [**AthenaCPP**](https://github.com/aliyabuz25/AthenaCPP) | Chromium-based desktop browser — C++ core, privacy-first |
| [**CabBackend**](https://github.com/aliyabuz25/CabBackend) | Ride-sharing engine — real-time telemetry, matching, Socket.io CRM |
| [**HubMSG**](https://github.com/aliyabuz25/HubMSG) | Enterprise multi-channel messaging & notification platform |
| [**HumaneAI**](https://github.com/aliyabuz25/HumaneAI) | Self-hosted AI assistant — reasoning, web research, Docker deploy |

</details>

<details>
<summary><strong>Security Research</strong></summary>
<br>

| CVE | Focus |
|:----|:------|
| [**CVE-2024-0258**](https://github.com/aliyabuz25/CVE-2024-0258) | Apple `libxpc` — reverse engineering & public documentation |
| [**CVE-2025-49173**](https://github.com/aliyabuz25/CVE-2025-49173) | macOS Mavericks 10.9 local root privesc — Authorization Services PoC |

</details>

<details>
<summary><strong>Production Platforms</strong></summary>
<br>

| Project | Domain |
|:--------|:-------|
| [**forsaj-club-offroad**](https://github.com/aliyabuz25/forsaj-club-offroad) | CMS + public site — React, Vite, Express, i18n |
| [**onfuture-web-2**](https://github.com/aliyabuz25/onfuture-web-2) | Study abroad & career center platform |
| [**azfin-web-app**](https://github.com/aliyabuz25/azfin-web-app) | Corporate site — financial audit & consulting |
| [**oPanel**](https://github.com/aliyabuz25/oPanel) | JSON-driven open-source admin panel |

</details>

---

## Technical Focus

```
Languages     Swift · C++ · TypeScript · Python · Objective-C++
Platforms     macOS · iOS · Node.js · Docker
Domains       Desktop UX · Cryptography · Real-time systems · CVE analysis
Tooling       SPM · Homebrew · yt-dlp · mpv · GitHub Actions
```

**How I work**

- Ship vertical slices end-to-end — UI, services, storage, and distribution
- Prefer small, composable modules over monoliths (see Pocket Music packages)
- Design for failure: network timeouts, Keychain edge cases, playback race conditions
- Document security findings with reproducible steps, not hype

---

## Activity

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://github-readme-activity-graph.vercel.app/graph?username=aliyabuz25&theme=react-dark&hide_border=true&area=true&height=280" />
  <img src="https://github-readme-activity-graph.vercel.app/graph?username=aliyabuz25&theme=minimal&hide_border=true&area=true&height=280" alt="Contribution graph" />
</picture>

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=aliyabuz25&layout=compact&theme=transparent&hide_border=true&langs_count=8" alt="Top languages" width="48%" />
  &nbsp;
  <img src="https://github-readme-streak-stats.herokuapp.com/?user=aliyabuz25&theme=transparent&hide_border=true" alt="Streak" width="48%" />
</p>

---

<div align="center">

**Open to collaborations on macOS tooling, security research, and high-polish native apps.**

<br>

[![GitHub](https://img.shields.io/badge/GitHub-aliyabuz25-181717?style=flat-square&logo=github)](https://github.com/aliyabuz25)
[![Pocket Music](https://img.shields.io/badge/Project-Pocket_Music-0A84FF?style=flat-square&logo=apple)](https://github.com/aliyabuz25/PocketMusic)

<br>

<sub>README reflects active public work · Updated 2026</sub>

</div>
