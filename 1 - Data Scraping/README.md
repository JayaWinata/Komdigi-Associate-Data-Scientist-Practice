# Praktikum Data Scraping

## 1. Identifikasi Kebutuhan Data
**Proyek:** Prediksi Harga Rumah (House Price Prediction)  

| Fitur | Alasan Penting | Ketersediaan Data |
|-------|----------------|------------------|
| **Luas Bangunan (sqft/㎡)** | Semakin besar bangunan, biasanya harga semakin tinggi. | Ada di dataset Kaggle (House Prices). |
| **Jumlah Kamar Tidur (Bedrooms)** | Indikator kapasitas rumah, memengaruhi harga. | Tersedia di dataset publik. |
| **Jumlah Kamar Mandi (Bathrooms)** | Menambah kenyamanan, berdampak pada harga. | Tersedia di dataset. |
| **Lokasi** | Faktor utama harga rumah (akses transportasi, sekolah, fasilitas umum). | Ada di dataset|
| **Tahun Dibangun (Year Built)** | Usia rumah memengaruhi kondisi fisik dan harga jual. | Ada di dataset. |
| **Harga (Sale Price)** | Target variabel untuk prediksi. | Ada di dataset Kaggle. |

---
dan masih banyak lagi fitur- fitur lainnya

## 2. Pengambilan Data Menggunakan Kaggle API

1. Menggunakan Kaggle API untuk mengunduh dataset.
2. File hasil unduhan diekstrak ke folder datasets/house_prices.
3. Dataset siap diintegrasikan ke dalam database

## 3. Integrasi Data ke Database
1. Dataset (data.csv) dimuat menggunakan pandas.
2. Membuat database SQLite bernama `house_prices.db`.
3. Data disimpan dalam tabel `houses`.
4. Query dilakukan untuk memastikan data berhasil masuk.