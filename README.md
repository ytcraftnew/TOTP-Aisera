# 🔐 Aisera TOTP Manager

Aisera TOTP Manager adalah aplikasi web sederhana untuk mengelola kode Two-Factor Authentication (2FA / TOTP) langsung di browser menggunakan JavaScript murni tanpa backend.

## ✨ Fitur

* 🔑 Generate kode TOTP real-time
* ⏱ Countdown timer 30 detik
* 💾 Penyimpanan akun menggunakan LocalStorage
* 🔐 Login protection menggunakan SHA-256 hash
* 📱 Responsive modern UI
* 📋 Copy OTP ke clipboard
* ➕ Tambah & hapus akun TOTP

---

# 📸 Tampilan

## Login Page

* Modern authentication screen
* SHA-256 credential verification

## Dashboard

* Daftar akun TOTP
* OTP code generator
* Live countdown timer
* Copy to clipboard

---

# 🛠 Teknologi

* HTML5
* CSS3
* Vanilla JavaScript
* Web Crypto API
* CryptoJS
* LocalStorage API

---

# 📂 Struktur Project

```bash
project/
│
├── TOTP Aisera.html
└── README.md
```

---

# 🚀 Cara Menjalankan

1. Download / clone project
2. Buka file `TOTP Aisera.html`
3. Jalankan langsung di browser

Atau gunakan local server:

```bash
python -m http.server
```

lalu buka:

```txt
http://localhost:8000
```

---

# 🔐 Sistem Login

Aplikasi menggunakan SHA-256 hash untuk validasi login.

Format hash:

```txt
SHA256(admin_aisera:AiseraJaya2026!)
```

Hash yang digunakan di project:

```txt
3e6cb84fa8f6bd5b9136d5a907a22de513c0699ae4d490d344769ee4510229b8
```

---

# 📦 Penyimpanan Data

Data akun TOTP disimpan di browser menggunakan:

```js
localStorage
```

Key storage:

```txt
aisera_totp_accounts
```

Session login menggunakan:

```txt
sessionStorage
```

Key:

```txt
aisera_logged_in
```

---

# ⚠️ Catatan Keamanan

Project ini dibuat untuk pembelajaran dan penggunaan lokal.

Karena semua data disimpan di browser:

* Jangan gunakan untuk production tanpa enkripsi tambahan
* Jangan menyimpan secret key sensitif di device publik

---

# 📄 License

Free to use for educational purposes.
