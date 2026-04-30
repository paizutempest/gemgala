# 🌊 Gemgala Deep Ocean - Referral Research & Automation

![Gemgala Header](https://images.igemgala.com/prod/2b3aec32-2cbc-44f6-85e0-9cb65fae9d7b.png)

> **Status:** 🛠️ Researching / On Hold (Encountered `APP_SIGN` Encryption)  
> **Author:** Paizutempest

## 📖 Deskripsi
Proyek ini adalah hasil riset mendalam mengenai alur pendaftaran dan sistem referral pada aplikasi **Gemgala**. Dibuat menggunakan **Node.js** dan **Playwright**, bot ini dirancang untuk mensimulasikan pendaftaran pengguna baru secara otomatis dengan identitas perangkat yang unik.

## 🛠️ Tech Stack
* **Runtime:** Node.js[cite: 1]
* **Automation:** Playwright (Stealth Mode)[cite: 1]
* **API Client:** Axios[cite: 1]
* **Styling:** Chalk & Gradient-String[cite: 1]
* **Identity:** 200+ Random Mobile Device List[cite: 1]

## 🧬 Alur Sniffing (Workflow)
Bot ini mengikuti urutan request API asli hasil intersep via **Reqable**:
1. **Pre-Register:** Mengunci posisi referral melalui `pub/preRegister/getPosition`[cite: 1].
2. **Server Config:** Sinkronisasi konfigurasi perangkat[cite: 1].
3. **OTP Request:** Mengirim kode verifikasi ke email dinamis[cite: 1].
4. **Email Polling:** Menggunakan "Siluman Browser" untuk memantau inbox secara headless[cite: 1].
5. **Registration:** Eksekusi pendaftaran akun baru[cite: 1].
6. **Retention Injector:** Melaporkan durasi bermain via `reportGameDuration` agar referral dianggap High Quality[cite: 1].

## 🚧 Tantangan Saat Ini
Saat ini proyek tertahan di bagian **`APP_SIGN`**. Server Gemgala melakukan validasi *hash* dinamis pada setiap request. Tanpa mengetahui algoritma pembuat tanda tangan (signature) ini, request akan ditolak oleh server[cite: 1].

## 🧪 Cara Penggunaan (Untuk Riset)
1. Clone repositori:
   
```bash
   git clone [https://github.com/username/gemgala-deep-ocean.git](https://github.com/username/gemgala-deep-ocean.git)
