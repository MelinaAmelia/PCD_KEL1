# PCD_KEL1

# 💵 Deteksi Nominal Uang Kertas dengan Pengolahan Citra Digital  
**Disusun Oleh:**  
- Hopid Saparudin (2106089)  
- Melina Amelia (2206152)  

---
  
# **BAB I**  
## **PENDAHULUAN**

### **1.1 Latar Belakang**  
Dalam kehidupan sehari-hari, mata uang merupakan alat tukar yang sangat penting dalam transaksi ekonomi. Mata uang rupiah, sebagai mata uang resmi Indonesia, terdiri dari berbagai pecahan dengan ciri khas yang berbeda pada setiap nominalnya. Ciri khas ini, berupa angka dan tulisan pada uang kertas, berfungsi sebagai indikator untuk membedakan satu nominal dengan nominal lainnya. Namun, dalam praktiknya, manusia seringkali menghadapi kesulitan dalam membedakan nominal uang rupiah secara cepat, terutama dalam kondisi tertentu, seperti pencahayaan yang buruk, uang yang terlipat, atau rusak. 

Ada banyak mata uang di seluruh dunia tetapi kertasnya berbeda, sama dengan warna dan pola. Ini tidak mudah pekerjaan untuk membedakan berbagai jenis mata uang. Staf yang bekerja untuk perusahaan money changer, perusahaan pembiayaan dll harus mengingat simbol masing-masing mata uang. Ini mungkin menyebabkan beberapa kegagalan atau pengenalan yang salah, sehingga mereka membutuhkan sistem yang akurat, cepat dan andal untuk membantu pekerjaan mereka [1]. 

Salah satu perkembangan teknologi informasi adalah image processing. Image processing atau biasa disebut pengolahan citra digital. Pengolahan citra digital merupakan teknik mengolah citra yang bertujuan memperbaiki kualitas citra agar mudah diinterpretasi oleh manusia atau mesin komputer yang dapat berupa foto maupun gambar bergerak Effendi et al, (2017) . Salah satu ciri untuk menentukan uang asli dengan mendeteksi ada tidaknya watermark pada uang kertas tersrbut. Untuk itu, perlu adanya suatu teknologi yang dapat mengetahui dan mendeteksi watermark pada uang kertas [2].

---

### **1.2 Masalah Penelitian atau Teori Terkait**  
Dalam penelitian sebelumnya oleh Alecia Maharani Ektya Antara, Syafrina Aulia Sari, Nita Riswanti, Dhestyara Alivia Amin, Vebi Verdila, dan Amin Padmo Azam Masa pada tahun 2023. Judul jurnalnya adalah "Deteksi Nominal Rupiah Uang Kertas Berdasarkan Citra Warna Menggunakan Segmentasi K-Means Clustering dan Klasifikasi Random Forest." Hasil dari penelitian ini menunjukkan bahwa model Random Forest yang dibangun memiliki tingkat akurasi mencapai 95% dalam memprediksi nominal rupiah uang kertas dari input gambar [3]

Pada jurnal sebelumya yang disusun oleh Wanda Hamidah dkk, dari Universitas Negeri Makassar, pada tahun 2022 dengan judul "Deteksi Nominal Uang Kertas Menggunakan OCR (Optical Character Recognition)". Hasil dari penelitian ini menunjukkan bahwa metode yang diusulkan berhasil mendeteksi nominal uang kertas dengan akurasi sebesar 94%, di mana dari 70 dataset yang diuji, 66 citra uang kertas terdeteksi dengan tepat dan 4 citra mengalami kesalahan deteksi [4].

Lalu pada jurnal yang disusun oleh Andhika Ryan Pratama, Muhammad Mustajib, dan Aryo Nugroho. Jurnal ini diajukan pada 11 Januari 2020, direvisi pada 18 Maret 2020, dan diterima pada 31 Maret 2020. Judul jurnalnya adalah "Deteksi Citra Uang Kertas dengan Fitur RGB Menggunakan K-Nearest Neighbor". Hasil dari penelitian ini menunjukkan bahwa dari 16 data uji, 15 objek uang kertas berhasil dideteksi dengan benar, menghasilkan akurasi sebesar 93,7% dengan nilai K=5 [5]

