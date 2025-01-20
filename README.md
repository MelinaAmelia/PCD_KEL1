# PCD_KEL1

# 💵 Deteksi Keaslian Uang Kertas dengan Pengolahan Citra Digital  
**Disusun Oleh:**  
- Hofid (2106 _ _ _)  
- Melina Amelia (2206152)  

---
  
# **BAB I**  
## **PENDAHULUAN**

### **1.1 Latar Belakang**  
Di era globalisasi dan transformasi digital yang semakin pesat, pemalsuan uang kertas menjadi salah satu masalah yang meresahkan masyarakat dan pemerintah. Pemalsuan uang tidak hanya mengancam stabilitas ekonomi, tetapi juga menimbulkan kerugian besar bagi pelaku usaha dan masyarakat umum. Dalam skala global, organisasi kriminal menggunakan teknologi canggih untuk menciptakan replika uang kertas yang sulit dibedakan dengan mata telanjang.  
Ada banyak mata uang di seluruh dunia tetapi kertasnya berbeda, sama dengan warna dan pola. Ini tidak mudah pekerjaan untuk membedakan berbagai jenis mata uang. Staf yang bekerja untuk perusahaan money changer, perusahaan pembiayaan dll harus mengingat simbol masing-masing mata uang. Ini mungkin menyebabkan beberapa kegagalan atau pengenalan yang salah, sehingga mereka membutuhkan sistem yang akurat, cepat dan andal untuk membantu pekerjaan mereka [1]. 

Salah satu perkembangan teknologi informasi adalah image processing. Image processing atau biasa disebut pengolahan citra digital. Pengolahan citra digital merupakan teknik mengolah citra yang bertujuan memperbaiki kualitas citra agar mudah diinterpretasi oleh manusia atau mesin komputer yang dapat berupa foto maupun gambar bergerak Effendi et al, (2017) . Salah satu ciri untuk menentukan uang asli dengan mendeteksi ada tidaknya watermark pada uang kertas tersrbut. Untuk itu, perlu adanya suatu teknologi yang dapat mengetahui dan mendeteksi watermark pada uang kertas [2].

---

### **1.2 Rumusan Masalah**  
Beberapa masalah yang menjadi fokus penelitian dalam deteksi keaslian uang kertas adalah:  
1. Bagaimana membedakan fitur uang asli dengan uang palsu secara otomatis menggunakan pengolahan citra digital?  
2. Bagaimana efektivitas metode **Canny Edge Detection** dalam mendeteksi watermark pada uang kertas?  
3. Bagaimana mengembangkan sistem yang efisien dan mudah digunakan untuk memeriksa keaslian uang secara real-time?  
4. Bagaimana meningkatkan akurasi deteksi untuk berbagai denominasi uang kertas dalam berbagai kondisi pencahayaan?  

---

### **1.3 Tujuan Penelitian**  
Tujuan dari penelitian ini adalah sebagai berikut:  
1. Mengembangkan sistem deteksi keaslian uang kertas menggunakan metode pengolahan citra digital.  
2. Mengukur tingkat akurasi metode **Canny Edge Detection** untuk mendeteksi fitur keamanan pada uang kertas.  
3. Merancang solusi yang dapat mendukung deteksi otomatis dengan biaya rendah dan efisiensi tinggi.  
4. Menyediakan teknologi yang mampu beradaptasi dengan tantangan masa depan, termasuk perkembangan teknik pemalsuan.  

---

### **1.4 Manfaat Penelitian**  
Manfaat dari penelitian ini meliputi:  
1. Memberikan kontribusi pada pengembangan teknologi keamanan finansial.  
2. Membantu masyarakat umum dan lembaga keuangan dalam memerangi pemalsuan uang.  
3. Meningkatkan literasi teknologi pada bidang pengolahan citra digital dan aplikasinya dalam kehidupan sehari-hari.  
4. Menunjukkan potensi pengolahan citra digital sebagai solusi yang adaptif dan inovatif untuk berbagai masalah dunia nyata.  

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

### Referensi

[1] M. Akbar, Awaluddin, A. Sedayu, A. A. Putra, and S. Widyarto, "Original and Counterfeit Money Detection Based on Edge Detection," in *2013 International Conference on Instrumentation, Communication, Information Technology and Biomedical Engineering*, Bandung, Indonesia, Nov. 7–8, 2013. [Online]. Available: E-mail: muh_akbar@yahoo.com, swidyarto@unisel.edu.my.

[2] A. R. Pambudi, Garno, and Purwantoro, "Deteksi Keaslian Uang Kertas Berdasarkan Watermark dengan Pengolahan Citra Digital," *JIP (Jurnal Informatika Polinema)*, vol. 6, no. 4, pp. 69, Agustus 2020, ISSN: 2614-6371, E-ISSN: 2407-070X. [Online]. Available: https://doi.org/example.


