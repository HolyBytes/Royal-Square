# Royal-Square - Game Catur Modern
**Dibuat oleh [Ade Pratama](https://github.com/HolyBytes)**  
✨ [Coba Sekarang](https://holybytes.github.io/Royal-Square/) | 📷 [Instagram](https://instagram.com/ryuu_adehara) | 🎵 [TikTok](https://tiktok.com/@anindya_lover12)

> *"Bidak putih atau hitam pilihan,*  
> *Strategi catur ujian pikiran,*  
> *Royal-Square hadir dengan keindahan,*  
> *Permainan klasik dengan sentuhan kekinian."*

Halo! Ini game catur berbasis web dengan tampilan simpel tapi keren banget. Cocok buat kamu yang baru belajar sampai yang udah jago main catur.

## 🌟 Fitur-Fitur Kece

### 🔥 Tampilan Kekinian
- 🌗 Mode Gelap/Terang (otomatis nyimpen pilihan kamu)
- 📱 Enak dipake di semua device (HP, Tablet, Laptop)
- 🎨 Ada 4 tema papan beda (klasik, kayu, biru, hijau)

### 🎮 Mode Main yang Seru
- 🤖 Lawan AI (ada 3 level: Gampang, Sedang, Susah)
- 👥 Main bareng temen (bisa 2 orang di 1 device)
- 🏆 Ada catatan statistik (biar tau seberapa jago kamu)

### ⚡ Fitur Game yang Keren
- ⏱️ Timer yang bisa diatur sendiri (5-60 menit)
- 🔊 Suara-suara yang bikin serasa main beneran
- 🔍 Ada highlight gerakan valid & langkah terakhir
- 🔄 Bisa putar papan 180° (buat lihat dari sudut lawan)
- 📜 Riwayat permainan & bisa nonton ulang

> *"Raja melangkah satu-satu,*  
> *Kuda melompat bentuk L selalu,*  
> *Royal-Square temani harimu,*  
> *Asah otak sambil ngadem di AC atau di bawah pohon jambu."*

## 🚧 Yang Masih Dibenerin

- 🌐 Mode main online (sebentar lagi ada!)
- 📊 Analisis gerakan setelah main
- 🎥 Animasi bidak yang lebih halus
- 🏆 Peringkat pemain global

## 🔧 Bagian Kode yang Bisa Diutak-atik

### 🎨 Tema dan Tampilan
```javascript
// assets/js/theme.js
const themes = {
  default: {
    lightSquare: '#f0d9b5',
    darkSquare: '#b58863'
  },
  // Mau bikin tema sendiri? Tambahin di sini
  custom: {
    lightSquare: '#warnaPilihanmu',
    darkSquare: '#warnaPilihanmu' 
  }
}
```
**Kenapa boleh diubah**: Ganti warna sesuka hati tanpa ngerusak game-nya

### 🔊 Efek Suara
```html
<!-- index.html -->
<audio id="moveSound" src="sounds/custom-move.mp3"></audio>
```
**Kenapa boleh diubah**: Mau suara yang lebih asik? Ganti aja filenya

### 🎚️ Level Kesulitan
```javascript
// assets/js/ai.js
function setDifficulty(level) {
  // Atur seberapa pinter AI-nya
  if(level === 'easy') {
    this.depth = 1;
  }
  // Mau bikin level custom? Bisa ditambahin di sini
}
```
**Kenapa boleh diubah**: Biar bisa diatur sendiri gimana AI-nya main

## ⚠️ Jangan Diotak-atik Kalau Nggak Ngerti

### ♟️ Aturan Gerakan Bidak
```javascript
// assets/js/game-logic.js
function validateMove(piece, from, to) {
  // Logika cek gerakan
  if(piece.type === 'pawn') {
    // Aturan khusus pion
  }
  // Awas, jangan diubah kalo gak paham aturan catur!
}
```
**Kenapa jangan diubah**: Bisa bikin aturan catur jadi kacau

### 🏗️ Struktur Papan
```html
<div id="chess-board">
  <!-- 64 kotak dengan struktur tertentu -->
  <div class="row" data-row="0">...</div>
  ...
</div>
```
**Kenapa jangan diubah**: Papan catur emang harus 8x8, kalo diubah malah aneh

### 💾 Sistem Penyimpanan
```javascript
// assets/js/storage.js
function saveGame(state) {
  // Format nyimpen data harus tetep sama
  localStorage.setItem('gameState', JSON.stringify(state));
}
```
**Kenapa jangan diubah**: Biar data tersimpan dengan benar

Kalo nekat diubah:
🛑 Game bakal rusak/error
🛑 Fitur undo/replay bakal ngaco
🛑 Update versi berikutnya bisa jadi gak nyambung

## 🐛 Mau Lapor Bug?

Nemu masalah atau punya ide keren?  
Langsung aja [buka issue di GitHub](https://github.com/HolyBytes/Royal-Square/issues) atau DM Instagram [@ryuu_adehara](https://instagram.com/ryuu_adehara)

## 📜 Lisensi & Hak Cipta

© 2025 ADE PRATAMA - All Rights Reserved
Lisensi: https://github.com/HolyBytes

### Yang boleh kamu lakukan:
✅ Pake buat belajar coding
✅ Modifikasi buat keperluan sendiri
✅ Bagikan ke orang lain (jangan lupa kredit ya!)

### Yang gak boleh kamu lakukan:
❌ Jual tanpa izin dari pembuat
❌ Ngaku-ngaku ini buatan kamu
❌ Pake buat bisnis tanpa bilang-bilang dulu

---

> *"Skak mat akhiri permainan,*  
> *Royal-Square bawa pengalaman,*  
> *Di dunia digital penuh kebahagiaan,*  
> *Main catur jadi lebih menyenangkan."*

## ✨ Selamat Mencoba!

Yuk cobain Royal-Square sekarang dan rasain serunya main catur versi digital! Siapa tau kamu bisa jadi GM (Grand Master) berikutnya dari Indonesia! Semoga game ini bisa nemenin waktu senggang kamu dan bikin hidup lebih seru!

## 🙏 Maaf Kalau Masih Ada Kekurangan

Mohon maaf kalau Royal-Square masih jauh dari sempurna. Sebagai project yang masih terus berkembang, pasti masih banyak kurangnya di sana-sini. Feedback kamu sangat berharga buat bikin game ini jadi lebih oke lagi. Makasih udah mau nyobain dan support project ini!

Dibuat pake HTML, CSS, dan JavaScript murni.  
Ikon-ikon dari [Font Awesome](https://fontawesome.com) dan [Twemoji](https://twemoji.twitter.com).