Pada penelitian yng disusun oleh Balthasar Kehi, Aryandi Saban, dan Yampi R. Kaesmetan pada tahun 2024 dengan judul "Deteksi Keaslian Uang Kertas Berdasarkan Watermark Dengan Metode Support Vector Machine (SVM)" yang diterbitkan dalam *Jurnal Informatika dan Komputer (JIK)*, vol. 15, no. 1, hal. 31–38. Penelitian ini bertujuan untuk mendeteksi keaslian uang kertas berdasarkan watermark menggunakan metode Canny Edge Detection. Dalam penelitian ini, citra uang kertas yang digunakan terdiri dari berbagai nominal, yakni 1.000, 2.000, 5.000, 10.000, 20.000, 50.000, dan 100.000. Proses deteksi dilakukan dengan melalui beberapa tahapan, seperti akuisisi citra, operasi grayscale, operasi morfologi, dan akhirnya, penerapan Canny Edge Detection. Hasil penelitian menunjukkan bahwa metode Canny Edge Detection mampu mendeteksi watermark pada uang kertas dengan tingkat akurasi sebesar 85,71%, yang mengindikasikan tingkat keberhasilan yang baik dalam menentukan keaslian uang tersebut. [6].

Pada penelitian sebelumya disusun oleh Yeni Nur Hasanah dan Zaehol Fatah dari Universitas Ibrahimy. Jurnal ini diterbitkan pada tahun 2024 dengan judul "Deteksi Keaslian Uang Kertas Berdasarkan Citra Digital Dengan Menggunakan Teachable Machine Learning" [1]. Hasil dari penelitian ini menunjukkan bahwa teachable machine dapat digunakan sebagai alat untuk validasi dataset dengan akurasi yang tinggi pada setiap kelas dataset. Model transfer learning terbaik menggunakan konfigurasi epoch 10, batch size 16, dan learning rate 0.0001, dengan akurasi mencapai 99% untuk beberapa kelas uang kertas [7]

Dibandingkan dengan penelitian sebelumnya yang telah mengidentifikasi gap dalam deteksi nominal uang kertas dengan pengolahan citra digital, penelitian baru ini dibuat bertujuan untuk memperhaharui Deteksi Nominal Uang Kertas Menggunakan OCR (Optical Character Recognition) yang sebelumnya telah diteliti oleh Wanda Hamidah dkk.  yang akan menghasilkan deteksi nominal uang yang lebih akurat dalam memberikan metode yang berbeda yang lebih tepat

---

### **1.3 Tujuan Penelitian**  
Tujuan dari penelitian ini adalah sebagai berikut:  
1. Memperbarui Metode yang digunakan dari hasil penelitian sebelumya oleh Wanda Hamidah dkk.  

---
  
# **BAB II**  
## **METODE**
Penelitian ini menggunakan metode eksperimental. Metode eksperimental merupakan metode yang digunakan untuk mengetahui sebab akibat dari suatu kejadian

