# 🚀 OVO CLI - Command Line Interface untuk OVO

[![PHP Version](https://img.shields.io/badge/PHP-7.4%2B-blue.svg)](https://www.php.net/)
[![License](https://img.shields.io/badge/License-Proprietary-red.svg)](LICENSE)
[![Platform](https://img.shields.io/badge/Platform-Windows%20%7C%20Linux%20%7C%20macOS-lightgrey.svg)](https://www.php.net/downloads.php)
[![Telegram](https://img.shields.io/badge/Telegram-@mangetaaa-blue.svg)](https://t.me/mangetaaa)

Sistem Command Line Interface (CLI) untuk mengelola akun OVO dengan fitur lengkap transfer, pembayaran QRIS, dan manajemen multi-akun. Dibuat dengan keamanan enterprise-grade dan enkripsi multi-layer.

---

## 📋 Daftar Isi

- [Fitur Utama](#-fitur-utama)
- [Persyaratan Sistem](#-persyaratan-sistem)
- [Instalasi](#-instalasi)
- [Penggunaan](#-penggunaan)
- [Fitur Detail](#-fitur-detail)
- [Keamanan](#-keamanan)
- [Troubleshooting](#-troubleshooting)
- [Kontak](#-kontak)

---

## ✨ Fitur Utama

### 🔐 Keamanan & Lisensi
- **Sistem Lisensi Terkontrol** - Akses OVO CLI dengan kode aktivasi
- **Validasi Real-Time** - Perlindungan akses tidak sah
- **Proteksi Data** - Storage dan transfer data aman

### 💼 Manajemen Akun
- **Multi-Akun** - Kelola banyak akun OVO dalam satu CLI
- **Ganti Akun Cepat** - Switch antar akun dengan satu perintah
- **Sinkronisasi Otomatis** - Auto-update saldo OVO Cash dan Points
- **Session Encrypted** - Simpan session dengan enkripsi lokal
- **Hapus Akun** - Fitur penghapusan akun yang aman

### 💸 Fitur Transfer & Pembayaran
- **Transfer OVO ke OVO** - Kirim uang antar pengguna OVO secara cepat
- **Transfer Bank** - Kirim ke 100+ bank Indonesia dengan verifikasi nama
- **Pembayaran QRIS** - Scan dan bayar kode QR secara instan
- **Simpan QRIS Favorit** - Simpan merchant favorit untuk akses cepat
- **Riwayat Transaksi** - Lihat 10 transaksi terakhir dengan detail lengkap

### 🎨 User Interface
- **Interface Modern** - CLI yang colorful dan user-friendly
- **Loading Bar Animasi** - Progress bar untuk setiap operasi
- **Validasi Smart** - Error handling dengan pesan yang jelas
- **Format Rupiah** - Tampilan saldo dalam format Indonesia
- **Bahasa Indonesia** - Interface penuh berbahasa Indonesia

### ⏱️ Jeda Transfer (Anti-Spam)
- **Konfigurasi Delay** - Atur jeda antar transaksi per tipe
- **Countdown Real-Time** - Tampilkan sisa waktu tunggu otomatis
- **Per Tipe Transaksi** - Jeda terpisah untuk OVO, Bank, dan QRIS
- **Auto-Process** - Transaksi otomatis diproses setelah countdown
- **Fleksibel** - Bisa dinonaktifkan atau diubah kapan saja

---

## 💻 Persyaratan Sistem

### Sistem Operasi
- ✅ **Windows** 10/11
- ✅ **Linux** (Ubuntu, Debian, CentOS, dll)
- ✅ **macOS** 10.15+
- ✅ **Android** (via Termux)

### PHP
- **PHP** versi 7.4 atau lebih tinggi

### Koneksi Internet
- Koneksi internet stabil diperlukan
- Port 443 (HTTPS) harus terbuka

---

## 📥 Instalasi

### Windows

1. **Pastikan PHP sudah terinstall:**
   ```cmd
   php -v
   ```

2. **Download file CLI:**
   ```cmd
   # Download dari repo GitHub
   git clone https://github.com/arcode13/ovo
   cd ovo
   ```

3. **Jalankan OVO CLI:**
   ```cmd
   php ovo.php
   ```

### Linux / macOS

1. **Install PHP (jika belum ada):**
   ```bash
   # Ubuntu/Debian
   sudo apt update
   sudo apt install php php-openssl php-curl php-json php-mbstring
   
   # macOS (dengan Homebrew)
   brew install php
   ```

2. **Clone atau download repository:**
   ```bash
   git clone https://github.com/arcode13/ovo
   cd ovo
   ```

3. **Beri izin eksekusi (opsional):**
   ```bash
   chmod +x ovo.php
   ```

4. **Jalankan OVO CLI:**
   ```bash
   php ovo.php
   ```

### Android (Termux)

1. **Install Termux dari [F-Droid](https://f-droid.org/repo/com.termux_1022.apk)**

2. **Install PHP di Termux:**
   ```bash
   pkg update
   pkg install php
   ```

3. **Clone repository:**
   ```bash
   git clone https://github.com/arcode13/ovo
   cd ovo
   ```

4. **Jalankan OVO CLI:**
   ```bash
   php ovo.php
   ```

---

## 🚀 Penggunaan

### 1. Aktivasi Lisensi (Pertama Kali)

Saat pertama kali menjalankan OVO CLI, Anda akan diminta untuk memasukkan kode aktivasi:

```bash
╔═══════════════════════╗
║        OVO CLI        ║
╠═══════════════════════╣
║ Telegram: @mangetaaa  ║
╚═══════════════════════╝

🔑 Kode Aktivasi: ************
🔄 Aktivasi...

╔═══════════════════════╗
║    ✅ LISENSI AKTIF   ║
╠═══════════════════════╣
║ Expires: 27 Okt 2025  ║
║ Sisa: 1 hari          ║
║                       ║
║ Telegram: @mangetaaa  ║
╚═══════════════════════╝
```

### 2. Login Akun OVO

Jika belum ada akun, Anda akan diminta untuk login:

```bash
Nomor HP: 081234567890
🔄 Memproses...
OTP telah dikirim ke +6281234567890.

Kode OTP [r=Kirim Ulang]: 123456
✅ OTP valid.

PIN (6 digit): ******
✅ Login Akun +6281234567890 berhasil.

┌──────────┬───────────────────────────┬──────────┬──────────────┐
│ Nomor HP │ Email                     │ OVO Cash │ OVO Points   │
├──────────┼───────────────────────────┼──────────┼──────────────┤
│ 08xxx    │ david.rodriguez@gmail.com │ Rp 5.000 │ 1.234        │
└──────────┴───────────────────────────┴──────────┴──────────────┘
```

### 3. Menu Utama

Setelah login, Anda akan melihat menu utama:

```bash
┌──────────┬───────────────────────────┬──────────┬──────────────┐
│ Nomor HP │ Email                     │ OVO Cash │ OVO Points   │
├──────────┼───────────────────────────┼──────────┼──────────────┤
│ 08xxx    │ david.rodriguez@gmail.com │ Rp 5.000 │ 1.234        │
└──────────┴───────────────────────────┴──────────┴──────────────┘

1. Konfigurasi
2. Transfer sesama OVO
3. Transfer ke Bank
4. Bayar QRIS
5. Transaksi
6. Refresh
7. Keluar

Pilih menu [1-7]:
```

### 4. Transfer OVO ke OVO

#### Tanpa Jeda / Jeda Berlaku:

```bash
────────── Transfer Sesama OVO ──────────

Nomor tujuan: 081111111111
Jumlah transfer: 50000
Catatan (opsional): Kiriman untuk makan siang
PIN: ******

🔄 Memproses transfer...
✅ Transfer berhasil.
```

#### Dengan Jeda Aktif:

```bash
────────── Transfer Sesama OVO ──────────

Nomor tujuan: 081111111111
Jumlah transfer: 50000
Catatan (opsional): Kiriman untuk makan siang
PIN: ******

⏳ Transfer ke OVO akan diproses dalam 3 menit 45 detik
...

✅ Transfer berhasil.
─────────────── Selesai ────────────────
```

### 5. Transfer ke Bank

#### Pencarian Bank:

```bash
────────── Transfer ke Bank ──────────

Ketik s untuk cari bank.
Kode bank: s

───────── Cari Bank [b=kembali] ─────────

Nama bank (mis: bca): bca

┌────┬────────────────────────┬──────┐
│ No │ Bank                   │ Kode │
├────┼────────────────────────┼──────┤
│ 1  │ Bank BCA               │ 008  │
│ 2  │ Bank BCA DIGITAL       │ 009  │
└────┴────────────────────────┴──────┘

Pilih nomor bank (cth: 1): 1
Transfer ke Bank: Bank BCA

Nomor rekening: 1234567890
Jumlah transfer: 100000
Catatan (opsional): 
PIN: ******

🔄 Memproses transfer...
✅ Transfer ke bank berhasil.
```

### 6. Pembayaran QRIS

#### Menggunakan Merchant Tersimpan:

```bash
────────── Bayar QRIS ──────────

Daftar Merchant:
1) Warung Kopi ABC (Terakhir: 27 Okt 2025 - 14:30)
2) Kelontong Cabang A (Terakhir: 26 Okt 2025 - 10:15)

Pilih Merchant atau Input QRIS ID: 1
Bayar QRIS ke Warung Kopi ABC

Jumlah bayar: 25000
PIN: ******

🔄 Memproses QRIS...
✅ Pembayaran QRIS di Warung Kopi ABC berhasil.
```

#### Input QRIS ID Manual:

```bash
────────── Bayar QRIS ──────────

QRIS ID: 00020101021126670016COM.NOBUBANK.WWW...
Jumlah bayar: 30000
PIN: ******

🔄 Memproses QRIS...
✅ Pembayaran QRIS berhasil.
```

### 7. Lihat Riwayat Transaksi

```bash
────────── 10 Transaksi Terakhir ──────────

┌─────────────────────┬───────────────┬─────────────────┬─────────────┐
│ Tanggal & Waktu     │ Nama          │ Deskripsi       │ Jumlah      │
├─────────────────────┼───────────────┼─────────────────┼─────────────┤
│ 27 Okt 2025, 16:43  │ Warung Kopi   │ QRIS Payment    │ Rp 25.000   │
│ 27 Okt 2025, 14:30  │ John Smith    │ Transfer OVO    │ Rp 50.000   │
│ 27 Okt 2025, 12:15  │ Bank BCA      │ Transfer Bank   │ Rp 100.000  │
└─────────────────────┴───────────────┴─────────────────┴─────────────┘
```

### 8. Manajemen Akun (Menu Konfigurasi)

#### Login Akun Baru:
```bash
─────────── Konfigurasi ───────────

a) Akun
b) QRIS
c) Kembali

Pilih [a/b/c]: a

a) Login Baru
b) Ganti Akun
c) Hapus Akun
d) Kembali

Pilih [a/b/c/d]: a
```

#### Ganti Akun:
```bash
─────────── Ganti Akun ───────────

Daftar Akun:
1) 081111111111 (michael.anderson@gmail.com)
2)* 081234567890 (sophia.martinez@gmail.com) ← Aktif

Pilih Akun Tersedia (cth: 1): 1
✅ Akun OVO diganti.
```

#### Hapus Akun:
```bash
─────────── Hapus Akun ───────────

Daftar Akun:
1) 081111111111
2)* 081234567890 (Aktif)

Pilih Akun yang akan dihapus (cth: 1): 1
Yakin hapus akun 081111111111? (y/n): y
✅ Akun 081111111111 berhasil dihapus.
```

### 9. Konfigurasi Jeda Transfer

```bash
─────────── Konfigurasi ───────────

a) Akun
b) QRIS
c) Jeda
d) Kembali

Pilih [a/b/c/d]: c

───────── Konfigurasi • Jeda ─────────

Jeda Transfer Saat Ini:
├─ Transfer OVO   : 5 menit
├─ Transfer Bank  : 10 menit
└─ Bayar QRIS     : 3 menit

Atur Jeda:
a) Transfer OVO
b) Transfer Bank
c) Bayar QRIS
d) Kembali

Pilih [a/b/c/d]: a

───────── Atur Jeda • Transfer OVO ─────────

Jeda saat ini: 5 menit

Jeda baru (menit, 0 = nonaktif): 0
✅ Jeda Transfer OVO diatur menjadi 0 menit.
```

### 10. Manajemen QRIS (Menu Konfigurasi)

```bash
─────────── Konfigurasi ───────────

a) Akun
b) QRIS
c) Jeda
d) Kembali

Pilih [a/b/c/d]: b

─────────── Konfigurasi • QRIS ───────────

┌────┬──────────────────────┬─────────────────────┐
│ No │ Merchant             │ Terakhir Dibayar    │
├────┼──────────────────────┼─────────────────────┤
│ 1  │ Warung Kopi ABC      │ 27 Okt 2025 - 14:30 │
│ 2  │ Kelonton Cabang A    │ 26 Okt 2025 - 10:15 │
└────┴──────────────────────┴─────────────────────┘

a) Hapus QRIS
b) Kembali

Pilih [a/b]: a

─────────── Hapus QRIS ───────────

Hapus QRIS nomor (cth: 1): 1
✅ QRIS Warung Kopi ABC berhasil dihapus.
```

---

## 🔧 Fitur Detail

### 🔐 Manajemen Lisensi

#### Aktivasi Lisensi
```bash
# Validasi lisensi saat startup
- Aktivasi dengan kode unik
- Validasi tanggal kadaluarsa
- Cek status aktif
- Otomatis divalidasi
```

#### Penyimpanan Data
```bash
# Data tersimpan dengan aman
- Enkripsi file lokal
- Sinkronisasi server
- Backup otomatis
```

### 💼 Manajemen Multi-Akun

#### Fitur Akun
```bash
✅ Akun tidak terbatas
✅ Ganti akun cepat
✅ Sinkronisasi saldo otomatis
✅ Manajemen sesi
✅ Penghapusan akun
✅ Tampilan email & telepon
```

#### Penyimpanan Data
```bash
# Data tersimpan dengan aman di server:
- Koneksi aman
- Sinkronisasi otomatis
- Update real-time
```

### 💸 Transfer & Pembayaran

#### Transfer OVO ke OVO
```bash
✅ Verifikasi nomor penerima
✅ Cek saldo cukup
✅ Validasi PIN
✅ Pemrosesan real-time
✅ Simpan ke riwayat otomatis
```

#### Transfer Bank
```bash
✅ Dukungan 100+ bank
✅ Pencarian bank berdasarkan nama
✅ Verifikasi nama rekening
✅ Minimal Rp 10.000
✅ Inquiry real-time
```

#### Pembayaran QRIS
```bash
✅ Scan kode QRIS
✅ Simpan merchant otomatis
✅ Bayar cepat dari favorit
✅ Riwayat pembayaran
✅ Timestamp terakhir digunakan
```

### 📊 Riwayat Transaksi

```bash
✅ 10 transaksi terakhir
✅ Format tanggal & waktu
✅ Nama merchant
✅ Deskripsi transaksi
✅ Jumlah dalam Rupiah
✅ Format Indonesia
```

### ⏱️ Jeda Transfer (Anti-Spam)

#### Konfigurasi Jeda
```bash
✅ Atur jeda untuk setiap tipe transaksi
✅ Delay terpisah untuk OVO/Bank/QRIS
✅ Bisa dinonaktifkan (set 0 menit)
✅ Disimpan otomatis di database
✅ Cross-device sync
```

#### Cara Kerja
```bash
✅ Transaksi pertama: Langsung diproses
✅ Transaksi kedua: Countdown muncul jika masih dalam periode jeda
✅ Setelah countdown: Transaksi otomatis diproses
✅ API tidak di-hit saat countdown (anti-spam)
```

### 🎨 User Experience

#### Loading Bar
```bash
[████████████████████████░░░░] 85%
```

#### Pesan Error
```bash
❌ Gagal: Kode OTP tidak valid
❌ Gagal: Saldo tidak cukup
❌ Gagal: Lisensi dicabut
```

#### Pesan Sukses
```bash
✅ Transfer berhasil
✅ Login Akun berhasil
✅ QRIS berhasil dihapus
```

---

## 🔒 Keamanan

### Sistem Keamanan

```bash
✅ Koneksi aman dengan server
✅ Perlindungan data pengguna
✅ Enkripsi storage lokal
✅ Validasi setiap request
✅ Proteksi akses tidak sah
```

### Perlindungan Data

```bash
✅ Data tersimpan terenkripsi
✅ Sync dengan server
✅ Backup otomatis
✅ Manajemen sesi
✅ Pembersihan otomatis
```

---

## 🐛 Troubleshooting

### Masalah: Lisensi Kadaluarsa

```bash
# Error yang muncul:
╔═══════════════════════╗
║   ❌ LISENSI EXPIRED  ║
╠═══════════════════════╣
║ Expired: 27 Okt 2025  ║
╚═══════════════════════╝

# Solusi: Hubungi admin untuk perpanjangan
Telegram: @mangetaaa
```

### Masalah: Koneksi ke Server Gagal

```bash
# Cek koneksi internet
ping api-server.com

# Cek firewall
# Buka port 443 (HTTPS)
```

### Masalah: Ekstensi PHP Hilang

```bash
# Ubuntu/Debian
sudo apt install php-openssl php-curl php-json php-mbstring

# CentOS/RHEL
sudo yum install php-openssl php-curl php-json php-mbstring

# macOS
brew install php
```

### Masalah: OTP Tidak Terkirim

```bash
# Pastikan nomor HP dalam format valid:
✅ 081234567890
✅ +6281234567890
✅ 6281234567890

❌ 081-234-567-890
❌ 081 234 567 890
```

### Masalah: Pembayaran QRIS Gagal

```bash
# Pastikan QR code adalah QRIS yang valid
✅ Dimulai dengan "0002"
✅ Format EMV QRIS
✅ Merchant mendukung OVO

# Tips:
- Pastikan QRIS dari merchant resmi
- Cek kode minimal 50 karakter
- Pastikan saldo cukup
```

---

## 📞 Kontak & Lisensi

### 💬 Beli Lisensi

**Telegram:** [@mangetaaa](https://t.me/mangetaaa)

Untuk mendapatkan kode aktivasi dan lisensi, silakan hubungi admin melalui Telegram.

### 🌐 Repository

**GitHub:** [https://github.com/arcode13/ovo](https://github.com/arcode13/ovo)

### 📝 Lisensi

Software ini adalah proprietary software yang memerlukan lisensi valid untuk operasi. Distribusi, modifikasi, atau reverse engineering tanpa izin adalah ilegal.

**Fitur Lisensi:**
- 📌 Binding ke perangkat spesifik
- ⏰ Expiration otomatis
- 🔒 Validasi server-side
- 🚫 Dukungan revokasi

---

## 📋 Credits

- **OVO** - Payment platform
- **PHP Community** - Documentation & support
- **Developers** - Testing & feedback

---

## 📝 Changelog

### Version 1.0 (Current)
- 

---

<div align="center">

**⭐ Star repo ini jika membantu!**

[⬆ Kembali Ke Atas](#-ovo-cli---command-line-interface-untuk-ovo)

</div>