# 💐 Cesa Botz - WhatsApp Multifungsi Bot

**Cesa Botz** adalah bot WhatsApp modular berbasis [Baileys](https://github.com/WhiskeySockets/Baileys), dengan fitur lengkap mulai dari AI, game, tools, downloader, sistem XP, anti-spam, hingga jadwal sholat & info gempa.

---

## 🗃️ Tentang Database
Bot ini menggunakan SQLite (cesa_bot.db) sebagai sistem penyimpanan utama.
Berbeda dengan penyimpanan berbasis JSON, SQLite menawarkan:

1. ✅ Query lebih cepat dan efisien
2. ✅ Mendukung relasi antar data (multiple tabel)
3. ✅ Aman dari konflik tulis/baca di saat bersamaan
4. ✅ Skala data lebih besar & stabil untuk bot aktif
5. ✅ Dukungan indexing, constraint, dan migrasi otomatis
- Ini menjadikan bot lebih stabil dan tangguh, terutama jika digunakan dalam banyak grup sekaligus.

## 📦 Fitur Utama

- 🤖 **AI Multi-engine**: Gemini, OpenAI, Bard, Copilot, Blackbox  
- 👥 **Manajemen Grup**: Anti-link, anti-kata kasar, auto welcome/goodbye, kick berdasarkan sticker  
- 🕹️ **Game Interaktif**: Tebak gambar, kata, lirik, kuis  
- 📊 **Sistem XP dan CesaCoin**: Reward + leveling otomatis  
- 📆 **Absensi Otomatis**: Sesi harian dengan auto-kick bagi yang tidak hadir  
- 🕌 **Jadwal Sholat + Adzan**: Notifikasi otomatis  
- 🚨 **Info Gempa BMKG**: Deteksi dan broadcast otomatis ke grup  
- 📤 **Menfess & Broadcast**: Anonim dan terjadwal  
- ⚙️ **Sistem Plugin Modular**: Auto load, reload, dan plugin handler  
- 🔐 **Owner Commands Lengkap**: Eval JS, Shell, DB, plugin manager  
- 🎨 **Sticker Maker & WebP Tools**: Dengan dukungan metadata (packname/author)  

---

## 🗃️ Struktur Direktori
```bash
index.js
settings.js
package.json

Data/
├── setbot.json
├── cesa_bot.db
└── game/

Control/
├── Function.js
├── Config.js
├── menuData.js
├── command-handler.js
├── database.js
└── webp.js

Plugins/
├── ai/
├── download/
├── game/
├── group/
├── islami/
├── main/
├── maker/
├── owner/
├── stalker/
└── tools/

logs/
└── bot.log, error.log (auto generated)
```

---

## 🚀 Cara Menjalankan Bot

### 1. Clone Repository
```bash
git clone https://github.com/
cd cesa-botz
```
2. Install Dependensi
```bash

npm install
```
3. Jalankan Bot
```bash

npm start
```
# ⚙️ Konfigurasi Bot (settings.js)

## Edit langsung file settings.js untuk mengatur:

1. Nomor owner
2. Nama bot
3. API key eksternal
4. Pairing code
5. Channel info
6. Link server pribadi

# 📑 Menu Utama (Kategori)
- .menu ai – Gemini, OpenAI, Bard, Blackbox, Copilot
- .menu game – Tebakan dan kuis
- .menu group – Kick, welcome, antibadword
- .menu maker – Sticker, TTP, OCR, Remini, dsb
- .menu tools – KBBI, TTS, cuaca, topdf, morse, URL shortener
- .menu islami – Kisah Nabi, wirid, tahlil, jadwal sholat
- .menu download – YouTube, TikTok, IG, Twitter, Capcut, GDrive
- .menu stalker – Dana, ShopeePay, Gopay, NIM kampus, dsb
- .menu owner – Eval, shell, plugin, db, reload, setpp, dsb

## 🔐 Khusus Owner

Beberapa perintah penting:

- `> kode` — Eval sinkron  
- `=> kode` — Eval async  
- `$ perintah` — Jalankan shell command  

### 🔌 Plugin Management
- `.splugin` — Simpan plugin baru  
- `.uplugin` — Update plugin  
- `.gplugin` — unduh plugin  
- `.rplugin` — menampilkan isi plugin  
- `.dplugin` — Hapus plugin tertentu  

### 📦 Database & Status
- `.getdb` — Unduh database  
- `.updatedb` — update databases (reply file .db)  
- `.bot on/off` — Aktif/nonaktif bot global  
- `.botgc on/off` — Aktif/nonaktif bot di grup  


# 🤝 Partner & Support
Berikut pihak/entitas yang mendukung pengembangan Cesa Botz:
1. 🌐 BetaBotz API – Penyedia API AI dan Sholat
2. 🤖 Nata API – AI Gemini / Blackbox chat
3. 🛠️ Mhcode Server – Server upload media & file
4. 👨 Alvin – donatur server


# 📞 Kontak Developer
- Nama: Mhcode
- Owner: 6281703660784
- Website: https://mhcode.web.id
- WhatsApp Channel: https://whatsapp.com/channel/0029Vb61JRDBfxnxirTkpu2X
# 📄 Lisensi
Proyek ini menggunakan lisensi MIT. Silakan digunakan, dimodifikasi, dan dikembangkan dengan mencantumkan kredit.
