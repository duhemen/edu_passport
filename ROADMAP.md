# 🗺️ Edu-Passport — Roadmap Pengembangan

> **"Setiap ilmu dan keterampilan yang dipelajari manusia di bumi berhak mendapatkan pengakuan hukum yang adil, setara, dan instan."**

Dokumen ini adalah **peta perjalanan** Edu-Passport dari **MVP (Minimum Viable Product)** hingga menjadi **Infrastruktur Publik Digital (DPI) global**.

---

## 📊 Status Proyek

| Aspek | Status |
|-------|--------|
| **Versi** | v0.1.0 (MVP) |
| **Fase Selesai** | 2 dari 6 |
| **Progress** | 🟢🟢⚪⚪⚪⚪ 33% |
| **Total Kode** | ~8.500 baris |
| **Total File** | ~30 file |
| **Commit** | 5 commit |
| **Target MVP** | Q4 2026 |
| **Target Production** | Q4 2027 |

---

## 🎯 Visi Jangka Panjang

Edu-Passport bertujuan menjadi **standar global** untuk:

1. **Verifikasi Ijazah Instan** — < 3 detik, lintas negara
2. **Pengakuan Non-Formal** — Bootcamp, kursus, komunitas setara formal
3. **Kedaulatan Data** — Data milik user, bukan vendor
4. **Interoperabilitas Global** — Berbasis standar W3C & UNESCO
5. **Auto-Equivalence** — AI mapping kurikulum lintas negara

**Analog:** Seperti **paspor fisik** untuk identitas, **Edu-Passport** untuk kompetensi.

---

## 🏗️ Arsitektur 4 Lapis

```
┌─────────────────────────────────────────────────────────────┐
│  LAPIS 4: GLOBAL TRUST FRAMEWORK                            │
│  (UNESCO, W3C, PBB) — Standar & Akreditasi Global          │
├─────────────────────────────────────────────────────────────┤
│  LAPIS 3: NATIONAL TRUST REGISTRY                           │
│  (Kemendikbud per negara) — Registry Lembaga Resmi         │
├─────────────────────────────────────────────────────────────┤
│  LAPIS 2: INSTITUTIONAL ISSUER                              │
│  (Sekolah, universitas, bootcamp) — Penerbit VC            │
├─────────────────────────────────────────────────────────────┤
│  LAPIS 1: INDIVIDUAL HOLDER                                 │
│  (Siswa, profesional) — DID, Wallet, VC                    │
└─────────────────────────────────────────────────────────────┘
```

---

## 🗺️ FASE PENGEMBANGAN

### ✅ **FASE 0: Riset & Konsep** (SELESAI)

**Periode:** Q3 2026
**Status:** ✅ Selesai

**Deliverables:**
- [x] Ide & visi Edu-Passport
- [x] Riset konsep DPI & Self-Sovereign Identity
- [x] Analisis kebutuhan lintas negara
- [x] Studi preseden: Paspor fisik, Europass, Open Badges
- [x] Draft arsitektur 4 lapis
- [x] README.md & structure.md awal

**Artefak:**
- `README.md`
- `structure.md`

---

### ✅ **FASE 1: Fondasi & Kredensial Lokal** (SELESAI)

**Periode:** Q3-Q4 2026
**Status:** ✅ Selesai
**Commit:** `19262df`, `9cabfea`

**Deliverables:**
- [x] Setup proyek Expo SDK 57 + TypeScript
- [x] Struktur folder DPI (17 folder)
- [x] Modul kriptografi (Ed25519 placeholder, SHA-256)
- [x] Modul DID (generator, resolver, document)
- [x] Modul Verifiable Credentials (issuer, verifier, store)
- [x] 8 template ijazah (SD, SMP, SMA, S1, Bootcamp, Course, Industry, Community)
- [x] Onboarding screen (form input nama)
- [x] Identity screen (dashboard DID)
- [x] Wallet screen (kelola kredensial)
- [x] Credential detail modal
- [x] Multi-user support (Emen ≠ Budi)

