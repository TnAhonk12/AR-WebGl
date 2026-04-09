# AR WebGL (Zappar - Unity)

## Deskripsi
Fitur Augmented Reality (AR) berbasis web menggunakan Unity WebGL dan Zappar SDK.  
Aplikasi ini memungkinkan pengguna menampilkan objek 3D melalui kamera perangkat secara real-time menggunakan marker.

---

## Teknologi
- Unity (WebGL)
- Zappar SDK (WebAR)
- JavaScript (browser integration)
- WebRTC (akses kamera)

---

## Cara Kerja
- Aplikasi mengakses kamera melalui browser
- Marker dideteksi menggunakan Zappar
- Objek 3D ditampilkan di atas marker
- User dapat berinteraksi (rotate objek)

---

## Izin Kamera
- Browser akan meminta izin akses kamera saat pertama kali dibuka
- Aplikasi harus dijalankan melalui HTTPS
- Tanpa izin kamera, fitur AR tidak akan berjalan

---

## Cara Menjalankan
1. Buka link hosting melalui browser mobile
2. Izinkan akses kamera
3. Arahkan kamera ke marker
4. Interaksikan objek dengan gesture sentuh

---

## Integrasi dengan Flutter
Unity WebGL dapat dijalankan di dalam WebView Flutter dengan memuat URL aplikasi.

Jika diperlukan komunikasi:
- Unity → menggunakan `SendMessage`
- Flutter → menggunakan JavaScript bridge

---

## Catatan
- AR berbasis WebGL bergantung pada dukungan browser
- Performa dapat berbeda tergantung perangkat
