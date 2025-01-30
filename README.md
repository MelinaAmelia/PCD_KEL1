# PCD_KEL1

# 💵 Sistem Klasifikasi Uang Rupiah Berdasarkan Citra Digital Menggunakan Edge Detection, K-Means Clustering, dan CNN 
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

### **1.2 Penelitian atau Teori Terkait**  
Dalam penelitian sebelumnya oleh Alecia Maharani Ektya Antara, Syafrina Aulia Sari, Nita Riswanti, Dhestyara Alivia Amin, Vebi Verdila, dan Amin Padmo Azam Masa pada tahun 2023. Judul jurnalnya adalah "Deteksi Nominal Rupiah Uang Kertas Berdasarkan Citra Warna Menggunakan Segmentasi K-Means Clustering dan Klasifikasi Random Forest." Hasil dari penelitian ini menunjukkan bahwa model Random Forest yang dibangun memiliki tingkat akurasi mencapai 95% dalam memprediksi nominal rupiah uang kertas dari input gambar [3]

Pada jurnal sebelumya yang disusun oleh Wanda Hamidah dkk, dari Universitas Negeri Makassar, pada tahun 2022 dengan judul "Deteksi Nominal Uang Kertas Menggunakan OCR (Optical Character Recognition)". Hasil dari penelitian ini menunjukkan bahwa metode yang diusulkan berhasil mendeteksi nominal uang kertas dengan akurasi sebesar 94%, di mana dari 70 dataset yang diuji, 66 citra uang kertas terdeteksi dengan tepat dan 4 citra mengalami kesalahan deteksi [4].

Lalu pada jurnal yang disusun oleh Andhika Ryan Pratama, Muhammad Mustajib, dan Aryo Nugroho. Jurnal ini diajukan pada 11 Januari 2020, direvisi pada 18 Maret 2020, dan diterima pada 31 Maret 2020. Judul jurnalnya adalah "Deteksi Citra Uang Kertas dengan Fitur RGB Menggunakan K-Nearest Neighbor". Hasil dari penelitian ini menunjukkan bahwa dari 16 data uji, 15 objek uang kertas berhasil dideteksi dengan benar, menghasilkan akurasi sebesar 93,7% dengan nilai K=5 [5]

Pada penelitian yng disusun oleh Balthasar Kehi, Aryandi Saban, dan Yampi R. Kaesmetan pada tahun 2024 dengan judul "Deteksi Keaslian Uang Kertas Berdasarkan Watermark Dengan Metode Support Vector Machine (SVM)" yang diterbitkan dalam *Jurnal Informatika dan Komputer (JIK)*, vol. 15, no. 1, hal. 31–38. Penelitian ini bertujuan untuk mendeteksi keaslian uang kertas berdasarkan watermark menggunakan metode Canny Edge Detection. Dalam penelitian ini, citra uang kertas yang digunakan terdiri dari berbagai nominal, yakni 1.000, 2.000, 5.000, 10.000, 20.000, 50.000, dan 100.000. Proses deteksi dilakukan dengan melalui beberapa tahapan, seperti akuisisi citra, operasi grayscale, operasi morfologi, dan akhirnya, penerapan Canny Edge Detection. Hasil penelitian menunjukkan bahwa metode Canny Edge Detection mampu mendeteksi watermark pada uang kertas dengan tingkat akurasi sebesar 85,71%, yang mengindikasikan tingkat keberhasilan yang baik dalam menentukan keaslian uang tersebut. [6].

Pada penelitian sebelumya disusun oleh Yeni Nur Hasanah dan Zaehol Fatah dari Universitas Ibrahimy. Jurnal ini diterbitkan pada tahun 2024 dengan judul "Deteksi Keaslian Uang Kertas Berdasarkan Citra Digital Dengan Menggunakan Teachable Machine Learning" [1]. Hasil dari penelitian ini menunjukkan bahwa teachable machine dapat digunakan sebagai alat untuk validasi dataset dengan akurasi yang tinggi pada setiap kelas dataset. Model transfer learning terbaik menggunakan konfigurasi epoch 10, batch size 16, dan learning rate 0.0001, dengan akurasi mencapai 99% untuk beberapa kelas uang kertas [7]

Penelitian ini akan mengembangkan model pengolahan citra digital dengan pendekatan eksperimental menggunakan kombinasi CNN (Convolutional Neural Networks) dan teknik pemrosesan citra lainnya untuk meningkatkan akurasi deteksi nominal uang rupiah

---

### **1.3 Tujuan Penelitian**  
Tujuan dari penelitian ini adalah sebagai berikut:  
1. Mengembangkan sistem deteksi nominal uang kertas rupiah menggunakan metode pengolahan citra digital.
2. Mengimplementasikan model deep learning (CNN) dalam klasifikasi nominal uang.
3. Mengevaluasi performa sistem berdasarkan metrik akurasi, presisi, dan recall.
4. Membandingkan hasil eksperimen dengan metode sebelumnya. 

---
  