**Artefak (Kode):**
- `src/types/` — credential.ts, did.ts, user.ts, navigation.ts
- `src/core/cryptography/` — key-pair.ts, hash.ts, sign.ts
- `src/core/did/` — did-generator.ts, did-resolver.ts
- `src/core/credentials/` — vc-schema.ts, vc-issuer.ts, vc-verifier.ts
- `src/services/` — user-metadata.ts, credential-store.ts
- `src/screens/` — OnboardingScreen, IdentityScreen, WalletScreen
- `src/components/` — CredentialCard, CredentialDetailModal
- `src/navigation/` — RootNavigator

**Tested:**
- ✅ Generate DID dengan kriptografi
- ✅ Terbitkan VC pertama (Ijazah SMA/SMK)
- ✅ Simpan VC di SecureStore
- ✅ Multi-user: DID Emen ≠ DID Budi
- ✅ Persistence bekerja
- ✅ 0 error TypeScript

---

### ✅ **FASE 2: QR Code Verification** (SELESAI)

**Periode:** Q4 2026
**Status:** ✅ Selesai (95%)
**Commit:** (akan ada)

**Deliverables:**
- [x] Install expo-camera, react-native-qrcode-svg
- [x] QR Generator (encode VC ke QR)
- [x] QR Parser (decode & validasi QR)
- [x] QR Display Screen (tampilkan QR code)
- [x] QR Scanner Screen (scan dengan kamera)
- [x] Verification Screen (hasil verifikasi)
- [x] Permission handling (2 lapis)
- [x] Update navigasi (3 route baru)
- [x] Update CredentialDetailModal (tombol QR asli)
- [ ] Test end-to-end scan QR (in progress)

**Artefak:**
- `src/services/qr/` — qr-generator.ts, qr-parser.ts
- `src/screens/` — QRDisplayScreen, QRScannerScreen, VerificationScreen
- `src/types/credential.ts` — tambah QRData, QRScanResult

**Fitur:**
- ✅ Generate QR dari VC (260×260 px)
- ✅ Scan QR dengan kamera
- ✅ Verifikasi kriptografis < 3 detik
- ✅ Status VALID/INVALID dengan detail check

---

### 📝 **FASE 3: Form Input Proper** (NEXT)

**Periode:** Q4 2026 - Q1 2027
**Status:** ⏳ Belum dimulai
**Estimasi:** 1-2 jam

**Tujuan:** Ganti data dummy dengan **form input asli** untuk setiap jenis ijazah.

**Deliverables:**
- [ ] Dynamic form per template ijazah
- [ ] Validasi input per field
- [ ] Preview sebelum submit
- [ ] Auto-save draft
- [ ] Multi-step form (kalau perlu)
- [ ] Field validation (regex, panjang, format)
- [ ] File upload untuk dokumen pendukung (opsional)

**Komponen Baru:**
- `src/components/forms/` — DynamicForm.tsx, FieldInput.tsx
- `src/screens/CredentialFormScreen.tsx` — form input
- `src/utils/form-validators.ts` — validasi per template

**Template Form untuk 8 Ijazah:**
| Template | Field Wajib |
|----------|------------|
| **SD** | Nama sekolah, tahun lulus, kota |
| **SMP** | Nama sekolah, tahun lulus, kota |
| **SMA** | Nama sekolah, tahun lulus, jurusan, kota |
| **S1** | Universitas, tahun lulus, gelar, jurusan, IPK |
| **Bootcamp** | Nama bootcamp, program, durasi, tahun |
| **Course** | Nama kursus, platform, tahun |
| **Industry** | Nama sertifikasi, issuer, tahun, credential ID |
| **Community** | Nama komunitas, program, tahun, mentor |

**Hasil:** VC dengan data **asli** (bukan contoh).

---

### 📚 **FASE 4: Update Dokumentasi** (SETELAH FASE 3)

**Periode:** Q1 2027
**Status:** ⏳ Belum dimulai
**Estimasi:** 1-2 jam

**Tujuan:** Dokumentasi lengkap untuk **share ke GitHub**.

