# 🌊PEMETAAN KERENTANAN BANJIR BERBASIS BIG DATA MENGGUNAKAN INTEGRASI DATA SPASIAL DAN SOSIODEMOGRAFI
---
## 👥Anggota Kelompok 06
| NAMA | NIM |
| --- | :---:|
| Mekar Cendra Narwastu | 123140074 |
| Mei Disti Ayuningtias | 123140076 |
| Ribka Hana Josephine Situmorang | 123140103 |
| Diwan Ramadhani Dwi Putra | 123140116 |
| M. Hafizurrahman Akbar | 123140123 |
| M. Gymnastiar Syahputra | 123140135 |
| Bima Aryaseta	| 123140177 |
---
## 📝Deskripsi Singkat
Proyek ini bertujuan untuk membangun model klasifikasi prediksi stroke menggunakan dataset kesehatan. Fokus utama dari proyek ini adalah penanganan imbalanced class (ketidakseimbangan kelas) yang umum terjadi pada dataset medis.
Model yang digunakan dalam proyek ini adalah Random Forest Classifier, dengan membandingkan tiga pendekatan penanganan data sebagai berikut:
| Metode | Deskripsi |
| :---: | --- |
| Baseline | Tanpa penanganan _imbalanced_ |
| SMOTE | _Synthetic Minority Over-sampling Technique_ |
| SMOTE-ENN | Kombinasi SMOTE dengan _Edited Nearest Neighbours_ |
---
## 📊Dataset
* **Data Topografi/Elevasi**: Menggunakan citra satelit SRTM resolusi 30 meter dari Google Earth Engine (GEE) yang dikonversi ke format CSV.
* **Data Tutupan Lahan**: Menggunakan data tutupan lahan MODIS (area hutan, sawah, pemukiman) dari GEE berskala raster (GeoTIFF).
* **Data Kepadatan & Kelompok Rentan Penduduk**: Data agregat tingkat kecamatan dari Badan Pusat Statistik (BPS) Lampung dalam format CSV/Excel.
* **Data Historis Kejadian Banjir**: Data titik kejadian historis dari Badan Nasional Penanggulangan Bencana (BNPB).
* **Data Curah Hujan Harian**: Data time-series (JSON/CSV) per kecamatan dari BMKG yang ditarik secara otomatis setiap hari menggunakan API resmi dan dikelola oleh pipeline Apache Kafka
---
## 📉Metrik Evaluasi
* Accuracy Exact Match
* Akurasi Toleransi ± 1 Kelas
* Koefisien Kappa
