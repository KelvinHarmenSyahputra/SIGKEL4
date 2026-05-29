# BuyCar Maps - Sistem Informasi Geografis Sebaran Dealer & Showroom Mobil Kota Pekanbaru

BuyCar Maps adalah aplikasi Sistem Informasi Geografis (SIG) berbasis web interaktif yang memetakan secara spasial sebaran lokasi **Dealer Mobil Baru** dan **Showroom Mobil Bekas** di seluruh wilayah Kota Pekanbaru. Aplikasi ini dirancang untuk memberikan kemudahan bagi masyarakat dan calon pembeli dalam mencari, memfilter, dan menemukan rute perjalanan menuju lokasi dealer terdekat.

---

## 🚀 Fitur Utama

Aplikasi ini dilengkapi dengan antarmuka modern bermaterial gelap (Dark Mode) serta berbagai fitur interaktif:

1. **Loading Screen Animatif:** Animasi pembuka bertema mobil melaju di atas jalan raya (menggunakan SVG & CSS Keyframes) yang sinkron dengan proses inisialisasi peta.
2. **Pencarian Real-Time (Live Search Dropdown):** Fitur pencarian cepat di bagian navbar untuk memudahkan pengguna mengetik nama dealer yang diinginkan.
3. **Filter Spasial Dinamis (Bottom Filter Bar):** Memungkinkan pengguna memfilter visualisasi peta dalam satu klik:
   * **Semua:** Menampilkan seluruh titik lokasi.
   * **Dealer:** Menampilkan diler resmi kendaraan baru (Marker Merah 🔴).
   * **Showroom:** Menampilkan tempat penjualan mobil bekas (Marker Hijau 🟢).
4. **Info Panel Detail:** Panel sisi kanan (Right Sidebar) yang muncul secara elegan saat objek peta diklik untuk menyajikan data:
   * Foto Lokasi (jika tersedia).
   * Nama Tempat & Kategori (Dealer/Showroom).
   * Koordinat Geografis presisi (Latitude & Longitude).
   * Kalkulasi Jarak dari titik pengguna.
5. **Navigasi & Rute Pintar:**
   * **Tampilkan Rute:** Menggambar garis rute perjalanan di dalam peta aplikasi.
   * **Buka di Google Maps:** Integrasi tautan langsung (*deep-linking*) menuju Google Maps eksternal untuk navigasi GPS langsung.
6. **Geolocation (Locate Me):** Tombol kustom untuk melacak posisi perangkat pengguna saat ini secara *real-time*.
7. **Marker Clustering:** Pengelompokan marker otomatis berbasis kepadatan wilayah sebaran untuk menjaga performa rendering peta tetap ringan dan rapi.

---

## 🛠️ Teknologi & Pustaka Pendukung

Sistem ini dibangun dengan mengintegrasikan teknologi pemetaan GIS berbasis web dan *library* frontend modern:

* **Engine Utama & GIS:**
  * **QGIS:** Perangkat lunak untuk pemrosesan, analisis data spasial, dan *layouting* data vektor awal.
  * **qgis2web:** *Plugin* web-exporter untuk mengonversi berkas spasial QGIS menjadi kode web siap pakai.
* **Frontend Web Stack:**
  * **Leaflet.js:** Pustaka Javascript open-source utama untuk rendering peta interaktif.
  * **Inter Font Family:** Desain tipografi antarmuka premium untuk memaksimalkan keterbacaan teks.
* **Leaflet Plugins Ecosystem:**
  * `Leaflet.markercluster` — Manajemen pengklasteran titik marker.
  * `leaflet-measure` & `leaflet.photon` — Alat ukur spasial dan geocoding.
  * `L.Control.Layers.Tree` — Pengorganisasian struktur layer peta secara hierarkis.
  * `leaflet-hash` & `Autolinker.min.js` — Manajemen URL koordinat state dan tautan teks otomatis.

---

## 📁 Struktur Direktori Proyek

```text
├── index.html               # File utama struktur antarmuka & tata letak aplikasi
├── css/                     # Modul gaya tampilan (Leaflet, MarkerCluster, qgis2web, FontAwesome)
├── js/                      # Logika aplikasi, plugin Leaflet, dan engine ekspresi QGIS
└── data/                    # Dataset spasial Kota Pekanbaru dalam format JSON/JS Vektor
    ├── pekanbaru_1.js       # Data batas administrasi / wilayah Kota Pekanbaru
    ├── jalan_2.js           # Data jaringan jalan raya Kota Pekanbaru
    └── DEALERMOBILBARU_fix_3.js # Data koordinat titik spasial diler & showroom
```
---
👥 Kreator (Kelompok 4)
Aplikasi ini dikembangkan secara kolaboratif sebagai Proyek Tugas Akhir Mata Kuliah Sistem Informasi Geografis oleh[cite::

Nama Anggota 1
Nama Anggota 2
Nama Anggota 3
Nama Anggota 4
Nama Anggota 5
---

Aplikasi ini bisa lansung anda nikmati di website kami 
```text
https://kelvinharmensyahputra.github.io/SIGKEL4
```