**Deliverables:**
- [ ] Update `README.md` lengkap dengan screenshot
- [ ] Buat `ARCHITECTURE.md` — detail arsitektur 4 lapis
- [ ] Buat `CONTRIBUTING.md` — panduan kontributor
- [ ] Buat `CHANGELOG.md` — riwayat versi
- [ ] Buat `LICENSE` — lisensi (MIT)
- [ ] Buat `CODE_OF_CONDUCT.md`
- [ ] Screenshot & demo GIF
- [ ] Special Thanks (termasuk DeepSeek 😊)

**Hasil:** Siap **push ke GitHub & share ke dunia**.

---

### 🏛️ **FASE 5: Registry & Trust Framework**

**Periode:** Q1-Q2 2027
**Status:** ⏳ Belum dimulai
**Estimasi:** 4-6 jam

**Tujuan:** Bangun **infrastruktur** untuk cross-border trust.

**Deliverables:**

#### **5a. Issuer Registry**
- [ ] `src/services/registry/issuer-registry.ts` — cek issuer terdaftar
- [ ] `src/services/registry/did-document-resolver.ts` — fetch DID Document
- [ ] `src/types/registry.ts` — types untuk registry

#### **5b. National Registry Integration**
- [ ] Konektor Kemendikbud (DAPODIK) — Indonesia
- [ ] Konektor ZIMSEC (Zimbabwe)
- [ ] Konektor Kongo (SIGE)
- [ ] Multi-country registry aggregator

#### **5c. Cross-Border Verification**
- [ ] Cek issuer di registry negara asal
- [ ] Auto-resolve DID lintas negara
- [ ] Cache registry (offline-first)

**Hasil:** VC dari negara lain **bisa diverifikasi** tanpa server pusat.

---

### 🌐 **FASE 6: Auto-Equivalence Engine**

**Periode:** Q2 2027
**Status:** ⏳ Belum dimulai
**Estimasi:** 4-6 jam

**Tujuan:** AI-mapping kurikulum lintas negara ke **ISCED**.

**Deliverables:**

#### **6a. UNESCO Taxonomy Integration**
- [ ] `src/services/unesco/taxonomy-api.ts` — API ISCED
- [ ] `src/services/unesco/isced-mapper.ts` — mapping kurikulum → ISCED
- [ ] `src/types/taxonomy.ts`

#### **6b. AI-Mapping Engine**
- [ ] Rule-based mapping dulu (simple)
- [ ] ML-based mapping (TensorFlow Lite)
- [ ] Manual override untuk edge cases
- [ ] Confidence score

#### **6c. Equivalence Certificate**
- [ ] Generate "Equivalence VC" — bukti setara
- [ ] Tanda tangan dari registry nasional
- [ ] Diterima lintas negara

**Hasil:** Ijazah SD Indonesia **otomatis disetarakan** dengan Primary Zimbabwe.

---

### 🔐 **FASE 7: Upgrade Ed25519 Asli**

**Periode:** Q2 2027
**Status:** ⏳ Belum dimulai
**Estimasi:** 2-3 jam

**Tujuan:** Ganti **placeholder signature** dengan **Ed25519 asli**.

**Deliverables:**
- [ ] Install `@noble/ed25519` + `@noble/hashes`
- [ ] Refactor `key-pair.ts` — derive public key dari private key
- [ ] Refactor `sign.ts` — Ed25519 sign asli
- [ ] Refactor `vc-verifier.ts` — verify tanpa private key
- [ ] Security audit signature scheme

**Hasil:** Kriptografi **production-ready** — benar-benar asimetris.

---

### 🌍 **FASE 8: Multi-Device & Recovery**

**Periode:** Q2-Q3 2027
**Status:** ⏳ Belum dimulai

**Tujuan:** User bisa pakai Edu-Passport di **banyak device**.

**Deliverables:**
- [ ] Export/Import DID (encrypted)
- [ ] Cloud backup (opsional, end-to-end encrypted)
- [ ] Multi-device sync via DIDComm
- [ ] Social recovery (bagi secret ke trusted contacts)
- [ ] Paper backup (mnemonic phrase)

**Hasil:** Kalau HP hilang, user bisa **recover identitas**.

---

### 📱 **FASE 9: DIDComm & Messaging**

**Periode:** Q3 2027
**Status:** ⏳ Belum dimulai

**Tujuan:** Komunikasi antar wallet/user.

