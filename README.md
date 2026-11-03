# 🌿 PlantCare - Aplikasi Penjadwalan Penyiraman Tanaman Berbasis IoT

PlantCare adalah sistem pintar berbasis *Internet of Things* (IoT) yang memungkinkan pengguna untuk memantau, mengontrol, dan menjadwalkan penyiraman tanaman secara otomatis melalui aplikasi *mobile*. Sistem ini memastikan tanaman Anda selalu mendapatkan hidrasi yang tepat, bahkan saat Anda tidak berada di rumah.

## ✨ Fitur Utama

Berdasarkan rancangan antarmuka, aplikasi ini mendukung fitur-fitur berikut:
*   🔗 **Pairing Perangkat IoT:** Menghubungkan aplikasi *mobile* dengan perangkat *hardware* (mikrokontroler/pompa) dengan mudah.
*   💧 **Penyiraman Manual (Siram Sekarang):** Mengaktifkan pompa air secara *real-time* langsung dari *smartphone*.
*   📅 **Penjadwalan Otomatis:** Membuat, mengedit, dan menghapus jadwal penyiraman harian atau mingguan agar tanaman disiram secara konsisten.
*   📊 **Monitoring Status Real-Time:** 
    *   Memantau status koneksi alat (Online/Offline).
    *   Mengecek status ketersediaan air (Tangki Normal / Tangki Hampir Habis).
    *   Melihat status aktivitas alat (Sedang Menyiram / Siaga).
*   🔔 **Sistem Notifikasi:** Peringatan pintar yang akan muncul jika air di tangki habis atau jika perangkat IoT terputus dari jaringan.

## 🛠️ Teknologi yang Digunakan

*(Silakan ubah bagian ini sesuai dengan teknologi spesifik yang Anda gunakan dalam pengembangan)*

**Hardware (Perangkat IoT):**
*   Mikrokontroler: ESP32 
*   Aktuator:  Pompa Air 5V / 12V, Modul Relay
*   Sensor: Soil Moisture Sensor

**Software & Backend:**
*   Frontend/Mobile App: Flutter
*   Backend/Database: Firebase Realtime Database 
*   Protokol Komunikasi: HTTP REST API]
*   Desain UI/UX: Figma

## 🚀 Cara Instalasi dan Penggunaan

### Prasyarat
*   Node.js (jika menggunakan React Native/Backend JS)
*   Flutter SDK (jika menggunakan Flutter)
*   Arduino IDE / PlatformIO (untuk *flashing hardware*)

### Menjalankan Aplikasi Mobile
1. Clone repositori ini:
   ```bash
   git clone [https://github.com/username-anda/plantcare-iot.git](https://github.com/username-anda/plantcare-iot.git)

   Masuk ke direktori proyek aplikasi:Bashcd plantcare-iot/app
Instal semua dependensi:Bashnpm install # atau 'flutter pub get'
Jalankan aplikasi di emulator atau perangkat fisik:Bashnpm run android # atau 'flutter run'
Setup Perangkat Keras (IoT)Buka source code hardware di direktori /hardware menggunakan Arduino IDE.
Ubah konfigurasi WiFi (SSID dan Password) serta kredensial database/MQTT pada file config.h.
Hubungkan mikrokontroler ke komputer dan lakukan upload kode.
📱 Tangkapan Layar (UI/UX)(Tambahkan gambar hasil ekspor dari desain Figma Anda di sini)Beranda (Status Alat)
Pengaturan JadwalSiram Manual🤝 
KontribusiKontribusi selalu diterima! Jika Anda ingin berkontribusi:Fork repositori ini.
Buat branch fitur baru (git checkout -b fitur-baru).
Lakukan commit perubahan Anda (git commit -m 'Menambahkan fitur baru').
Push ke branch tersebut (git push origin fitur-baru).Buat Pull Request.
