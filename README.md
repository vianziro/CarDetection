# Sistem Deteksi, Klasifikasi, Tracking, dan Counting Kendaraan Berbasis Video

Proyek ini bertujuan untuk membangun sistem cerdas yang mampu mendeteksi, melacak, mengklasifikasikan, dan menghitung kendaraan secara otomatis dari sebuah video lalu lintas menggunakan teknologi deep learning.

## 🔧 Teknologi yang Digunakan

- **YOLOv8**: Deteksi objek kendaraan secara real-time.
- **DeepSORT**: Pelacakan kendaraan antar frame dengan ID unik.
- **ResNet50**: Klasifikasi merek kendaraan berdasarkan dataset mobil Indonesia.
- **Python, PyTorch, OpenCV, NumPy, Pandas**

##  Arsitektur Sistem

```text
[ Video Input ]
       ↓
[ YOLOv8 - Deteksi Mobil ]
       ↓
[ DeepSORT - Pelacakan Objek ]
       ↓
[ Crop Gambar Mobil Detected ]
       ↓
[ ResNet50 - Klasifikasi Merek Mobil ]
       ↓
[ Mapping Merek ke Kategori (MPV, SUV, dll) ]
       ↓
[ Visualisasi + Log ke CSV + Counting ]
       ↓
[ Output Video Akhir + Statistik ]
```

## Hasil Utama
1. Akurasi klasifikasi kendaraan: 95.05%
2. Deteksi dan tracking stabil dengan DeepSORT
3/ Label bounding box mencantumkan kategori & merek: Contoh: MPV - Toyota Avanza, SUV - Pajero


Sistem ini dikembangkan sebagai bagian dari proyek pengolahan video dan AI untuk pemantauan lalu lintas otomatis.
