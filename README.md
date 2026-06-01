# Proyek Data Scientist Customer Behavior Prediction

## Business Understanding

<img width="1440" height="816" alt="image" src="https://github.com/user-attachments/assets/ef143979-2263-4d64-86bf-d9da3beb47c7" />

### Latar Belakang 

#### Latar Belakang

## Latar Belakang
Dalam era digital, perusahaan menghasilkan dan menyimpan data transaksi pelanggan dalam jumlah yang sangat besar. Data tersebut tidak hanya berfungsi sebagai catatan aktivitas bisnis, tetapi juga dapat dimanfaatkan untuk memahami perilaku pelanggan secara lebih mendalam. Namun, banyak perusahaan masih menghadapi kesulitan dalam mengidentifikasi karakteristik pelanggan karena seluruh pelanggan sering kali diperlakukan sebagai satu kelompok yang homogen, padahal setiap pelanggan memiliki tingkat aktivitas dan kontribusi yang berbeda terhadap bisnis.

Kurangnya pemahaman mengenai perilaku pelanggan dapat menyebabkan strategi pemasaran yang kurang efektif, seperti pemberian promosi yang tidak tepat sasaran atau penggunaan sumber daya yang tidak optimal. Oleh karena itu, perusahaan perlu melakukan segmentasi pelanggan untuk mengelompokkan pelanggan berdasarkan pola transaksi yang mereka lakukan.

Salah satu pendekatan yang umum digunakan untuk segmentasi pelanggan adalah metode **RFM (Recency, Frequency, Monetary)**. Metode ini memungkinkan perusahaan untuk mengevaluasi pelanggan berdasarkan seberapa baru transaksi terakhir dilakukan (*Recency*), seberapa sering pelanggan bertransaksi (*Frequency*), dan seberapa besar nilai transaksi yang dihasilkan (*Monetary*). Dengan memanfaatkan ketiga indikator tersebut, perusahaan dapat memperoleh gambaran yang lebih jelas mengenai tingkat keterlibatan dan nilai setiap pelanggan.

Pada proyek ini dilakukan segmentasi pelanggan menggunakan teknik clustering berdasarkan atribut RFM untuk mengidentifikasi kelompok pelanggan yang memiliki karakteristik serupa. Hasil segmentasi diharapkan mampu membantu perusahaan memahami perbedaan perilaku pelanggan, mengenali pelanggan yang aktif maupun kurang aktif, serta mendukung penyusunan strategi pemasaran dan program retensi pelanggan yang lebih efektif. Dengan demikian, perusahaan dapat meningkatkan efisiensi pemasaran, mempertahankan pelanggan bernilai tinggi, dan mengoptimalkan pertumbuhan bisnis secara berkelanjutan.

------------------------------

### Permasalahan Bisnis

#### Permasalahan Bisnis yang Akan Diselesaikan

1. **Perusahaan belum memiliki segmentasi pelanggan yang jelas**, sehingga sulit memahami perbedaan karakteristik dan perilaku transaksi antar pelanggan.

2. **Sulit mengidentifikasi pelanggan yang aktif dan memberikan kontribusi transaksi tinggi** dibandingkan pelanggan yang jarang melakukan transaksi.

3. **Strategi pemasaran dan promosi masih berpotensi diterapkan secara seragam kepada seluruh pelanggan**, sehingga kurang efektif dan tidak tepat sasaran.

4. **Perusahaan belum dapat menentukan prioritas pelanggan yang perlu dipertahankan atau ditingkatkan keterlibatannya**, karena belum ada pengelompokan berdasarkan aktivitas dan nilai transaksi.

5. **Kurangnya pemahaman terhadap tingkat loyalitas dan aktivitas pelanggan**, yang dapat menghambat upaya peningkatan retensi pelanggan dan pertumbuhan bisnis.

6. **Diperlukan segmentasi pelanggan berbasis data transaksi menggunakan metode RFM** untuk menghasilkan kelompok pelanggan yang memiliki karakteristik serupa dan mendukung pengambilan keputusan bisnis yang lebih efektif.



------------------------------

### Cakupan Proyek

#### Cakupan Proyek

1. Menggunakan data transaksi pelanggan sebagai sumber utama untuk melakukan analisis segmentasi pelanggan.

2. Melakukan pengolahan data dan pembersihan data (*data preprocessing*) agar data siap digunakan dalam proses analisis.

3. Menghitung metrik **RFM (Recency, Frequency, Monetary)** untuk setiap pelanggan:

   * **Recency**: Jarak waktu sejak transaksi terakhir pelanggan.
   * **Frequency**: Frekuensi transaksi yang dilakukan pelanggan.
   * **Monetary**: Total nilai transaksi yang dihasilkan pelanggan.

4. Melakukan **Exploratory Data Analysis (EDA)** untuk memahami distribusi dan karakteristik nilai RFM pelanggan.

5. Melakukan normalisasi data RFM untuk memastikan setiap variabel memiliki skala yang sebanding dalam proses clustering.

6. Membangun model **K-Means Clustering** untuk mengelompokkan pelanggan berdasarkan kemiripan karakteristik RFM.

7. Menentukan jumlah cluster optimal menggunakan metode evaluasi clustering seperti **Elbow Method** dan **Silhouette Score**.

8. Menganalisis dan menginterpretasikan karakteristik setiap cluster yang terbentuk untuk menghasilkan segmentasi pelanggan yang bermakna secara bisnis.

9. Memberikan rekomendasi bisnis berdasarkan hasil segmentasi pelanggan, seperti strategi retensi, pemasaran, dan peningkatan keterlibatan pelanggan.

### Di luar cakupan proyek

* Prediksi perilaku pelanggan di masa depan.
* Pembangunan model klasifikasi atau prediksi churn pelanggan.
* Implementasi sistem segmentasi secara real-time.
* Deployment model ke lingkungan produksi atau integrasi dengan sistem perusahaan.

------------------------------

### Dataset

**Data source:** https://www.kaggle.com/datasets/vijayuv/onlineretail

## Conclusion

Berdasarkan hasil analisis dan penerapan algoritma **K-Means Clustering** pada data pelanggan yang telah direpresentasikan menggunakan metode **RFM (Recency, Frequency, Monetary)**, diperoleh **2 cluster optimal** yang menggambarkan perbedaan perilaku transaksi pelanggan.

Hasil segmentasi menunjukkan bahwa:

* **Cluster 0 (Inactive Customers)** terdiri dari pelanggan dengan frekuensi transaksi yang lebih rendah dan nilai transaksi yang relatif kecil. Kelompok ini menunjukkan tingkat keterlibatan yang rendah terhadap bisnis sehingga berpotensi memerlukan strategi aktivasi kembali (*re-engagement*).
* **Cluster 1 (Active Customers)** terdiri dari pelanggan yang lebih aktif bertransaksi dan memiliki kontribusi nilai transaksi yang lebih tinggi. Kelompok ini merupakan pelanggan yang lebih bernilai bagi perusahaan dan perlu dipertahankan melalui program loyalitas atau strategi retensi yang tepat.

Secara keseluruhan, proses clustering berhasil mengidentifikasi segmentasi pelanggan berdasarkan perilaku transaksinya. Hasil segmentasi ini dapat membantu perusahaan memahami karakteristik pelanggan dengan lebih baik, menyusun strategi pemasaran yang lebih terarah, meningkatkan efektivitas program retensi pelanggan, serta mendukung pengambilan keputusan bisnis yang berbasis data.
