# Laporan Proyek Credit Risk Prediction - Syahvan Alviansyah Diva Ritonga

## Domain Proyek

Dalam industri finansial, penilaian risiko kredit adalah salah satu aspek yang sangat penting. Hal ini karena risiko kredit merupakan faktor utama yang mempengaruhi kesehatan keuangan sebuah perusahaan. Pemberian  kredit  dapat  mengalami  berbagai  masalah ataupun  risiko.  Permasalahan  atau  risiko  yang  dapat  dialami dalam  pemberian  kredit  adalah sikap  nasabah  yang  tidak  melakukan  pembayaran angsuran   secara   tepat   waktu   ataupun   menunda pembayaran  sampai  beberapa  bulan  pembayaran angsuran  yang  menyebabkan  terjadinya  kredit  macet (Hasan, 2017). Dalam konteks ini, Credit Risk Prediction memainkan peran kunci dalam membantu perusahaan finansial dalam membuat keputusan pemberian pinjaman yang lebih baik. Melalui analisis data historis pinjaman, perusahaan dapat mengidentifikasi pola-pola yang berkaitan dengan pelunasan pinjaman dan mengembangkan model prediksi untuk memproyeksikan kemungkinan seorang peminjam untuk melunasi pinjaman di masa depan.

## Business Understanding

### Problem Statements

Berdasarkan latar belakang di atas, berikut ini batasan masalah yang dapat diselesaikan dengan proyek ini:
- Bagaimana mengembangkan model prediksi yang dapat memproyeksikan kemungkinan seorang peminjam untuk melunasi pinjaman di masa depan?
- Bagaimana meningkatkan keputusan pemberian pinjaman dengan mengurangi risiko kredit yang tidak diinginkan?
- Bagaimana cara menentukan hasil prediksi suatu Algoritma Machine Learning dapat dikatakan baik?

### Goals

Menjelaskan tujuan dari pernyataan masalah:
- Mengembangkan model prediksi risiko kredit yang memiliki akurasi tinggi.
- Mengurangi tingkat risiko kredit yang tidak diinginkan dalam keputusan pemberian pinjaman.
- Melakukan evaluasi terhadap metrik dari masing-masing algoritma.

### Solution statements

- Melakukan pemodelan menggunakan beberapa algoritma machine learning seperti XGBoost dan Random Forest untuk mencapai solusi yang diinginkan.
- Melakukan evaluasi model menggunakan classification report, AUC-ROC, dan Kolmogorov-Smirnov.

