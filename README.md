# Tugas 3 – Advanced Network Security

Repository ini berisi laporan teknis **Tugas 3** untuk mata kuliah **Advanced Network Security**. Laporan ini mendokumentasikan proses instalasi aplikasi rentan (DVWA) serta simulasi berbagai teknik serangan jaringan menggunakan alat keamanan di lingkungan Linux.

---

## Isi Tugas
Laporan ini mencakup dua bagian utama:

### 1. Instalasi & Konfigurasi Sistem
- **Deployment DVWA**: Proses pengunduhan source code dari GitHub dan pemasangan pada direktori `/var/www/html/dvwa`.
- **Konfigurasi Database**: Pengaturan MariaDB meliputi pembuatan database `dvwa`, manajemen hak akses user, dan sinkronisasi file `config.inc.php`.
- **Environment Adjustment**: Konfigurasi izin akses folder (`chmod 777`) dan pengaturan `php.ini` (allow_url_include) untuk kebutuhan simulasi.

### 2. Simulasi Serangan Jaringan
- **Network Reconnaissance**: Pemindaian port aktif menggunakan **Nmap** (Port 23 & Port 80).
- **SYN Flood Attack**: Simulasi serangan Denial of Service (DoS) pada transport layer menggunakan **hping3**.
- **ICMP Flood**: Pengujian beban jaringan (stress testing) dengan pengiriman paket ICMP secara agresif (13.000+ paket dalam waktu singkat).
- **Smurf Attack**: Simulasi serangan berbasis **IP Spoofing** dan **Broadcast Amplification** menggunakan protokol ICMP.

---

## Tools yang Digunakan
- **Sistem Operasi**: Linux (dengan Thunar File Manager)
- **Scanner**: Nmap
- **Attack Tool**: hping3
- **Platform**: DVWA (Damn Vulnerable Web Application)

---

## Tujuan Tugas
- Memahami prosedur instalasi dan konfigurasi server web untuk keperluan pengujian keamanan.
- Menganalisis dampak dari serangan banjir paket (Flooding) terhadap ketersediaan sistem.
- Mempelajari mekanisme pemalsuan identitas jaringan (IP Spoofing) melalui hping3.

---


## Catatan
Dokumen ini dibuat semata-mata untuk **keperluan pembelajaran dan pemenuhan Tugas 3**. Seluruh simulasi dilakukan di lingkungan lokal yang aman dan terkontrol.
