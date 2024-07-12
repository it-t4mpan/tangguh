# TANGGUH
**Tata Amanat Network Generik Guna Update dan Hardening**

**reC0ded by IT T4mp@n, 2024 - S0URCE BY XSAN LAHCI**

Script ini bertujuan untuk melakukan hardening dan pembaruan pada sistem Ubuntu, serta mengatasi kerentanan CVE-2024-6387. Berikut adalah langkah-langkah yang dilakukan oleh script ini:

## Langkah-langkah Hardening

1. **Pembaruan Paket**
   - Memperbarui daftar paket dan meng-upgrade semua paket yang terinstal.

2. **Pembaruan OpenSSH**
   - Meng-upgrade OpenSSH untuk memitigasi CVE-2024-6387.

3. **Hardening SSH**
   - Menonaktifkan login root.
   - Menonaktifkan otentikasi password.
   - Mengubah port SSH dari 22 ke 2222.
   - Menambahkan catatan mitigasi CVE-2024-6387.

4. **Instalasi Fail2ban**
   - Melindungi dari serangan brute-force dengan menginstal dan mengonfigurasi Fail2ban.

5. **Instalasi ModSecurity**
   - Menginstal ModSecurity sebagai Web Application Firewall (WAF) untuk melindungi aplikasi web.

6. **Instalasi ClamAV**
   - Menginstal ClamAV sebagai antivirus untuk memindai dan melindungi sistem dari malware.

7. **Instalasi Rootkit Hunter**
   - Menginstal Rootkit Hunter untuk mendeteksi rootkit dan ancaman keamanan lainnya.

8. **Konfigurasi Firewall (UFW)**
   - Mengonfigurasi UFW untuk membatasi lalu lintas masuk dan mengizinkan port tertentu.

9. **Pembaruan Keamanan Otomatis**
   - Mengatur pembaruan keamanan otomatis agar sistem selalu mendapatkan patch terbaru.

10. **Instalasi dan Konfigurasi AIDE**
    - Menginstal dan mengonfigurasi AIDE untuk mendeteksi perubahan file yang tidak sah.

11. **Aktivasi Fitur Keamanan Kernel**
    - Mengaktifkan pengaturan keamanan kernel untuk melindungi dari berbagai serangan jaringan.

12. **Pembatasan Penggunaan Sudo**
    - Mengkonfigurasi sudo untuk meminta password setiap kali perintah sudo dijalankan.

## Cara Menggunakan

1. Pastikan Anda memiliki akses root atau menggunakan `sudo`.
2. Unduh script ini dan jalankan dengan perintah:
   ```bash
   chmod +x tangguh-v1.sh.x
   sudo ./tangguh-v1.sh.x