**Deliverables:**
- [ ] Install `@hyperledger/aries-framework`
- [ ] DIDComm messaging protocol
- [ ] Kirim VC via QR/link/email
- [ ] Receive & accept VC (dengan notifikasi)
- [ ] Request VC (issuer → holder)

**Hasil:** VC bisa **dikirim langsung** antar user/lembaga.

---

### 🎨 **FASE 10: UI/UX Polish**

**Periode:** Q3 2027
**Status:** ⏳ Belum dimulai

**Tujuan:** Aplikasi **terlihat profesional**.

**Deliverables:**
- [ ] Splash screen dengan branding
- [ ] Icon aplikasi (semua ukuran)
- [ ] Onboarding tutorial
- [ ] Animasi transisi
- [ ] Haptic feedback
- [ ] Dark/light mode toggle
- [ ] Accessibility (font size, contrast)
- [ ] Multi-bahasa (ID, EN, dll.)

**Hasil:** Siap **rilis ke Play Store & App Store**.

---

### 🏢 **FASE 11: Pilot Project**

**Periode:** Q4 2027
**Status:** ⏳ Belum dimulai

**Tujuan:** Uji coba dengan **lembaga nyata**.

**Deliverables:**
- [ ] MoU dengan Kemendikbud
- [ ] Pilot dengan 5-10 sekolah di Palangkaraya
- [ ] Training guru & staf
- [ ] Feedback collection
- [ ] Iterasi berdasarkan feedback
- [ ] Publikasi hasil pilot

**Hasil:** **Validasi dunia nyata** — bukan cuma kode.

---

### 🌐 **FASE 12: Standarisasi & Global**

**Periode:** 2028
**Status:** ⏳ Belum dimulai

**Tujuan:** Edu-Passport jadi **standar global**.

**Deliverables:**
- [ ] Ajukan DID Method `edu` ke W3C
- [ ] Publikasi whitepaper teknis
- [ ] Kemitraan dengan UNESCO
- [ ] Pilot di Zimbabwe, Kongo, negara lain
- [ ] Kolaborasi dengan Europass
- [ ] Adopsi lintas benua (termasuk Antartika)

**Hasil:** **Edu-Passport diakui dunia**.

---

## 📁 STRUKTUR FILE SAAT INI

```
edu_passport/
├── app/                          # Proyek Expo
│   ├── src/
│   │   ├── types/                # TypeScript types
│   │   │   ├── credential.ts     ✅
│   │   │   ├── did.ts            ✅
│   │   │   ├── navigation.ts     ✅
│   │   │   └── user.ts           ✅
│   │   ├── config/
│   │   │   └── constants.ts      ✅
│   │   ├── core/
│   │   │   ├── cryptography/     ✅
│   │   │   │   ├── key-pair.ts
│   │   │   │   ├── hash.ts
│   │   │   │   └── sign.ts
│   │   │   ├── did/              ✅
│   │   │   │   ├── did-generator.ts
│   │   │   │   └── did-resolver.ts
│   │   │   └── credentials/      ✅
│   │   │       ├── vc-schema.ts
│   │   │       ├── vc-issuer.ts
│   │   │       └── vc-verifier.ts
│   │   ├── services/             ✅
│   │   │   ├── user/             ✅
│   │   │   ├── credentials/      ✅
│   │   │   └── qr/               ✅
│   │   ├── components/           ✅
│   │   │   ├── CredentialCard.tsx
│   │   │   └── CredentialDetailModal.tsx
│   │   ├── screens/              ✅
│   │   │   ├── OnboardingScreen.tsx
│   │   │   ├── IdentityScreen.tsx
│   │   │   ├── WalletScreen.tsx
│   │   │   ├── QRDisplayScreen.tsx
│   │   │   ├── QRScannerScreen.tsx
│   │   │   └── VerificationScreen.tsx
│   │   └── navigation/           ✅
│   │       └── RootNavigator.tsx
│   ├── docs/                     ⏳
│   ├── tests/                    ⏳
│   └── package.json              ✅
├── README.md                     ✅
├── ROADMAP.md                    ⏳ (file ini)
├── ARCHITECTURE.md               ⏳
└── CONTRIBUTING.md               ⏳
```