![image](https://github.com/user-attachments/assets/bd624cd9-6d42-41be-8518-ce9ce440cbae)

Tahapan yang terdapat dalam Metode Eximental adalah sebagai berikut: 

Pemilihan ide atau topik penelitian, Merumuskan masalah penelitian, merumuskan hipotesis, Menentukan variabel, Menentukan tipe dan desain penelitian, Merancang dan melaksanakan penelitian, Menganalisis hasil penelitian, dan membuat kesimpulan. Adapun dalam pelaksanaan penelitian ini mengacu pada rancangan penelitian yang dapat dilihat pada gambar diatas.

---

  
# **BAB III**  
## **HASIL**


---

  
# **BAB IV**  
## **KESIMPULAN**



## **REFERENSI**
[1] M. Akbar, Awaluddin, A. Sedayu, A. A. Putra, and S. Widyarto, "Original and Counterfeit Money Detection Based on Edge Detection," in *2013 International Conference on Instrumentation, Communication, Information Technology and Biomedical Engineering*, Bandung, Indonesia, Nov. 7–8, 2013. 

[2] A. R. Pambudi, Garno, and Purwantoro, "Deteksi Keaslian Uang Kertas Berdasarkan Watermark dengan Pengolahan Citra Digital," *JIP (Jurnal Informatika Polinema)*, vol. 6, no. 4, pp. 69, Agustus 2020, ISSN: 2614-6371, E-ISSN: 2407-070X. 

[3] A. M. Ektya Antara, S. A. Sari, N. Riswanti, D. A. Amin, V. Verdila, and A. P. A. Masa, "Deteksi Nominal Rupiah Uang Kertas Berdasarkan Citra Warna Menggunakan Segmentasi K-Means Clustering dan Klasifikasi Random Forest," *Kreatif Teknologi dan Sistem Informasi (KRETISI)*, vol. 1, no. 1, Jun. 2023. [Online]. Available: https://doi.org/10.30872/kretisi.v1i1.776
 

[4] W. Hamidah, N. A. P. Hasbullah, T. S. B. Irawan, and A. B. Kaswar, "Deteksi Nominal Uang Kertas Menggunakan OCR (Optical Character Recognition)," *Techno Xplore: Jurnal Ilmu Komputer dan Teknologi Informasi*, vol. 7, no. 2, pp. xx-xx, Oct. 2022. ISSN: 2503-054X.

[5] A. R. Pratama, M. Mustajib, and A. Nugroho, "Deteksi Citra Uang Kertas dengan Fitur RGB Menggunakan K-Nearest Neighbor," *Jurnal Eksplora Informatika*, pp. 163-xx, Mar. 2020.  

[6] B. Kehi, A. Saban, and Y. R. Kaesmetan, "Deteksi Keaslian Uang Kertas Berdasarkan Watermark Dengan Metode Support Vector Machine (SVM)," *Jurnal Informatika dan Komputer (JIK)*, vol. 15, no. 1, pp. 31–38, Jun. 2024. ISSN: 2089-4384. [Online]. Available: sardikehi@gmail.com, andysaban675@gmail.com, kaesmetanyampi@gmail.com

[7] Y. N. Hasanah and Z. Fatah, "Deteksi Keaslian Uang Kertas Berdasarkan Citra Digital Dengan Menggunakan Teachable Machine Learning," *Gudang Jurnal Multidisiplin Ilmu*, vol. 2, no. 12, pp. 44–50, Dec. 2024. [Online]. Available: https://doi.org/10.59435/gjmi.v2i12.1111

---
## 🔍 Tabel Perbandingan


| No | Penulis                                                | Tahun | Judul Jurnal                                                                                      | Metode yang Digunakan                                      | Hasil Penelitian                                                                                 |
|----|--------------------------------------------------------|-------|--------------------------------------------------------------------------------------------------|-----------------------------------------------------------|--------------------------------------------------------------------------------------------------|
| 1  | Alecia Maharani Ektya Antara, Syafrina Aulia Sari, Nita Riswanti, Dhestyara Alivia Amin, Vebi Verdila, Amin Padmo Azam Masa | 2023  | "Deteksi Nominal Rupiah Uang Kertas Berdasarkan Citra Warna Menggunakan Segmentasi K-Means Clustering dan Klasifikasi Random Forest" | Segmentasi K-Means Clustering, Klasifikasi Random Forest   | Model Random Forest mencapai akurasi 95% dalam memprediksi nominal rupiah uang kertas dari input gambar |
| 2  | Wanda Hamidah dkk, Universitas Negeri Makassar         | 2022  | "Deteksi Nominal Uang Kertas Menggunakan OCR (Optical Character Recognition)"                   | Optical Character Recognition (OCR)                       | Metode berhasil mendeteksi nominal uang kertas dengan akurasi 94%, 66 dari 70 citra terdeteksi dengan tepat |
| 3  | Andhika Ryan Pratama, Muhammad Mustajib, Aryo Nugroho  | 2020  | "Deteksi Citra Uang Kertas dengan Fitur RGB Menggunakan K-Nearest Neighbor"                      | Fitur RGB, K-Nearest Neighbor                              | 15 dari 16 objek uang kertas berhasil dideteksi dengan akurasi 93,7% menggunakan nilai K=5         |
| 4  | Balthasar Kehi, Aryandi Saban, Yampi R. Kaesmetan      | 2024  | "Deteksi Keaslian Uang Kertas Berdasarkan Watermark Dengan Metode Support Vector Machine (SVM)"  | Canny Edge Detection, Support Vector Machine (SVM)         | Akurasi 85,71% dalam mendeteksi watermark pada uang kertas untuk menentukan keaslian              |
| 5  | Yeni Nur Hasanah, Zaehol Fatah, Universitas Ibrahimy   | 2024  | "Deteksi Keaslian Uang Kertas Berdasarkan Citra Digital Dengan Menggunakan Teachable Machine Learning" | Teachable Machine Learning                                | Akurasi 99% dengan model transfer learning terbaik, menggunakan epoch 10, batch size 16, dan learning rate 0.0001 |


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

### Referensi

[1] M. Akbar, Awaluddin, A. Sedayu, A. A. Putra, and S. Widyarto, "Original and Counterfeit Money Detection Based on Edge Detection," in *2013 International Conference on Instrumentation, Communication, Information Technology and Biomedical Engineering*, Bandung, Indonesia, Nov. 7–8, 2013. [Online]. Available: E-mail: muh_akbar@yahoo.com, swidyarto@unisel.edu.my.

[2] A. R. Pambudi, Garno, and Purwantoro, "Deteksi Keaslian Uang Kertas Berdasarkan Watermark dengan Pengolahan Citra Digital," *JIP (Jurnal Informatika Polinema)*, vol. 6, no. 4, pp. 69, Agustus 2020, ISSN: 2614-6371, E-ISSN: 2407-070X. 

[3] N. Yasmeen, S. Nida, N. Fathima, M. Aftab, and N. R. Deepak, "A Review on Fake Currency Detection using Feature Extraction," *International Journal of Modern Developments in Engineering and Science*, vol. 1, no. 5, pp. xx-xx, May 2022. ISSN: 2583-3138. 

[4] W. Hamidah, N. A. P. Hasbullah, T. S. B. Irawan, and A. B. Kaswar, "Deteksi Nominal Uang Kertas Menggunakan OCR (Optical Character Recognition)," *Techno Xplore: Jurnal Ilmu Komputer dan Teknologi Informasi*, vol. 7, no. 2, pp. xx-xx, Oct. 2022. ISSN: 2503-054X.

[5] A. R. Pratama, M. Mustajib, and A. Nugroho, "Deteksi Citra Uang Kertas dengan Fitur RGB Menggunakan K-Nearest Neighbor," *Jurnal Eksplora Informatika*, pp. 163-xx, Mar. 2020.  

[6] A. Jalil, "Sistem kontrol deteksi nominal uang kertas rupiah menggunakan image processing Raspberry Pi," *Jurnal IT*, vol. 14, STMIK Handayani, Mar. 2014.  

[7] D. Galeana-Pérez and E. Bayro-Corrochano, "Recognition system for Euro and Mexican banknotes based on deep learning with real scene images," *Computación y Sistemas*, vol. 22, no. 4, pp. 1065–1076, 2018, doi: 10.13053/CyS-22-4-3079.  


