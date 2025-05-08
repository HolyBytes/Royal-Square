# Royal-Square - Game Catur Modern

**Dibuat oleh [Ade Pratama](https://github.com/HolyBytes)**  
✨ [Coba Sekarang](https://holybytes.github.io/Royal-Square/) | 📷 [Instagram](https://instagram.com/ryuu_adehara) | 🎵 [TikTok](https://tiktok.com/@anindya_lover12)

Game catur berbasis web dengan antarmuka sederhana tapi powerful. Cocok buat pemula sampai yang udah mahir.

## 🌟 Fitur-Fitur Super Keren
- 🔥 Tampilan Futuristik

🌗 Mode Gelap/Mode Terang (auto-save preferensi kamu)

📱 Responsif di semua device (HP, Tablet, Laptop)

🎨 4 tema papan berbeda (classic, wood, blue, green)

- 🎮 Mode Permainan Seru

🤖 VS AI (3 level kesulitan: Easy, Medium, Hard)

👥 VS Teman (2 pemain di 1 device)

🏆 Sistem statistik pemain (track record kemenanganmu)

- ⚡ Fitur Gameplay Canggih

⏱️ Timer game yang bisa disesuaikan (5-60 menit)

🔊 Efek suara realistis (gerakan, serangan, skakmat)

🔍 Highlight gerakan valid & last move

🔄 Putar papan 180° (buat yang suka perspektif berbeda)

📜 Riwayat permainan & fitur replay


## 🚧 Kekurangan & Yang Masih Aku Kembangin
- 🛠️ Dalam Proses Penyempurnaan

🌐 Mode online multiplayer (coming soon!)

📊 Analisis game pasca-permainan

🎥 Animasi gerakan bidak yang lebih smooth

🏆 Sistem leaderboard global



## 🔧 Bagian Kode yang Bisa Dimodifikasi
### 🎨 Tema dan Tampilan
```javascript
// assets/js/theme.js
const themes = {
  default: {
    lightSquare: '#f0d9b5',
    darkSquare: '#b58863'
  },
  // Tambahkan tema custom disini
  custom: {
    lightSquare: '#yourColor',
    darkSquare: '#yourColor' 
  }
}
```
**Alasan**: Warna dan tema bisa disesuaikan tanpa ganggu logika game

### 🔊 Efek Suara
```html
<!-- index.html -->
<audio id="moveSound" src="sounds/custom-move.mp3"></audio>
```
**Alasan**: Bisa diganti dengan file suara custom

### 🎚️ Tingkat Kesulitan
```javascript
// assets/js/ai.js
function setDifficulty(level) {
  // Atur kedalaman analisis AI
  if(level === 'easy') {
    this.depth = 1;
  }
  // Bisa ditambah level custom
}
```
**Alasan**: Parameter AI bisa disesuaikan

## ⚠️ Jangan Diubah Kalau Nggak Ngerti Konsekuensinya

### ♟️ Aturan Gerakan Bidak
```javascript
// assets/js/game-logic.js
function validateMove(piece, from, to) {
  // Logika validasi gerakan
  if(piece.type === 'pawn') {
    // Aturan khusus pion
  }
  // Jangan diubah kecuali paham betul aturan catur
}
```
**Alasan**: Mengubah ini bisa bikin aturan catur jadi tidak valid

### 🏗️ Struktur Dasar Papan
```html
<div id="chess-board">
  <!-- 64 squares dengan struktur spesifik -->
  <div class="row" data-row="0">...</div>
  ...
</div>
```
**Alasan**: Layout papan harus tetap 8x8 grid

### 💾 Sistem Penyimpanan
```javascript
// assets/js/storage.js
function saveGame(state) {
  // Format penyimpanan harus konsisten
  localStorage.setItem('gameState', JSON.stringify(state));
}
```
**Alasan**: Format data harus tetap sama biar kompatibel

Dampak kalau diubah sembarangan:
🛑 Game bisa error total
🛑 Fitur undo/replay nggak bakal work
🛑 Kompatibilitas versi selanjutnya bisa broken

## 🐛 Melaporkan Masalah

Ketemu bug atau punya saran?  
Buka [issue di GitHub](https://github.com/HolyBytes/Royal-Square/issues) atau DM Instagram [@ryuu_adehara](https://instagram.com/ryuu_adehara)

## 📜 Lisensi & Hak Cipta

© 2025 ADE PRATAMA - All Rights Reserved
Lisensi: https://github.com/HolyBytes

##Yang diperbolehkan:

✅ Pakai buat belajar programming
✅ Modifikasi untuk keperluan pribadi
✅ Sebarkan dengan tetap mencantumkan kredit

##Yang dilarang:

❌ Jual kembali tanpa izin
❌ Klaim sebagai karya sendiri
❌ Gunakan untuk tujuan komersial tanpa persetujuan
---

Dikembangkan dengan HTML, CSS, dan JavaScript murni.  
Ikon dari [Font Awesome](https://fontawesome.com) dan [Twemoji](https://twemoji.twitter.com).
