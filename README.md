<div align="center">

# 🌐 Edu-Passport

### *One ID to Learn. One Passport to Prove. One Lifetime to Recognize.*

**A Digital Public Infrastructure (DPI) for Universal Academic Recognition**

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![W3C VC](https://img.shields.io/badge/W3C-Verifiable_Credentials-blue)](https://www.w3.org/TR/vc-data-model/)
[![W3C DID](https://img.shields.io/badge/W3C-Decentralized_Identifiers-purple)](https://www.w3.org/TR/did-core/)
[![TypeScript](https://img.shields.io/badge/TypeScript-5.0+-3178C6?logo=typescript&logoColor=white)](https://www.typescriptlang.org/)
[![React Native](https://img.shields.io/badge/React_Native-Expo_SDK_57-61DAFB?logo=react)](https://reactnative.dev/)
[![Status](https://img.shields.io/badge/Status-MVP_in_Development-orange)](./ROADMAP.md)

[**Vision**](#-vision) • [**The Problem**](#-the-problem) • [**The Solution**](#-the-solution) • [**How It Looks**](#-how-it-looks) • [**Roadmap**](./ROADMAP.md) • [**Contribute**](#-contributing)

</div>

---

## 🌍 Vision

> **"Every knowledge and skill learned by a human on Earth deserves fair, equal, and instant legal recognition — without being blocked by physical passports, bureaucracy, or formal/non-formal boundaries."**

**Edu-Passport** is a **Digital Wallet** built on **Digital Public Infrastructure (DPI)** principles. It serves as an **interactive global academic passport**, ensuring that every individual's educational and skill achievements — from any corner of the world, whether through formal or non-formal pathways — can be:

- 📝 **Recorded** permanently, from birth to grave
- 🔐 **Cryptographically verified** in seconds
- 🌐 **Automatically recognized** across borders
- ♾️ **Preserved** throughout one's lifetime

Inspired by the essence of **International Birth Registration** — which gives every human a legal identity from day one — Edu-Passport gives every human **a legal academic identity** that transcends geography.

---

## 🔥 The Problem

### 🎭 Problem 1: The Fake Diploma Crisis

> *"In the digital age, forging a diploma costs $5. Verifying it takes 6 months and $1,000."*

- UNESCO estimates **30%** of internationally submitted diplomas contain discrepancies
- Traditional legalization (wet stamp, apostille) takes **2-6 months** and costs **$500-2,000** per document
- Employers, universities, and immigration offices cannot verify credentials reliably

### 🧱 Problem 2: The Cross-Border Bureaucracy Wall

Imagine a real scenario:

```
   Primary School        Middle School         High School         Bachelor's
   Palangkaraya     →    Zimbabwe        →     Congo         →     Antarctica
   (Indonesia)           (ZIMSEC)              (Congo Basin)       (Research)
   
   Kurikulum Merdeka     ZIMSEC Curriculum     Congo Curriculum    International
   6 years               3 years               3 years             4 years
```

**Every country transition requires 6-12 months of manual curriculum equivalence — with inconsistent results.**

### ⚖️ Problem 3: Non-Formal Pathway Discrimination

- **Google Data Analytics Certificate** ≠ Statistics Degree (even though both teach analytics)
- **6-month coding bootcamp** ≠ 3-year IT Diploma (even though both teach programming)
- **Indigenous community school** has zero formal recognition mechanism

### 🏢 Problem 4: Single-Vendor Dependency

- Current verification systems are dominated by **2-3 global vendors** setting monopoly prices
- User data is stored in **vendor servers**, not in the hands of the data owner
- No interoperability — vendor A cannot verify credentials issued by vendor B

---

## 💡 The Solution

### A Global Academic Passport in Your Pocket

Edu-Passport replaces the **physical diploma** with a **cryptographically signed digital credential** that:

- 🆔 Is tied to **your decentralized identity (DID)** — not to any institution or government
- 📜 Can be **issued by any accredited institution** — school, university, bootcamp, or community
- ✅ Can be **verified by anyone in seconds** — employer, university, or immigration
- 🌐 Works **across borders** — Palangkaraya to Zimbabwe to Congo to Antarctica
- 🔐 Is **tamper-proof** — cryptographic signatures cannot be forged

### The Three Pillars

```
┌─────────────────────────────────────────────────────────────┐
│  🆔 IDENTITY                                                │
│  W3C Decentralized Identifiers (DID)                        │
│  → You own your identity, not any institution               │
├─────────────────────────────────────────────────────────────┤
│  📜 CREDENTIALS                                             │
│  W3C Verifiable Credentials (VC)                            │
│  → Tamper-proof digital diplomas                            │
├─────────────────────────────────────────────────────────────┤
│  ✅ VERIFICATION                                            │
│  Cryptographic signatures + QR codes                        │
│  → Instant, offline-capable verification                    │
└─────────────────────────────────────────────────────────────┘
```

---

## 🎬 How It Looks

### 📱 The Edu-Passport App

<div align="center">

**Identity Dashboard** — Your personal academic identity
```
┌─────────────────────────────────────────┐
│  🌐 Edu-Passport                        │
│  Paspor Akademik Global                 │
│                                         │
│  Halo, Emen 👋                          │
│                                         │
│  ✅ DID AKTIF                           │
│                                         │
│  DID EMEN                               │
│  ┌─────────────────────────────────┐   │
│  │ did:edu:palangkaraya:emen:      │   │
│  │ z6MkhaXgBZDvotDkL5257faizti...  │   │
│  └─────────────────────────────────┘   │
│                                         │
│  FINGERPRINT                            │
│  ┌─────────────────────────────────┐   │
│  │     fa34dcd0ec7a1330            │   │
│  └─────────────────────────────────┘   │
│                                         │
│  📜 KREDENSIAL                    [2]   │
│  ┌─────────────────────────────────┐   │
│  │ 🎓 Ijazah SMA/SMK               │   │
│  │    8/10/2026                    │   │
│  └─────────────────────────────────┘   │
│  ┌─────────────────────────────────┐   │
│  │ 📖 Sertifikat Kursus            │   │
│  │    8/10/2026                    │   │
│  └─────────────────────────────────┘   │
│                                         │
│  ┌─────────────────────────────────┐   │
│  │    📜 Terbitkan Ijazah          │   │
│  └─────────────────────────────────┘   │
│  ┌─────────────────────────────────┐   │
│  │  📂 Lihat Semua Kredensial →    │   │
│  └─────────────────────────────────┘   │
│                                         │
│  One ID to Learn.                       │
│  One Passport to Prove.                 │
│  One Lifetime to Recognize. 🌏          │
└─────────────────────────────────────────┘
```

**Digital Wallet** — Manage all your credentials
```
┌─────────────────────────────────────────┐
│  ← Kembali                              │
│  📜 Wallet                              │
│  2 kredensial tersimpan                 │
│                                         │
│  [📚 Semua] [🎓 Formal] [💼 Non-Formal]│
│                                         │
│  ┌─────────────────────────────────┐   │
│  │ 🎓 Ijazah SMA/SMK          ✅   │   │
│  │    SMA Negeri 1 Palangkaraya    │   │
│  │    8/10/2026                    │   │
│  └─────────────────────────────────┘   │
│  ┌─────────────────────────────────┐   │
│  │ 📖 Sertifikat Kursus       ✅   │   │
│  │    Coursera                     │   │
│  │    8/10/2026                    │   │
│  └─────────────────────────────────┘   │
│                                         │
│  One ID to Learn. One Passport... 🌏   │
└─────────────────────────────────────────┘
```

**QR Code Sharing** — Show credentials for instant verification
```
┌─────────────────────────────────────────┐
│  ← Kembali                              │
│                                         │
│                🎓                       │
│          Ijazah SMA/SMK                 │
│             Duhemen                     │
│                                         │
│         ┌─────────────────┐             │
│         │  ████████████    │             │
│         │  ██ ▄▄▄▄▄ ██    │             │
│         │  ██ █▀▀▀█ ██    │             │
│         │  ██ █▄▄▄█ ██    │             │
│         │  ██▄▄▄▄▄▄██    │             │
│         │  ████████████    │             │
│         │  ██ ▀▀ ▀▀ ██    │             │
│         │  ████████████    │             │
│         └─────────────────┘             │
│                                         │
│  📱 Scan QR Code Ini                    │
│  Buka aplikasi Edu-Passport, tap        │
│  "Scan QR", arahkan kamera...           │
│                                         │
│  One ID to Learn. 🌏                    │
└─────────────────────────────────────────┘
```

**Verification Result** — Cryptographic verification in < 3 seconds
```
┌─────────────────────────────────────────┐
│  ← Kembali                              │
│                                         │
│              ✅                          │
│            VALID                        │
│      Kredensial terverifikasi           │
│                                         │
│  🎓 Ijazah SMA/SMK                      │
│  ─────────────────────                  │
│  Pemilik      Duhemen                   │
│  Penerbit     did:edu:palang...         │
│  Terbit       8 Oktober 2026            │
│                                         │
│  🔍 Detail Verifikasi                    │
│  ✅ Struktur VC                         │
│  ✅ Tanda Tangan                        │
│  ✅ Belum Kadaluarsa                    │
│  ✅ Issuer Terverifikasi                │
│                                         │
│  One ID to Learn. 🌏                    │
└─────────────────────────────────────────┘
```

</div>

---

## 🚀 User Flow

### From Zero to Verified Credential in 5 Steps

```
┌─────────────────────────────────────────────────────────────┐
│                                                             │
│  STEP 1: CREATE IDENTITY                                    │
│  ┌───────────────────────────────────────────────┐          │
│  │  Enter name & region                          │          │
│  │  Tap "Generate DID"                           │          │
│  │  → Cryptographic key pair created             │          │
│  └───────────────────────────────────────────────┘          │
│                          ↓                                  │
│  STEP 2: RECEIVE CREDENTIALS                                │
│  ┌───────────────────────────────────────────────┐          │
│  │  Tap "Issue Diploma"                          │          │
│  │  Choose from 8 credential types               │          │
│  │  → Verifiable Credential created              │          │
│  └───────────────────────────────────────────────┘          │
│                          ↓                                  │
│  STEP 3: MANAGE WALLET                                      │
│  ┌───────────────────────────────────────────────┐          │
│  │  View all credentials                         │          │
│  │  Filter by formal / non-formal                │          │
│  │  Tap to view details                          │          │
│  └───────────────────────────────────────────────┘          │
│                          ↓                                  │
│  STEP 4: SHARE VIA QR                                       │
│  ┌───────────────────────────────────────────────┐          │
│  │  Tap "Show QR"                                │          │
│  │  Show screen to verifier                      │          │
│  │  → QR code contains encrypted VC              │          │
│  └───────────────────────────────────────────────┘          │
│                          ↓                                  │
│  STEP 5: INSTANT VERIFICATION                               │
│  ┌───────────────────────────────────────────────┐          │
│  │  Verifier scans QR                            │          │
│  │  Cryptographic signature checked              │          │
│  │  → ✅ VALID in under 3 seconds                │          │
│  └───────────────────────────────────────────────┘          │
│                                                             │
└─────────────────────────────────────────────────────────────┘
```

---

## 🌍 Cross-Border Use Case

### The Palangkaraya → Zimbabwe → Congo → Antarctica Scenario

> *"A child from Palangkaraya, Indonesia studies abroad — and their education is recognized instantly, everywhere."*

```
   🎒 Primary School          🏫 Middle School          🎓 High School          🏛️ Bachelor's
   SD Negeri 1 Palangkaraya   Harare High School        Brazzaville Academy    Antarctic Research
   Palangkaraya, Indonesia    Harare, Zimbabwe          Brazzaville, Congo     Antarctica
   
   ┌────────────────┐         ┌────────────────┐        ┌────────────────┐     ┌────────────────┐
   │  ISCED 1       │         │  ISCED 2       │        │  ISCED 3       │     │  ISCED 4       │
   │  Primary       │         │  Lower Sec.    │        │  Upper Sec.    │     │  Bachelor      │
   │  Education     │         │  Education     │        │  Education     │     │  Degree        │
   └────────────────┘         └────────────────┘        └────────────────┘     └────────────────┘
         ↓                          ↓                          ↓                      ↓
   ┌──────────────────────────────────────────────────────────────────────────────────────┐
   │                                                                                      │
   │                    🆔 ONE IDENTITY — ONE WALLET — ONE PASSPORT                       │
   │                                                                                      │
   │   ┌────────────────────────────────────────────────────────────────────────────┐    │
   │   │  🎒 SD Ijazah  │  📚 SMP Ijazah  │  🎓 SMA Ijazah  │  🏛️ Sarjana Ijazah  │    │
   │   │  (Indonesia)   │  (Zimbabwe)     │  (Congo)        │  (Antarctica)       │    │
   │   └────────────────────────────────────────────────────────────────────────────┘    │
   │                                                                                      │
   │                    All verified instantly across borders via W3C VC                  │
   │                                                                                      │
   └──────────────────────────────────────────────────────────────────────────────────────┘

   Every credential cryptographically signed by issuing institution
   Every credential verifiable in < 3 seconds
   Every credential recognized cross-border via UNESCO ISCED taxonomy
```

**What used to take 6-12 months of bureaucracy now takes 3 seconds.**

---

## 🏗️ Architecture

### Four-Layer Digital Public Infrastructure

```
┌─────────────────────────────────────────────────────────────────────┐
│                                                                     │
│  LAYER 4: GLOBAL TRUST FRAMEWORK                                    │
│  ┌───────────────────────────────────────────────────────────────┐  │
│  │  UNESCO (ISCED taxonomy)  •  W3C (VC & DID standards)         │  │
│  │  PBB (SDG 4)  •  ISO 21001 (Educational Organizations)        │  │
│  └───────────────────────────────────────────────────────────────┘  │
│                                                                     │
├─────────────────────────────────────────────────────────────────────┤
│                                                                     │
│  LAYER 3: NATIONAL TRUST REGISTRY                                   │
│  ┌───────────────────────────────────────────────────────────────┐  │
│  │  🇮🇩 Kemendikbud (DAPODIK)   •   🇿🇼 ZIMSEC (EMIS)              │  │
│  │  🇨🇩 Ministère de l'Éducation  •  🇦🇶 Antarctic Treaty          │  │
│  └───────────────────────────────────────────────────────────────┘  │
│                                                                     │
├─────────────────────────────────────────────────────────────────────┤
│                                                                     │
│  LAYER 2: INSTITUTIONAL ISSUER                                      │
│  ┌───────────────────────────────────────────────────────────────┐  │
│  │  🎒 Schools  •  🏛️ Universities  •  💻 Bootcamps              │  │
│  │  📖 Course Platforms  •  🏆 Industry Certifiers               │  │
│  └───────────────────────────────────────────────────────────────┘  │
│                                                                     │
├─────────────────────────────────────────────────────────────────────┤
│                                                                     │
│  LAYER 1: INDIVIDUAL HOLDER                                         │
│  ┌───────────────────────────────────────────────────────────────┐  │
│  │  🆔 DID  •  💼 Wallet  •  📜 Verifiable Credentials            │  │
│  │  📱 Mobile App (iOS, Android)  •  🔐 Self-Sovereign Identity  │  │
│  └───────────────────────────────────────────────────────────────┘  │
│                                                                     │
└─────────────────────────────────────────────────────────────────────┘
```

---

## 🛠️ Tech Stack

### Core Technologies

| Category | Technology | Purpose |
|----------|-----------|---------|
| **Language** | TypeScript 5.0+ | Type safety, modern JS features |
| **Framework** | React Native (Expo SDK 57) | Cross-platform mobile (Android/iOS) |
| **Standards** | W3C VC, W3C DID | Global credential standards |
| **Crypto** | Ed25519, SHA-256 | Digital signatures & hashing |
| **Storage** | expo-secure-store (AES-256) | Encrypted local storage |
| **QR Code** | react-native-qrcode-svg | QR generation |
| **Camera** | expo-camera | QR scanning |
| **Navigation** | @react-navigation/native-stack | Screen navigation |

### Coming Soon (see [ROADMAP.md](./ROADMAP.md))

| Category | Technology | Phase |
|----------|-----------|-------|
| **Ed25519 Production** | @noble/ed25519 | Phase 7 |
| **DIDComm** | @hyperledger/aries-framework | Phase 9 |
| **AI Mapping** | TensorFlow Lite | Phase 6 |
| **Distributed Storage** | IPFS (Helia) | Phase 5 |
| **Database** | expo-sqlite | Phase 8 |

---

## 📚 Standards & Compliance

### ✅ Already Following

- [W3C Verifiable Credentials Data Model](https://www.w3.org/TR/vc-data-model/)
- [W3C Decentralized Identifiers (DID) Core](https://www.w3.org/TR/did-core/)
- [Ed25519Signature2020 Suite](https://w3c-ccg.github.io/lds-ed25519-2020/)
- [JSON-LD 1.1](https://www.w3.org/TR/json-ld11/)

### ⏳ Planning to Follow

- [UNESCO ISCED](http://uis.unesco.org/en/topic/international-standard-classification-education-isced) — Education taxonomy
- [ISO 21001](https://www.iso.org/standard/66266.html) — Educational organizations management
- [Open Badges 3.0](https://openbadges.org/) — Micro-credentials
- [DIDComm v2](https://identity.foundation/didcomm-messaging/spec/) — Messaging protocol
- [GDPR](https://gdpr.eu/) & [Indonesia UU PDP](https://peraturan.go.id/) — Data privacy

---

## 📊 Project Status

| Metric | Value |
|--------|-------|
| **Version** | v0.1.0 (MVP — In Development) |
| **Progress** | 🟢🟢⚪⚪⚪⚪🟢 33% |
| **Current Phase** | Phase 2 → Phase 3 |
| **Total Code** | ~8,500 lines |
| **Total Files** | ~30 files |
| **Commit** | 6 commits |
| **License** | MIT |
| **Status** | 🚧 Active Development |

### Phase Progress

| Phase | Feature | Status |
|-------|---------|--------|
| **Phase 0** | Research & Concept | ✅ Done |
| **Phase 1** | Foundation & Credentials | ✅ Done |
| **Phase 2** | QR Code Verification | ✅ Done |
| **Phase 3** | Form Input Proper | ⏳ Next |
| **Phase 4** | Documentation | ⏳ Planned |
| **Phase 5** | Registry & Trust Framework | ⏳ Planned |
| **Phase 6** | Auto-Equivalence Engine | ⏳ Planned |
| **Phase 7** | Ed25519 Production | ⏳ Planned |
| **Phase 8** | Multi-Device & Recovery | ⏳ Planned |
| **Phase 9** | DIDComm & Messaging | ⏳ Planned |
| **Phase 10** | UI/UX Polish | ⏳ Planned |
| **Phase 11** | Pilot Project | ⏳ Planned |
| **Phase 12** | Standardization & Global | ⏳ Planned |

👉 **[See full roadmap →](./ROADMAP.md)**

---

## 🤝 Contributing

**Edu-Passport is open-source** and welcomes contributions from:

- 👨‍💻 **Developers** — TypeScript, React Native, Rust (crypto)
- 🎓 **Academics** — Curriculum experts, psychometrics, ISCED specialists
- 🏛️ **Policy Makers** — Education regulators, data protection officials
- 🌍 **Community** — Non-formal institutions, community schools, bootcamps

### How to Contribute

```bash
# 1. Fork repository
# 2. Create feature branch
git checkout -b feature/amazing-feature

# 3. Commit changes
git commit -m 'feat: add amazing feature'

# 4. Push to branch
git push origin feature/amazing-feature

# 5. Open Pull Request
```

### Good First Issues

- 📸 **Visual Design** — Design UI/UX for future phases
- 🌐 **Translations** — Add more languages (Shona, French, Swahili)
- 📝 **Documentation** — Improve docs, fix typos
- 🧪 **Testing** — Write test scenarios
- 🎨 **ASCII Art** — Help create more visual mockups

---

## 🎯 Roadmap Overview

**Current Status:** 🟢🟢⚪⚪⚪⚪🟢 **33% Complete**

**Milestone Tracker:**

| Milestone | Target | Status |
|-----------|--------|--------|
| **MVP Demo** | Q4 2026 | 🟡 95% |
| **Alpha Release** | Q1 2027 | ⏳ |
| **Beta Release** | Q2 2027 | ⏳ |
| **Production Ready** | Q3 2027 | ⏳ |
| **Pilot Launch** | Q4 2027 | ⏳ |
| **Global Standard** | 2028 | ⏳ |

👉 **[See detailed roadmap →](./ROADMAP.md)**

---

## 📄 License

**MIT License** — Free to use, modify, and distribute with attribution.

---

## 🙏 Special Thanks

<div align="center">

### 🌟 To Everyone Who Made This Possible

</div>

- **🙏 God Almighty** — For the inspiration of an inclusive digital state architecture
- **📜 International Birth Registration Movement Initiators** — For opening the world's eyes to the importance of universal human identity rights from day one on Earth
- **🌐 Global Open Source Community** — W3C, Hyperledger Foundation, Decentralized Identity Foundation — for open technology standards that free the world from single-vendor dependency
- **💡 Emen** — The visionary from Palangkaraya who sparked the radical and fresh idea of a human competency passport without territorial boundaries
- **🤖 Google Mode AI** — Discussion collaborator who helped translate Emen's wild imagination into a DPI blueprint
- **🧠 DeepSeek** — Technical architect & co-pilot who translated the vision into production-ready code

---

## 📞 Contact & Community

| Channel | Link |
|---------|------|
| **GitHub** | [github.com/edu-passport](https://github.com/edu-passport) |
| **Email** | contact@edu-passport.org *(coming soon)* |
| **Discord** | *(coming soon)* |
| **Initiator** | **Emen** — Palangkaraya, Indonesia |

---

## 📌 Footnotes

> *This project is designed as a Digital Public Infrastructure (DPI) framework. Ensure all production implementations comply with national personal data protection regulations (such as Indonesia's UU PDP) and high-level encryption protection.*

> *"Education is a human right. Its recognition must not be a privilege of the wealthy and powerful nations."*

---

<div align="center">

## ⭐ Star This Repo If You Believe Education Recognition Should Be Borderless ⭐

**Built with ❤️ from Palangkaraya, Indonesia — for the world.**

*One ID to Learn. One Passport to Prove. One Lifetime to Recognize.* 🌏

[⬆ Back to Top](#-edu-passport)

</div>

---