## Data Understanding
Dataset yang digunakan merupakan data credit dari tahun 2007-2014 yang berasal dari [LendingClub](https://www.kaggle.com/datasets/devanshi23/loan-data-2007-2014), sebuah perusahaan Peer-to-Peer (P2P) Lending yang berbasis di Amerika Serikat. Dataset tersebut berisi 466285 baris dan 74 kolom.

### Variabel-variabel pada Dataset LendingClub adalah sebagai berikut:
- `id`: ID unik yang ditetapkan LC untuk daftar pinjaman. 
- `member_id`: Id unik yang ditetapkan untuk anggota peminjam.
- `loan_amnt`: Jumlah pinjaman yang tercantum yang diajukan oleh peminjam. Jika suatu saat departemen kredit mengurangi jumlah pinjaman, maka hal itu akan tercermin dalam nilai ini.
- `funded_amnt`: Jumlah total yang berkomitmen untuk pinjaman tersebut pada saat itu.
- `funded_amnt_inv`: Jumlah total yang berkomitmen oleh investor untuk pinjaman tersebut pada saat itu.
- `term`: Jumlah pembayaran pinjaman. Nilai dalam bulan dan dapat berupa 36 atau 60.          
- `int_rate`: Suku Bunga pinjaman
- `installment`: Pembayaran bulanan yang harus dibayar oleh peminjam jika pinjaman itu berasal.
- `grade`: LC menetapkan tingkat pinjaman               
- `sub_grade`: LC menetapkan tanah dasar pinjaman           
- `emp_title`: Jabatan yang diberikan oleh Peminjam saat mengajukan pinjaman.                    
- `emp_length`: Lamanya masa kerja dalam tahun. Nilai yang mungkin adalah antara 0 dan 10 dimana 0 berarti kurang dari satu tahun dan 10 berarti sepuluh tahun atau lebih.
- `home_ownership`: Status kepemilikan rumah yang diberikan oleh peminjam pada saat pendaftaran. Nilai-nilai: SEWA, SENDIRI, KPR, LAINNYA.      
- `annual_inc`: Pendapatan tahunan yang dilaporkan sendiri yang diberikan oleh peminjam saat pendaftaran.
- `verification_status`: Status verifikasi.
- `issue_d`: Bulan dimana pinjaman itu didanai.            
- `loan_status`: Status pinjaman saat ini.         
- `pymnt_plan`: Menunjukkan apakah rencana pembayaran telah diterapkan untuk pinjaman      
- `url`: URL untuk halaman LC dengan data daftar.
- `desc`: Deskripsi pinjaman yang diberikan oleh peminjam.
- `purpose`: Kategori yang disediakan oleh peminjam untuk permintaan pinjaman.             
- `title`: Judul pinjaman yang diberikan oleh peminjam.
- `zip_code`            
- `addr_state`          
- `dti`             
- `delinq_2yrs`     
- `earliest_cr_line`             466256 non-null  object 
- `inq_last_6mths`  
- `mths_since_last_delinq`       215934 non-null  float64
- `mths_since_last_record`       62638 non-null   float64
- `open_acc`        
 31  `pub_rec`         
 32  `revol_bal`                    466285 non-null  int64  
 33  `revol_util`                   465945 non-null  float64
 34  `total_acc`       
 35  `initial_list_status` 
 36  `out_prncp`       
 37  `out_prncp_inv`   
 38  `total_pymnt`     
 39  `total_pymnt_inv` 
 40  `total_rec_prncp` 
 41  `total_rec_int`   
 42  `total_rec_late_fee`           466285 non-null  float64
 43  `recoveries`      
 44  `collection_recovery_fee`      466285 non-null  float64
 45  `last_pymnt_d`                 465909 non-null  object 
 46  `last_pymnt_amnt` 
 47  `next_pymnt_d`                 239071 non-null  object 
 48  `last_credit_pull_d`           466243 non-null  object 
 49  `collections_12_mths_ex_med`   466140 non-null  float64
 50  `mths_since_last_major_derog`  98974 non-null   float64
 51  `policy_code`                  466285 non-null  int64  
 52  `application_type`    
 53  `annual_inc_joint`    
 54  `dti_joint`   
 55  `verification_status_joint` 
 56  `acc_now_delinq`  
 57  `tot_coll_amt`      
 58  `tot_cur_bal`       
 59  `open_acc_6m` 
 60  `open_il_6m`  
 61  `open_il_12m` 
 62  `open_il_24m` 
 63  `mths_since_rcnt_il`  
 64  `total_bal_il`
 65  `il_util`     
 66  `open_rv_12m` 
 67  `open_rv_24m` 
 68  `max_bal_bc`  
 69  `all_util`    
 70  `total_rev_hi_lim`  
 71  `inq_fi`      
 72  `total_cu_tl` 
 73  `inq_last_12m`


## Data Preparation
Dalam data preparation, prinsip "garbage in, garbage out" berlaku. Artinya, jika data yang digunakan untuk melatih model tidak berkualitas baik, maka hasil prediksi dari model tersebut juga akan tidak akurat atau tidak dapat diandalkan. Dengan memastikan data yang digunakan untuk melatih model memiliki kualitas yang baik, kita dapat menghasilkan model yang lebih andal dalam memprediksi risiko kredit.

Proses data preparation meliputi:
- Pembuangan fitur-fitur yang tidak berguna. Contohnya seperti fitur yang merupakan id unik, berupa free text, nilainya kosong semua (NULL), dsb.
- Pembersihan data untuk menangani nilai yang hilang atau tidak lengkap.
- Pemrosesan data seperti pengkodean variabel kategorikal menggunakan one hot encoding.
- Penskalaan fitur numerik menggunakan standard scaler untuk memastikan skala yang seragam.
- Pembagian dataset yang ada menjadi 2 bagian yaitu data latih dan data uji dengan rasio 80:20. 

## Modeling
Untuk tahap pemodelan, saya menggunakan dua algoritma machine learning, yaitu XGBoost dan Random Forest. Berikut adalah penjelasan singkat mengenai kedua algoritma tersebut:

### 1. XGBoost (Extreme Gradient Boosting)

XGBoost (Extreme Gradient Boosting) adalah algoritma ensemble yang kuat dan efisien yang sering digunakan dalam kompetisi data dan aplikasi produksi. Beberapa parameter yang dapat digunakan dalam pemodelan XGBoost ini adalah:
- `learning_rate`: Menentukan seberapa besar update yang akan dilakukan pada nilai prediksi setiap kali ada iterasi.
- `max_depth`: Menentukan kedalaman maksimum dari setiap pohon dalam ensemble.
- `n_estimators`: Menentukan jumlah pohon keputusan yang akan dibangun.
- `gamma`: Menentukan minimum penurunan kerugian yang diperlukan untuk melakukan pemisahan tambahan pada simpul pohon.
- `subsample`: Menentukan fraksi sampel yang akan digunakan dalam setiap iterasi.
- `colsample_bytree`: Menentukan fraksi kolom yang akan digunakan dalam setiap iterasi untuk membangun setiap pohon.

Kelebihan XGBoost adalah kemampuannya dalam menangani dataset besar dengan cepat, toleran terhadap overfitting, dan memiliki fleksibilitas dalam menangani berbagai jenis data. Namun, kelemahannya adalah rentan terhadap overfitting jika parameter tidak disetel dengan benar.

### 2. Random Forest

Random Forest adalah algoritma ensemble lain yang sangat populer. Algoritma ini bekerja dengan membangun sejumlah besar pohon keputusan selama pelatihan dan menggabungkan hasil prediksi dari setiap pohon untuk menghasilkan prediksi akhir. Beberapa parameter yang dapat digunakan dalam pemodelan Random Forest ini adalah:
- `n_estimators`: Menentukan jumlah pohon keputusan yang akan dibangun.
- `max_depth`: Menentukan kedalaman maksimum dari setiap pohon.
- `min_samples_split`: Menentukan jumlah sampel minimum yang diperlukan untuk membagi simpul internal.
- `min_samples_leaf`: Menentukan jumlah sampel minimum yang diperlukan untuk menjadi simpul daun.
- `max_features`: Menentukan jumlah fitur yang akan dipertimbangkan saat mencari split terbaik.

Kelebihan dari Random Forest adalah kemampuannya dalam menangani data yang tidak seimbang dan rentan terhadap overfitting. Namun, kelemahannya adalah model yang dihasilkan tidak mudah diinterpretasi dibandingkan dengan model linear.

Pemilihan model terbaik antara XGBoost dan Random Forest biasanya bergantung pada karakteristik dataset dan tujuan pemodelan. Dalam kasus ini, setelah melakukan eksperimen dan validasi menggunakan kedua model, saya memilih XGBoost sebagai model terbaik karena kinerjanya yang lebih unggul dalam memprediksi risiko kredit berdasarkan metrik evaluasi yang telah ditetapkan. XGBoost memberikan hasil yang lebih tinggi dalam hal akurasi, presisi, recall, dan AUC-ROC dibandingkan dengan Random Forest pada dataset dan konteks proyek ini.

## Evaluation
### Metrik Evaluasi

Dalam proyek ini, kami menggunakan beberapa metrik evaluasi yang sesuai dengan konteks klasifikasi pada model prediksi risiko kredit. Berikut adalah penjelasan singkat mengenai metrik-metrik yang digunakan:

1. **Akurasi (Accuracy)**:
   Akurasi mengukur seberapa tepat model dalam memprediksi keseluruhan kelas yang benar. Metrik ini dihitung sebagai rasio prediksi benar (positif dan negatif) dengan total sampel.
   
   $$\text{Accuracy} = \frac{\text{TP} + \text{TN}}{\text{TP} + \text{TN} + \text{FP} + \text{FN}}$$

2. **Presisi (Precision)**:
   Presisi mengukur seberapa tepat model dalam memprediksi kelas positif. Metrik ini dihitung sebagai rasio prediksi benar positif (TP) dengan total prediksi positif (TP + FP).
   
   $$\text{Precision} = \frac{\text{TP}}{\text{TP} + \text{FP}}$$

3. **Recall (Sensitivitas)**:
   Recall mengukur seberapa baik model dalam menemukan kembali semua instansi kelas positif. Metrik ini dihitung sebagai rasio prediksi benar positif (TP) dengan total kelas positif yang sebenarnya (TP + FN).
   
   $$\text{Recall} = \frac{\text{TP}}{\text{TP} + \text{FN}}$$

4. **F1 Score**:
   F1 score adalah rata-rata harmonis dari presisi dan recall. Metrik ini memberikan keseimbangan antara presisi dan recall.
   
   $$\text{F1 Score} = 2 \times \frac{\text{Precision} \times \text{Recall}}{\text{Precision} + \text{Recall}}$$

5. **Area Under the Receiver Operating Characteristic (ROC-AUC)**:
   ROC-AUC mengukur kemampuan model dalam membedakan antara kelas positif dan negatif. Ini adalah area di bawah kurva ROC yang menunjukkan seberapa baik model dapat membedakan antara kelas positif dan negatif.

6. **Kolmogorov-Smirnov (KS) Statistic**:
   KS Statistik mengukur seberapa baik model memisahkan dua distribusi, dalam konteks ini, pembayar dan peminjam gagal. Ini sering digunakan dalam pemodelan risiko kredit untuk mengevaluasi kualitas prediksi model.

### Hasil Evaluasi

Setelah melatih model menggunakan data historis dan melakukan evaluasi menggunakan metrik-metrik di atas, berikut adalah hasil proyek berdasarkan metrik evaluasi yang digunakan:

| Metrics                 | XGBoost | Random Forest |
|-------------------------|---------|---------------|
| Akurasi                 | 0.945   | 0.897         |
| Presisi                 | 0.947   | 0.908         |
| Recall                  | 0.945   | 0.897         |
| F1 Score                | 0.938   | 0.855         |
| AUC                     | 0.912   | 0.864         |
| Kolmogorov-Smirnov (KS) | 0.651   | 0.570         |

|        Grafik ROC Curve XGBoost        |  Grafik ROC Curve Random Forest   |
|----------------------------------------|-----------------------------------|
| ![Gambar 1](img/roc-curve-xgboost.png) | ![Gambar 2](img/roc-curve-rf.png) |

| Grafik Kolmogorov-Smirnov XGBoost  | Grafik Kolmogorov-Smirnov Random Forest |
|------------------------------------|-----------------------------------------|
| ![Gambar 3](img/KS-xgb.png)        | ![Gambar 4](img/KS-rf.png)              |


Dengan hasil evaluasi diatas, model XGBoost memiliki peforma yang lebih baik dibandingkan model random forest dan telah terbukti efektif dalam memprediksi risiko kredit sehingga dapat digunakan dalam pengambilan keputusan pemberian pinjaman di masa depan.


## References
Hasan, M. (2017). Prediksi Tingkat Kelancaran Pembayaran Kredit Bank Menggunakan Algoritma Naïve Bayes Berbasis Forward Selection. ILKOM Jurnal Ilmiah, 9(3), 317-324.


