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

## Struktur Project
- `/fix` → Berisi hasil build WebGL (deploy-ready)
- `/Assets` → Asset Unity (model, script, dll)
- `/ProjectSettings` → Konfigurasi project Unity
- `/QR` → Marker yang digunakan untuk AR

---

## Cara Kerja
- Aplikasi mengakses kamera melalui browser
- Marker dideteksi menggunakan Zappar
- Objek 3D ditampilkan di atas marker
- User dapat berinteraksi (rotate objek)

---

## Marker (QR / Image Target)

Gunakan marker berikut untuk menjalankan AR:

![Marker AR](QR/marker.png)

---

## Izin Kamera
- Browser akan meminta izin akses kamera saat pertama kali dibuka
- Aplikasi harus dijalankan melalui HTTPS
- Tanpa izin kamera, fitur AR tidak akan berjalan

---

## Cara Menjalankan
1. Buka link demo melalui browser mobile
2. Izinkan akses kamera
3. Arahkan kamera ke marker (QR di atas)
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
- Pastikan menggunakan browser modern (Chrome / Safari)

---

## Demo

[Link Demo AR](https://elaborate-entremet-53e20f.netlify.app/)
