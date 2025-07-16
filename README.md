# SOUIY XOS Testnet Auto Bot

## Deskripsi
Bot otomatis untuk berpartisipasi dalam testnet XOS. Bot ini dirancang untuk membantu Anda berinteraksi dengan jaringan testnet XOS secara otomatis.

## Persyaratan Sistem
- Node.js (versi 16 atau lebih baru)
- NPM (biasanya terinstal bersama Node.js)
- Git

## Instalasi

### 1. Clone Repository
```bash
git clone https://github.com/AirdropRefferal-Node-Testnet/XosTestnetBot-SOUIY.git
```

### 2. Masuk ke Direktori Proyek
```bash
cd XosTestnetBot-SOUIY
```

### 3. Instal Dependensi
```bash
npm install
```

## Konfigurasi

### 1. Buat File account.json
Buat file `account.json` di root direktori proyek dan isi dengan konfigurasi Anda:

```bash
nano account.json
```

Isi dengan format berikut:
```json
{
  "privateKey": "your_private_key_here",
  "bearerToken": "your_bearer_token_here"
}
```

Simpan file dengan menekan:
1. `Ctrl+O` lalu Enter untuk menyimpan
2. `Ctrl+X` untuk keluar dari nano

### 2. Verifikasi Konfigurasi
Pastikan file `account.json` telah dibuat dengan benar:
```bash
cat account.json
```

## Penggunaan

### Menjalankan Bot
```bash
node index.js
```

### Opsi Command Line
Bot mungkin mendukung beberapa argumen command line. Gunakan `--help` untuk melihat opsi yang tersedia:
```bash
node index.js --help
```

## Struktur File Penting
```
XosTestnetBot-SOUIY/
├── account.json       # File konfigurasi akun
├── index.js          # File utama bot
├── package.json      # Dependensi proyek
└── README.md         # Panduan penggunaan
```

## Keamanan
- **JANGAN** berbagi file `account.json` dengan siapapun
- **JANGAN** commit file `account.json` ke repository publik
- Simpan private key dan bearer token Anda dengan aman

## Troubleshooting

### Error: File account.json tidak ditemukan
Pastikan:
1. File `account.json` ada di direktori utama proyek
2. Nama file tepat `account.json` (perhatikan huruf besar/kecil)

### Error Format JSON tidak valid
Gunakan tools seperti [JSONLint](https://jsonlint.com/) untuk memverifikasi format JSON Anda valid

## Kontribusi
Kontribusi dipersilakan! Silakan buka issue atau pull request untuk melaporkan bug atau menambahkan fitur baru.

## DONASI
- Satukan Solidaritas Bantu Palestina!
[PEDULI PALESTINA](https://digital.dompetdhuafa.org/donasi/jagapalestina)

