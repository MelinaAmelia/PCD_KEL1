# PCD_KEL1
Analisis Jurnal
# 💵 Analisis Penelitian: Deteksi Keaslian Uang Kertas dengan Pengolahan Citra Digital  

---

## 📌 Pendahuluan  
Penelitian ini berfokus pada **deteksi keaslian uang kertas** menggunakan metode **pengolahan citra digital**, dengan teknik utama **deteksi tepi Canny**. Dua dokumen analisis dibandingkan untuk menggambarkan pendekatan yang berbeda dalam mendeteksi watermark dan uang palsu.  

---
## 🔍 Ringkasan Penelitian  

### 🗂 File 1: Deteksi Watermark dengan Pengolahan Citra Digital  
- **Metode Utama**: Deteksi tepi **Canny**, operasi morfologi, dan binarisasi.  
- **Tahapan Penelitian**:  
  1. Konversi gambar ke skala abu-abu.  
  2. Operasi morfologi untuk mempertegas fitur gambar.  
  3. Deteksi watermark menggunakan tepi Canny.  
- **Dataset**: 21 gambar uang kertas dengan denominasi 1.000 hingga 100.000.  
- **Hasil**: Tingkat keberhasilan deteksi sebesar **85,71%**.  
- **Rekomendasi**:  
  - Penggunaan gambar langsung dari webcam.  
  - Pengujian pada skenario lebih kompleks.  

---

### 🗂 File 2: Deteksi Mata Uang Palsu India dengan Pemrosesan Citra  
Berdasarkan keterangan dari jurnal ini, berikut adalah penjelasan mengenai deteksi mata uang palsu India menggunakan teknik pemrosesan citra:  

1. **Tujuan dan Signifikansi**:  
   - Jurnal ini menyoroti pentingnya deteksi mata uang palsu untuk menjaga stabilitas ekonomi.  
   - Pemalsuan uang dapat merusak kepercayaan masyarakat terhadap sistem moneter dan menyebabkan kerugian ekonomi yang signifikan.  

2. **Fitur Keamanan**:  
   - Penelitian ini mengidentifikasi berbagai fitur keamanan pada uang kertas India yang digunakan untuk mendeteksi keaslian, seperti:  
     - Benang keamanan.  
     - Watermark.  
     - Micro-lettering.  
     - Cetakan intaglio.  

3. **Teknik Pemrosesan Citra**:  
   - Sistem yang diusulkan menggunakan teknik pemrosesan citra untuk membedakan antara uang asli dan palsu.  
   - Dengan mencapai akurasi **100%**, sistem ini menunjukkan potensi besar untuk digunakan oleh masyarakat umum dalam mendeteksi uang palsu.  

4. **Relevansi Historis**:  
   - Penelitian ini mengakui bahwa pemalsuan uang telah menjadi masalah sejak zaman kuno.  
   - Ini menunjukkan bahwa tantangan ini terus berlanjut dan memerlukan solusi yang efektif.  

5. **Pengembangan di Masa Depan**:  
   - Penelitian di masa depan akan berfokus pada peningkatan kecepatan dan akurasi deteksi dengan menggunakan algoritma pemrosesan citra yang lebih canggih.  
   - Ini menunjukkan komitmen untuk terus memperbaiki sistem deteksi seiring dengan perkembangan teknologi.  

**Kesimpulan**:  
Jurnal ini memberikan kontribusi penting dalam bidang deteksi mata uang palsu dengan menawarkan solusi yang akurat dan dapat diakses oleh masyarakat luas. Namun, untuk implementasi yang lebih luas, penelitian lebih lanjut diperlukan untuk memastikan sistem ini dapat berfungsi secara efektif dalam berbagai kondisi dan dengan berbagai jenis uang kertas.  

---

## 📊 Analisis Komparatif  

| **Aspek**                 | **File 1**                                                    | **File 2**                                                       |  
|---------------------------|--------------------------------------------------------------|-------------------------------------------------------------------|  
| **Fokus Penelitian**      | Deteksi watermark pada uang kertas.                          | Deteksi mata uang palsu India berdasarkan fitur keamanan.         |  
| **Metode Utama**          | Deteksi tepi (Canny) + operasi morfologi.                    | Deteksi fitur keamanan + algoritma pemrosesan citra.             |  
| **Keberhasilan**          | 85,71% berhasil mendeteksi watermark.                        | Akurasi mencapai 100%.                                           |  
| **Dataset**               | 21 gambar uang dari denominasi 1.000 hingga 100.000.         | Uang kertas India dengan berbagai fitur keamanan.                |  
| **Rekomendasi Masa Depan**| Penggunaan gambar dari webcam dan pengujian lebih beragam.   | Peningkatan algoritma untuk akurasi dan kecepatan lebih tinggi.  |  

---

## 📈 Kesimpulan  

Kedua pendekatan memberikan kontribusi signifikan dalam **deteksi keaslian uang kertas**:  
1. **File 1** menekankan keunggulan metode deteksi watermark.  
2. **File 2** menyoroti pentingnya fitur keamanan dalam mendeteksi uang palsu.  