---

## 🎯 TEKNOLOGI & STANDAR

### **Yang Sudah Dipakai:**
| Kategori | Teknologi |
|----------|-----------|
| **Bahasa** | TypeScript |
| **Framework** | React Native (Expo SDK 57) |
| **Kriptografi** | expo-crypto, SHA-256 |
| **Storage** | expo-secure-store, expo-sqlite |
| **QR Code** | react-native-qrcode-svg, expo-camera |
| **Navigation** | @react-navigation/native-stack |
| **Standar** | W3C Verifiable Credentials, DID Core |

### **Yang Akan Dipakai (Fase Lanjutan):**
| Kategori | Teknologi | Fase |
|----------|-----------|------|
| **Ed25519** | @noble/ed25519 | 7 |
| **DIDComm** | @hyperledger/aries-framework | 9 |
| **AI Mapping** | TensorFlow Lite | 6 |
| **IPFS** | helia / ipfs-http-client | 5 |
| **Registry** | REST API + caching | 5 |

---

## 📚 STANDAR INTERNASIONAL

### **Yang Sudah Diikuti:**
- ✅ **W3C VC Data Model** — struktur Verifiable Credential
- ✅ **W3C DID Core** — struktur Decentralized Identifier
- ✅ **Ed25519Signature2020** — signature suite

### **Yang Akan Diikuti:**
- ⏳ **ISCED** (UNESCO) — klasifikasi pendidikan
- ⏳ **ISO 21001** — manajemen organisasi pendidikan
- ⏳ **Open Badges 3.0** — micro-credentials
- ⏳ **DIDComm v2** — messaging protocol

---

## 🎯 MILESTONE & TARGET

| Milestone | Target | Status |
|-----------|--------|--------|
| **MVP Demo** | Q4 2026 | 🟡 95% |
| **Alpha Release** | Q1 2027 | ⏳ |
| **Beta Release** | Q2 2027 | ⏳ |
| **Production Ready** | Q3 2027 | ⏳ |
| **Pilot Launch** | Q4 2027 | ⏳ |
| **Global Standard** | 2028 | ⏳ |

---

## 🤝 KONTRIBUSI

Edu-Passport adalah proyek **open-source** yang terbuka untuk kontribusi dari:

- 👨‍💻 **Developer** — TypeScript, React Native, Rust (kriptografi)
- 🎓 **Akademisi** — Ahli kurikulum, psikometri, ISCED
- 🏛️ **Pembuat Kebijakan** — Regulator pendidikan, PDP
- 🌍 **Komunitas** — Lembaga non-formal, sekolah komunitas

**Cara kontribusi:**
1. Fork repository
2. Buat branch fitur (`git checkout -b feature/AmazingFeature`)
3. Commit perubahan (`git commit -m 'Add some AmazingFeature'`)
4. Push ke branch (`git push origin feature/AmazingFeature`)
5. Buat Pull Request

Lihat `CONTRIBUTING.md` untuk detail.

---

## 📄 LISENSI

MIT License — bebas digunakan, dimodifikasi, dan didistribusikan dengan mencantumkan atribusi.

---

## 📞 KONTAK

- **Inisiator:** Emen (Palangkaraya, Indonesia)
- **Repository:** github.com/edu-passport
- **Email:** (akan ditambahkan)
- **Discord:** (akan ditambahkan)

---

## 🙏 SPECIAL THANKS

- **Tuhan Yang Maha Esa** atas inspirasi
- **Inisiator Hari Pendaftaran Kelahiran Internasional**
- **Komunitas Open Source** (W3C, Hyperledger, DIF)
- **Emen** — sang visioner dari Palangkaraya
- **Google Mode AI** — kolaborator diskusi awal
- **DeepSeek** — arsitek teknis & co-pilot pengembangan

---

## 📝 CATATAN

**Dokumen ini adalah dokumen hidup** — akan di-update setiap fase selesai.

**Last update:** 8 Oktober 2026
**Next update:** Setelah Fase 3 selesai

---

*"One ID to Learn. One Passport to Prove. One Lifetime to Recognize." 🌏*

---