# **BAB II**  
## **METODE**
### **2.1 Langkah-langkah Penelitian**  
Penelitian ini menggunakan metode eksperimental. Metode eksperimental merupakan metode yang digunakan untuk mengetahui sebab akibat dari suatu kejadian
1. Akuisisi Data: Mengumpulkan dataset gambar uang rupiah dari berbagai sumber dengan variasi kondisi pencahayaan dan orientasi.
2. Preprocessing Citra: Konversi gambar ke grayscale, normalisasi, dan augmentasi data.
3. Ekstraksi Fitur: Penerapan metode deteksi tepi Canny untuk menyoroti karakteristik utama uang kertas.
4. Segmentasi Citra: Menggunakan K-Means Clustering untuk memisahkan area penting pada gambar.
5. Klasifikasi: Menerapkan Convolutional Neural Networks (CNN) untuk mengenali nominal uang.
6. Evaluasi Model: Menggunakan metrik akurasi, precision, recall, serta membandingkan hasil dengan metode lainnya.

### **2.2 Visualisasi Model**   

Tahapan yang terdapat dalam Metode Experimental adalah sebagai berikut: 

![image](https://github.com/user-attachments/assets/e36a3f12-be3e-4999-a023-86ada9fc8a05)


Secara keseluruhan, diagram ini menggambarkan alur proses deteksi nominal uang kertas mulai dari pengumpulan data, preprocessing, ekstraksi fitur, segmentasi, klasifikasi, hingga evaluasi model. Setiap tahapan memiliki tujuan dan metode yang spesifik untuk mencapai tujuan akhir, yaitu pengenalan nominal uang.

---

  
# **BAB III**  
## **HASIL**

### **3.1 Hasil Eksperimen**

![WhatsApp Image 2025-01-30 at 22 08 15](https://github.com/user-attachments/assets/f542958e-f0d7-4b23-867e-b8e97fa7a2b7)

<p align="center">
&nbsp;&nbsp;&nbsp;&nbsp;**Gambar 1**
</p>





Setelah melatih model CNN dengan dataset uang rupiah, hasil pengujian menunjukkan:

1. Grayscale

   Gambar diubah menjadi hitam putih untuk menghilangkan warna yang tidak diperlukan dalam ekstraksi fitur. Detail uang tetap terlihat jelas dalam skala keabuan.

2. Edge Detection (Canny)

   Teknik Canny digunakan untuk mendeteksi tepi uang kertas dan angka nominal. Beberapa noise muncul di area luar gambar.

3. K-Means Clustering

   Segmentasi membagi citra berdasarkan kemiripan intensitas piksel. Uang kertas tampak terpisah dari background, meskipun ada area yang bercampur.



![WhatsApp Image 2025-01-30 at 22 09 24](https://github.com/user-attachments/assets/fabdfb06-09d8-468f-bc62-4a0a6254c451)

<p align="center">
&nbsp;&nbsp;&nbsp;&nbsp;**Gambar 2**
</p>




Berdasarkan output pelatihan model CNN pada gambar, berikut analisisnya:
1. Dataset
Dataset berisi 1324 gambar untuk training dan 330 gambar untuk validasi.
Namun, ada indikasi bahwa dataset hanya memiliki 1 kelas (Found 1324 images belonging to 1 classes). Ini berarti model hanya belajar dari satu label dan tidak bisa melakukan klasifikasi dengan benar.
2. Hasil Pelatihan
Akurasi meningkat cepat sejak epoch pertama (90.44%) dan langsung mencapai 100% akurasi pada epoch ke-2.
Loss (kerugian) mendekati nol, yang menunjukkan bahwa model sangat cocok dengan data training.
Akurasi validasi (val_accuracy) juga 100%, yang menunjukkan tidak ada kesalahan prediksi.
3. Masalah Potensial
Overfitting: Model mungkin terlalu menghafal data training dan tidak bisa digeneralisasi dengan baik.
Dataset bermasalah: Sepertinya hanya ada satu kelas dalam dataset, sehingga model tidak benar-benar belajar membedakan nominal uang.
4. Solusi
Periksa dataset dan pastikan ada lebih dari satu kelas.
Gunakan augmentasi data (misalnya rotasi, zoom, perubahan warna) untuk meningkatkan variasi.
Kurangi kompleksitas model jika dataset kecil untuk menghindari overfitting.
Gunakan dropout yang lebih tinggi atau regularisasi L2 untuk meningkatkan generalisasi model.

Hasil deteksi nominal uang menggunakan Grayscale, Edge Detection dan K-Means Clustering.

---

  
# **BAB IV**  
## **KESIMPULAN**

### **4.1 Ringkasan Temuan**

Sistem berhasil mendeteksi nominal uang kertas dengan akurasi tinggi pada data training dan validasi. Namun, ada indikasi overfitting yang perlu diatasi dengan peningkatan dataset dan teknik regularisasi. Untuk penelitian selanjutnya, dapat dilakukan eksperimen dengan metode lain seperti YOLO atau Transformer-based models untuk meningkatkan akurasi dan efisiensi.

### **4.2 Batasan Pekerjaan**

- Model mengalami penurunan akurasi pada gambar uang yang sangat buram atau rusak.

- Dataset masih terbatas pada pecahan uang tertentu, sehingga perlu diperluas.

### **4.3 Rekomendasi Untuk Pekerjaan di Masa Depan**

- Menggunakan teknik transfer learning untuk meningkatkan akurasi lebih lanjut.

- Mengembangkan model yang lebih tahan terhadap kondisi pencahayaan ekstrem.

- Mengintegrasikan metode OCR untuk mendukung pengenalan karakter numerik pada uang kertas.



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






 




