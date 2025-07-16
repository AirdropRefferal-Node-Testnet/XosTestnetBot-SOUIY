# XOS Testnet Bot - Panduan Instalasi dan Penggunaan

## Deskripsi
Bot ini dirancang untuk otomatisasi aktivitas di jaringan testnet XOS, termasuk:
- Swap token (XOS, USDC, BNB)
- Daily check-in
- Pembuatan token
- Deploy kontrak pintar

## Persyaratan Sistem
- Node.js v18 atau lebih baru
- NPM atau Yarn
- Git

## Instalasi

### 1. Clone Repository
```bash
git clone https://github.com/AirdropRefferal-Node-Testnet/XosTestnetBot-SOUIY.git
cd XosTestnetBot-SOUIY
```

### 2. Instal Dependensi
```bash
npm install
```
#### atau
```bash
yarn install
```

### 3. Persiapan File Konfigurasi
Edit file `account.json` 
```bash
nano account.json
```

#### Dengan format berikut:
```json
[
  {
    "privateKey": "YOUR_PRIVATE_KEY",
    "token": "YOUR_XOS_TOKEN"
  }
]
```

**Catatan:** Anda bisa menambahkan banyak akun dalam array.

### 4. File Proxy (Opsional)
Buat file `proxy.txt` dan masukkan daftar proxy Anda (satu proxy per baris):
```
http://user:pass@ip:port
socks://user:pass@ip:port
```

## Penggunaan

### Menjalankan Bot
```bash
node index.js
```

### Menu Utama
1. **Start Daily Activity**: Memulai aktivitas harian otomatis
2. **Manual Configuration**: Konfigurasi manual parameter swap
3. **Was Labs**: Fitur lanjutan (buat token, deploy kontrak)
4. **Clear Logs**: Membersihkan log transaksi
5. **Refresh**: Memperbarui data wallet
6. **Exit**: Keluar dari aplikasi

### Fitur Utama
1. **Daily Activity**:
   - Swap otomatis antara XOS, USDC, dan BNB
   - Daily check-in otomatis
   - Dapat dijalankan untuk semua akun sekaligus

2. **Was Labs**:
   - **Auto Create Token**: Buat token baru di testnet
   - **Auto Deploy Contract**: Deploy kontrak pintar

## Konfigurasi
File `config.json` akan dibuat otomatis setelah pertama kali menjalankan bot. Anda bisa mengeditnya secara manual atau melalui menu:
- Swap repetitions: Jumlah swap per akun
- XOS Swap Range: Range jumlah XOS untuk swap
- USDC/BNB Swap Range: Range jumlah token untuk swap

## Troubleshooting
1. **Error Koneksi**:
   - Pastikan RPC URL aktif
   - Periksa koneksi internet
   - Verifikasi proxy (jika digunakan)

2. **Error Transaksi**:
   - Pastikan ada cukup gas (XOS)
   - Periksa saldo token yang cukup
   - Cek nonce wallet

3. **Error Lainnya**:
   - Hapus `node_modules` dan install ulang dependensi
   - Pastikan versi Node.js sesuai

## Dukungan
- Ikuti [TikTok AirdropRefferal](https://www.tiktok.com/@souiy1) untuk update terbaru
- Donasi untuk Palestina: [Dompet Dhuafa](https://digital.dompetdhuafa.org/donasi/jagapalestina)


**Catatan:** Bot ini hanya untuk jaringan testnet. Jangan gunakan private key mainnet.
