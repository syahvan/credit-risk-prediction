# Laporan Proyek _Credit Risk Prediction_ - Syahvan Alviansyah

## Domain Proyek

Dalam industri finansial, penilaian risiko kredit adalah salah satu aspek yang sangat penting. Hal ini karena risiko kredit merupakan faktor utama yang mempengaruhi kesehatan keuangan sebuah perusahaan. Pemberian kredit dapat mengalami berbagai masalah ataupun risiko. Permasalahan atau risiko yang dapat dialami dalam pemberian kredit adalah sikap nasabah yang tidak melakukan pembayaran angsuran secara tepat waktu atau menunda pembayaran sampai beberapa bulan pembayaran angsuran yang menyebabkan terjadinya **kredit macet** (Hasan, 2017). Dalam konteks ini, proyek _**Credit Risk Prediction**_ memainkan peran kunci dalam membantu perusahaan finansial dalam membuat keputusan pemberian pinjaman yang lebih baik. Melalui analisis data historis pinjaman, perusahaan dapat mengidentifikasi pola-pola yang berkaitan dengan pelunasan pinjaman dan mengembangkan model prediksi untuk memproyeksikan kemungkinan seorang peminjam untuk melunasi pinjaman di masa depan.

Risiko kredit memiliki dampak langsung yang signifikan terhadap kesehatan keuangan perusahaan finansial. Berikut adalah beberapa cara di mana risiko kredit mempengaruhi perusahaan finansial:

1. **Penurunan Pendapatan dan Laba**: Ketika kredit macet terjadi, perusahaan finansial akan mengalami penurunan pendapatan karena pembayaran angsuran yang seharusnya diterima tidak diterima. Selain itu, perusahaan juga mungkin harus menanggung biaya yang terkait dengan penagihan kredit macet. Hal ini akan mengurangi laba bersih perusahaan dan dapat mengganggu kinerja keuangan mereka secara keseluruhan.

   *Contoh*: Misalkan sebuah bank memberikan pinjaman kepada seorang pengusaha kecil. Jika pengusaha tersebut mengalami kesulitan keuangan dan tidak mampu membayar pinjaman, bank akan kehilangan pendapatan bunga yang diharapkan dari pinjaman tersebut, yang pada gilirannya akan mengurangi laba bersih mereka.

2. **Penurunan Kualitas Aset**: Pinjaman yang gagal membayar secara tepat waktu atau bahkan macet menjadi aset bermasalah bagi perusahaan finansial. Ini mempengaruhi kualitas portofolio aset mereka secara keseluruhan. Penurunan kualitas aset dapat memicu penurunan nilai aset, mengurangi nilai bersih perusahaan, dan mengganggu kemampuan mereka untuk memperoleh pembiayaan tambahan dari pasar modal.

   *Contoh*: Jika sejumlah besar pinjaman tidak terbayar dalam portofolio kredit bank, nilai portofolio tersebut akan menurun karena aset-aset tersebut menjadi tidak likuid atau bahkan bernilai nol. Hal ini dapat mempengaruhi kemampuan bank untuk memberikan pinjaman baru atau mendapatkan modal dari investor.

3. **Peningkatan Cadangan Kerugian Kredit**: Perusahaan finansial harus menyediakan cadangan kerugian kredit untuk mengantisipasi kemungkinan kerugian yang timbul dari kredit yang gagal dibayar. Peningkatan cadangan ini akan mempengaruhi laba bersih perusahaan secara negatif.

   *Contoh*: Bank harus mengalokasikan dana untuk cadangan kerugian kredit sesuai dengan estimasi risiko kredit yang mereka hadapi. Jika risiko kredit meningkat, bank harus meningkatkan cadangan kerugian kredit mereka, yang pada akhirnya akan mengurangi laba bersih mereka.

4. **Pengaruh Terhadap Kecukupan Modal**: Kredit macet dapat mempengaruhi rasio kecukupan modal perusahaan finansial. Jika jumlah kerugian kredit melebihi dana yang disediakan untuk cadangan kerugian kredit, perusahaan mungkin perlu menutupi kerugian tersebut dengan modal tambahan. Hal ini dapat menyebabkan tekanan pada kecukupan modal dan bahkan memicu kewajiban untuk mengumpulkan modal tambahan, yang mungkin sulit dilakukan terutama dalam situasi pasar yang sulit.

   *Contoh*: Jika bank mengalami kerugian besar karena kredit macet yang tidak diantisipasi, mereka mungkin perlu meningkatkan modal mereka untuk memenuhi persyaratan kecukupan modal yang ditetapkan oleh regulator. Hal ini dapat membutuhkan penggalangan modal tambahan dari pemegang saham atau pasar modal, atau bahkan menjual aset untuk memperoleh dana.

Dengan demikian, risiko kredit memiliki dampak yang sangat nyata dan langsung terhadap kesehatan keuangan perusahaan finansial, yang dapat merusak reputasi, pertumbuhan, dan stabilitas mereka dalam jangka panjang. Oleh karena itu, manajemen risiko kredit yang efektif menjadi kunci bagi perusahaan finansial untuk meminimalkan dampak negatif ini dan menjaga kesehatan keuangan mereka.

## Business Understanding

### Problem Statements

Berdasarkan latar belakang di atas, berikut ini batasan masalah yang dapat diselesaikan dengan proyek ini:
- Bagaimana mengembangkan model prediksi yang dapat memproyeksikan kemungkinan seorang peminjam untuk melunasi pinjaman di masa depan?
- Bagaimana meningkatkan keputusan pemberian pinjaman dengan mengurangi risiko kredit yang tidak diinginkan?
- Bagaimana cara menentukan hasil prediksi suatu algoritma _machine learning_ dapat dikatakan baik?

### Goals

Menjelaskan tujuan dari pernyataan masalah:
- Mengembangkan model prediksi risiko kredit yang memiliki akurasi tinggi.
- Mengurangi tingkat risiko kredit yang tidak diinginkan dalam keputusan pemberian pinjaman.
- Melakukan evaluasi terhadap metrik dari masing-masing algoritma.

### Solution Statements

- Melakukan pemodelan menggunakan beberapa algoritma _machine learning_ seperti _XGBoost_ dan _Random Forest_ untuk mencapai solusi yang diinginkan.
- Melakukan evaluasi model menggunakan classification report, AUC-ROC, dan Kolmogorov-Smirnov.

### Value Proposition

Implementasi model ini akan memberikan nilai tambah secara praktis bagi perusahaan finansial dengan beberapa cara:
- Meningkatkan akurasi dalam menilai risiko kredit, sehingga perusahaan dapat membuat keputusan pemberian pinjaman yang lebih baik dan mengurangi kemungkinan default.
- Mengoptimalkan proses pengambilan keputusan dengan menggunakan pendekatan berbasis data, yang dapat menghemat waktu dan sumber daya yang diperlukan dalam mengevaluasi aplikasi kredit secara manual.
- Mengurangi kerugian akibat kredit macet, yang pada gilirannya akan meningkatkan profitabilitas dan stabilitas keuangan perusahaan finansial.

### Social and Economic Impact

Penggunaan model ini dalam pengambilan keputusan kredit dapat memiliki dampak sosial dan ekonomi yang signifikan:
- Memberikan akses lebih luas kepada layanan keuangan bagi individu atau bisnis yang sebelumnya dianggap berisiko tinggi, sehingga membantu mendorong inklusi keuangan.
- Mengurangi risiko terhadap sistem keuangan secara keseluruhan dengan mengidentifikasi lebih awal potensi kredit macet, yang dapat membantu mencegah krisis finansial yang lebih luas.

## Data Understanding
Dataset yang digunakan merupakan data credit dari tahun 2007-2014 yang berasal dari [LendingClub](https://www.kaggle.com/datasets/devanshi23/loan-data-2007-2014), sebuah perusahaan _Peer-to-Peer_ (P2P) Lending yang berbasis di Amerika Serikat. Dataset tersebut berisi 466285 baris dan 74 kolom.

### Variabel-variabel pada Dataset LendingClub adalah sebagai berikut:
- `id`: ID unik yang ditetapkan LendingClub untuk daftar pinjaman. 
- `member_id`: Id unik yang ditetapkan untuk anggota peminjam.
- `loan_amnt`: Jumlah pinjaman yang tercantum yang diajukan oleh peminjam. Jika suatu saat departemen kredit mengurangi jumlah pinjaman, maka hal itu akan tercermin dalam nilai ini.
- `funded_amnt`: Jumlah total yang berkomitmen untuk pinjaman tersebut pada saat itu.
- `funded_amnt_inv`: Jumlah total yang berkomitmen oleh investor untuk pinjaman tersebut pada saat itu.
- `term`: Jumlah pembayaran pinjaman. Nilai dalam bulan dan dapat berupa 36 atau 60.          
- `int_rate`: Suku Bunga pinjaman
- `installment`: Pembayaran bulanan yang harus dibayar oleh peminjam jika pinjaman itu berasal.
- `grade`: Tingkat pinjaman               
- `sub_grade`: Tanah dasar pinjaman           
- `emp_title`: Jabatan yang diberikan oleh Peminjam saat mengajukan pinjaman.                    
- `emp_length`: Lamanya masa kerja dalam tahun. Nilai yang mungkin adalah antara 0 dan 10 dimana 0 berarti kurang dari satu tahun dan 10 berarti sepuluh tahun atau lebih.
- `home_ownership`: Status kepemilikan rumah yang diberikan oleh peminjam pada saat pendaftaran. Nilai-nilai: SEWA, SENDIRI, KPR, LAINNYA.      
- `annual_inc`: Pendapatan tahunan yang dilaporkan sendiri yang diberikan oleh peminjam saat pendaftaran.
- `verification_status`: Status verifikasi.
- `issue_d`: Bulan dimana pinjaman itu didanai.            
- `loan_status`: Status pinjaman saat ini.         
- `pymnt_plan`: Menunjukkan apakah rencana pembayaran telah diterapkan untuk pinjaman      
- `url`: URL untuk halaman LendingClub dengan data daftar.
- `desc`: Deskripsi pinjaman yang diberikan oleh peminjam.
- `purpose`: Kategori yang disediakan oleh peminjam untuk permintaan pinjaman.             
- `title`: Judul pinjaman yang diberikan oleh peminjam.
- `zip_code`: 3 angka pertama kode pos yang diberikan peminjam dalam permohonan pinjaman.             
- `addr_state`: Negara yang disediakan oleh peminjam dalam permohonan pinjaman.          
- `dti`: Rasio yang dihitung menggunakan total pembayaran utang bulanan peminjam terhadap total kewajiban utang, tidak termasuk hipotek dan pinjaman LC yang diminta, dibagi dengan pendapatan bulanan peminjam yang dilaporkan sendiri.             
- `delinq_2yrs`: Jumlah kejadian tunggakan lebih dari 30 hari dalam arsip kredit peminjam selama 2 tahun terakhir.     
- `earliest_cr_line`: Bulan dimana batas kredit peminjam yang paling awal dilaporkan dibuka.
- `inq_last_6mths`: Jumlah pertanyaan dalam 6 bulan terakhir (tidak termasuk pertanyaan otomotif dan hipotek).  
- `mths_since_last_delinq`: Jumlah bulan sejak tunggakan terakhir peminjam.
- `mths_since_last_record`: Jumlah bulan sejak pencatatan publik terakhir.
- `open_acc`: Jumlah jalur kredit terbuka dalam file kredit peminjam.        
- `pub_rec`: Jumlah catatan publik yang menghina.         
- `revol_bal`: Total saldo kredit bergulir
- `revol_util`: Tingkat pemanfaatan jalur bergulir, atau jumlah kredit yang digunakan peminjam relatif terhadap seluruh kredit bergulir yang tersedia.
- `total_acc`: Jumlah total batas kredit yang saat ini ada dalam arsip kredit peminjam.       
- `initial_list_status`: Status pencatatan awal pinjaman. Nilai yang mungkin adalah – W, ​​F 
- `out_prncp`: Sisa pokok terutang untuk jumlah total yang didanai.       
- `out_prncp_inv`: Sisa pokok terutang untuk sebagian dari jumlah total yang didanai oleh investor.   
- `total_pymnt`: Pembayaran diterima sampai saat ini untuk jumlah total yang didanai.     
- `total_pymnt_inv`: Pembayaran diterima hingga saat ini untuk sebagian dari jumlah total yang didanai oleh investor 
- `total_rec_prncp`: Pokok sudah diterima sampai saat ini. 
- `total_rec_int`: Bunga yang diterima sampai saat ini.   
- `total_rec_late_fee`: Biaya keterlambatan diterima sampai saat ini.
- `recoveries`: Pasca biaya dari pemulihan kotor.      
- `collection_recovery_fee`: Biaya pos dari biaya pengambilan.
- `last_pymnt_d`: Pembayaran bulan lalu telah diterima.
- `last_pymnt_amnt`: Jumlah total pembayaran terakhir yang diterima. 
- `next_pymnt_d`: Tanggal pembayaran terjadwal berikutnya.
- `last_credit_pull_d`: Bulan terakhir LC menarik kredit untuk pinjaman ini.
- `collections_12_mths_ex_med`: Jumlah koleksi dalam 12 bulan tidak termasuk koleksi medis.
- `mths_since_last_major_derog`: Bulan sejak rating 90 hari terakhir atau lebih buruk.
- `policy_code`: policy_code=1 tersedia untuk umum produk baru tidak tersedia untuk umum policy_code=2.
- `application_type`: Menunjukkan apakah pinjaman tersebut merupakan permohonan perorangan atau permohonan bersama dengan dua peminjam bersama.    
- `annual_inc_joint`: Gabungan pendapatan tahunan yang dilaporkan sendiri yang diberikan oleh peminjam bersama pada saat pendaftaran.    
- `dti_joint`: Rasio yang dihitung menggunakan total pembayaran bulanan rekan peminjam terhadap total kewajiban hutang, tidak termasuk hipotek dan pinjaman LC yang diminta, dibagi dengan gabungan pendapatan bulanan yang dilaporkan sendiri oleh rekan peminjam.
- `verification_status_joint`: Menunjukkan apakah pendapatan bersama peminjam bersama telah diverifikasi oleh LC, tidak diverifikasi, atau jika sumber pendapatan telah diverifikasi. 
- `acc_now_delinq`: Jumlah rekening dimana peminjam sekarang menunggak.  
- `tot_coll_amt`: Total jumlah penagihan yang terutang.      
- `tot_cur_bal`: Total saldo saat ini dari semua akun.       
- `open_acc_6m`: Jumlah perdagangan terbuka dalam 6 bulan terakhir. 
- `open_il_6m`: Jumlah perdagangan cicilan yang aktif saat ini.  
- `open_il_12m`: Jumlah rekening angsuran yang dibuka dalam 12 bulan terakhir. 
- `open_il_24m`: Jumlah rekening angsuran yang dibuka dalam 24 bulan terakhir. 
- `mths_since_rcnt_il`: Bulan sejak rekening cicilan terakhir dibuka.  
- `total_bal_il`: Total saldo saat ini dari semua rekening angsuran.
- `il_util`: Rasio total saldo saat ini terhadap kredit/batas kredit yang tinggi pada semua akun pemasangan.     
- `open_rv_12m`: Jumlah perdagangan bergulir yang dibuka dalam 12 bulan terakhir. 
- `open_rv_24m`: Jumlah perdagangan bergulir yang dibuka dalam 24 bulan terakhir. 
- `max_bal_bc`: Saldo terhutang maksimum saat ini pada semua akun bergulir.  
- `all_util`: Saldo hingga batas kredit pada semua perdagangan.    
- `total_rev_hi_lim`: Total batas kredit/kredit tinggi yang bergulir.  
- `inq_fi`: Jumlah pertanyaan keuangan pribadi.      
- `total_cu_tl`: Jumlah perdagangan keuangan. 
- `inq_last_12m`: Jumlah pertanyaan kredit dalam 12 bulan terakhir.

![Gambar 1](img/heatmap.png)
Gambar 1. _Heatmap_ Korelasi Antar Fitur pada Dataset

Analisis korelasi antar variabel dapat memberikan wawasan yang berharga tentang hubungan antara berbagai fitur dalam dataset dan bagaimana hal itu dapat mempengaruhi risiko kredit. _Heatmap_ korelasi (Gambar 1) menunjukkan tingkat korelasi antar variabel dalam bentuk matriks warna, di mana warna yang lebih terang menunjukkan korelasi yang lebih tinggi.

Beberapa temuan yang dapat diidentifikasi dari _heatmap_ korelasi ini adalah:

1. **Korelasi Positif**:
   - Terdapat korelasi positif yang cukup kuat antara `loan_amnt`, `funded_amnt`, dan `installment`, yang masuk akal karena pinjaman dengan jumlah yang lebih tinggi cenderung memiliki pembayaran bulanan yang lebih besar.
   - Juga, terdapat korelasi positif antara `total_pymnt`, `total_pymnt_inv`, `total_rec_prncp`, dan `total_rec_int`, yang dapat diharapkan karena jumlah pembayaran total harus sebanding dengan jumlah pokok dan bunga yang harus dibayarkan.

2. **Korelasi Negatif**:
   - Ada korelasi negatif yang cukup jelas antara `int_rate` (suku bunga) dan `grade`, `sub_grade`, yang sesuai dengan harapan bahwa tingkat bunga yang lebih tinggi akan diberikan kepada peminjam dengan peringkat risiko yang lebih rendah.

3. **Korelasi dengan `loan_status`**:
   - Variabel `loan_status` (status pinjaman) menunjukkan korelasi yang signifikan dengan beberapa fitur seperti `total_rec_prncp` (pokok yang diterima), `last_pymnt_amnt` (jumlah pembayaran terakhir yang diterima), dan `out_prncp` (sisa pokok terutang), yang dapat diharapkan karena fitur-fitur ini terkait langsung dengan status pembayaran pinjaman.

4. **Korelasi antara `dti` dan `annual_inc`**:
   - Terdapat korelasi antara `dti` (rasio utang terhadap pendapatan) dan `annual_inc` (pendapatan tahunan), yang wajar karena pembayaran bulanan yang lebih tinggi dapat terkait dengan pendapatan yang lebih rendah dan rasio utang yang lebih tinggi.

Analisis ini membantu memahami hubungan antara variabel-variabel dalam dataset dan bagaimana hubungan tersebut dapat memengaruhi risiko kredit. Misalnya, tingkat suku bunga (`int_rate`) yang lebih tinggi dapat berkorelasi dengan risiko kredit yang lebih tinggi, sementara pendapatan tahunan (`annual_inc`) yang lebih tinggi mungkin berhubungan dengan risiko kredit yang lebih rendah. Dengan pemahaman ini, perusahaan finansial dapat menggunakan informasi ini untuk mengembangkan model risiko kredit yang lebih baik dan membuat keputusan pemberian pinjaman yang lebih cerdas.

## Data Preparation

Dalam _data preparation_, prinsip **"_garbage in, garbage out_"** berlaku. Artinya, jika data yang digunakan untuk melatih model tidak berkualitas baik, maka hasil prediksi dari model tersebut juga akan tidak akurat atau tidak dapat diandalkan. Dengan memastikan data yang digunakan untuk melatih model memiliki kualitas yang baik, kita dapat menghasilkan model yang lebih andal dalam memprediksi risiko kredit.

Proses _data preparation_ meliputi beberapa tahap:

### 1. Pembersihan Data

- **Penanganan _Missing Values_**: Mengidentifikasi dan mengatasi nilai yang hilang atau tidak lengkap dalam dataset. Metode yang dapat digunakan termasuk menghapus baris atau kolom yang memiliki nilai yang hilang, mengisi nilai yang hilang dengan rata-rata atau median, atau menggunakan teknik imputasi berbasis model.
  
- **Penanganan _Outliers_**: Mendeteksi dan memproses nilai-nilai yang ekstrem atau tidak wajar yang mungkin mengganggu analisis atau model. Ini dapat dilakukan dengan menggunakan teknik seperti penghapusan _outliers_, transformasi data, atau menggunakan model yang lebih tahan terhadap _outliers_.

### 2. Pemrosesan Data

- **Pengkodean Variabel Kategorikal**: Mengubah variabel kategorikal menjadi bentuk numerik agar dapat digunakan dalam pemodelan. Salah satu pendekatan umum adalah _one-hot encoding_ di mana setiap nilai kategori diubah menjadi kolom biner baru.

- **Penskalaan Fitur Numerik**: Menyesuaikan skala fitur numerik agar memiliki rentang nilai yang seragam. Ini dapat dilakukan dengan menggunakan teknik seperti _standard scaler_ atau _min-max scaler_.

### 3. Seleksi Fitur

- Memilih fitur yang paling relevan dan berdampak signifikan terhadap target (misalnya, kemampuan untuk melunasi pinjaman). Ini dapat dilakukan dengan menggunakan teknik analisis statistik seperti korelasi, atau dengan menggunakan metode pemilihan fitur seperti _recursive feature elimination_.

- Pembuangan Fitur yang Tidak Berguna: Menghapus fitur-fitur yang tidak memberikan informasi yang berguna untuk pemodelan atau fitur-fitur yang memiliki masalah seperti memiliki nilai yang sama untuk setiap sampel, tidak bervariasi, atau tidak memiliki korelasi dengan target.

### 4. Pembagian Dataset

- Membagi dataset menjadi dua bagian: data latih dan data uji. Data latih digunakan untuk melatih model, sedangkan data uji digunakan untuk menguji kinerja model yang dilatih. Rasio pembagian yang umum adalah 80:20 atau 70:30.

Penentuan fitur-fitur mana yang harus dipertahankan atau dibuang untuk pemodelan biasanya didasarkan pada pemahaman domain dan eksplorasi data yang teliti. Misalnya, fitur yang merupakan identifikasi unik (seperti ID pelanggan), fitur yang memiliki nilai yang sama untuk setiap sampel, atau fitur yang tidak memiliki korelasi dengan target umumnya dianggap tidak berguna dan dibuang. Sedangkan fitur-fitur yang memiliki hubungan yang kuat dengan target atau membawa informasi yang relevan untuk pemodelan akan dipertahankan.

Dengan melakukan proses _data preparation_ dengan cermat, kita dapat memastikan bahwa model yang dikembangkan berdasarkan data yang berkualitas akan memberikan hasil prediksi yang lebih andal dan akurat dalam memprediksi risiko kredit.

## Modeling

Untuk tahap pemodelan, digunakan dua algoritma _machine learning_, yakni _XGBoost_ dan _Random Forest_. Berikut adalah gambaran ringkas tentang kedua algoritma tersebut:

### 1. _XGBoost_ (_Extreme Gradient Boosting_)

_XGBoost_ (_Extreme Gradient Boosting_) adalah algoritma _ensemble_ yang kuat dan efisien yang sering digunakan dalam kompetisi data dan aplikasi produksi. Beberapa parameter yang dapat digunakan dalam pemodelan _XGBoost_ ini adalah:

- `learning_rate`: Menentukan seberapa besar update yang akan dilakukan pada nilai prediksi setiap kali ada iterasi.
- `max_depth`: Menentukan kedalaman maksimum dari setiap pohon dalam _ensemble_.
- `n_estimators`: Menentukan jumlah pohon keputusan yang akan dibangun.
- `gamma`: Menentukan minimum penurunan kerugian yang diperlukan untuk melakukan pemisahan tambahan pada simpul pohon.
- `subsample`: Menentukan fraksi sampel yang akan digunakan dalam setiap iterasi.
- `colsample_bytree`: Menentukan fraksi kolom yang akan digunakan dalam setiap iterasi untuk membangun setiap pohon.

Kelebihan _XGBoost_ adalah kemampuannya dalam menangani dataset besar dengan cepat, toleran terhadap _overfitting_, dan memiliki fleksibilitas dalam menangani berbagai jenis data. Namun, kelemahannya adalah rentan terhadap _overfitting_ jika parameter tidak disetel dengan benar.

### 2. _Random Forest_

_Random Forest_ adalah algoritma _ensemble_ lain yang sangat populer. Algoritma ini bekerja dengan membangun sejumlah besar pohon keputusan selama pelatihan dan menggabungkan hasil prediksi dari setiap pohon untuk menghasilkan prediksi akhir. Beberapa parameter yang dapat digunakan dalam pemodelan _Random Forest_ ini adalah:

- `n_estimators`: Menentukan jumlah pohon keputusan yang akan dibangun.
- `max_depth`: Menentukan kedalaman maksimum dari setiap pohon.
- `min_samples_split`: Menentukan jumlah sampel minimum yang diperlukan untuk membagi simpul internal.
- `min_samples_leaf`: Menentukan jumlah sampel minimum yang diperlukan untuk menjadi simpul daun.
- `max_features`: Menentukan jumlah fitur yang akan dipertimbangkan saat mencari split terbaik.

Kelebihan dari _Random Forest_ adalah kemampuannya dalam menangani data yang tidak seimbang dan rentan terhadap _overfitting_. Namun, kelemahannya adalah model yang dihasilkan tidak mudah diinterpretasi dibandingkan dengan model linear.

### Pemilihan Model

Pemilihan model terbaik antara _XGBoost_ dan _Random Forest_ bergantung pada karakteristik dataset dan tujuan pemodelan. Dalam kasus ini, kedua algoritma dipilih karena:

- Kedua algoritma ini dikenal memiliki kinerja yang baik dalam pemodelan prediksi, terutama dalam kasus klasifikasi seperti prediksi risiko kredit.
- Keduanya memiliki kemampuan untuk menangani data yang besar dan kompleks.
- _XGBoost_ dan _Random Forest_ adalah dua algoritma yang sudah terbukti dalam banyak kasus penggunaan dan kompetisi data.

Dalam implementasi, parameter-parameter dalam model dapat disesuaikan untuk meningkatkan performa. Misalnya, untuk _XGBoost_, kita dapat menyesuaikan learning rate, max depth, dan jumlah estimators untuk mencari kombinasi yang optimal. Sedangkan untuk _Random Forest_, kita dapat menyesuaikan jumlah pohon, kedalaman maksimum, dan kriteria pemisahan.

Berikut adalah nilai parameter yang digunakan dalam pemodelan:

- **_XGBoost_**:
  - `learning_rate`: 0.1
  - `max_depth`: 10
  - `n_estimators`: 100
  - `gamma`: 0
  - `subsample`: 0.8
  - `colsample_bytree`: 0.8

- **_Random Forest_**:
  - `n_estimators`: 100
  - `max_depth`: 10
  - `min_samples_split`: 2
  - `min_samples_leaf`: 1
  - `max_features`: 'auto'

Dengan memilih dan menyesuaikan parameter-parameter ini, diharapkan kedua model dapat memberikan performa yang optimal dalam memprediksi risiko kredit.

## Evaluation
### Metrik Evaluasi

Dalam proyek ini, kami menggunakan beberapa metrik evaluasi yang sesuai dengan konteks klasifikasi pada model prediksi risiko kredit. Berikut adalah penjelasan singkat mengenai metrik-metrik yang digunakan:

1. **Akurasi (_Accuracy_)**:
   Akurasi mengukur seberapa tepat model dalam memprediksi keseluruhan kelas yang benar. Metrik ini dihitung sebagai rasio prediksi benar (positif dan negatif) dengan total sampel.
   
   $$\text{Accuracy} = \frac{\text{TP} + \text{TN}}{\text{TP} + \text{TN} + \text{FP} + \text{FN}}$$

   - **Keuntungan**: Akurasi memberikan gambaran tentang seberapa baik model dapat memprediksi secara keseluruhan.
   - **Kerugian**: Tidak cocok untuk dataset yang tidak seimbang, di mana kelas target memiliki proporsi yang berbeda. Misalnya, jika kelas negatif lebih dominan daripada kelas positif, akurasi tinggi dapat diperoleh dengan model yang hanya memprediksi kelas mayoritas.

2. **Presisi (_Precision_)**:
   Presisi mengukur seberapa tepat model dalam memprediksi kelas positif. Metrik ini dihitung sebagai rasio prediksi benar positif (TP) dengan total prediksi positif (TP + FP).
   
   $$\text{Precision} = \frac{\text{TP}}{\text{TP} + \text{FP}}$$

   - **Keuntungan**: Presisi memberikan informasi tentang seberapa baik model dalam mengidentifikasi kelas positif. Ini penting dalam kasus seperti pemberian pinjaman di mana keakuratan dalam mengidentifikasi peminjam yang akan melunasi pinjaman sangat penting.
   - **Kerugian**: Presisi tidak mempertimbangkan _false negative_ (FN), sehingga tidak memberikan gambaran lengkap tentang kemampuan model dalam menghindari kesalahan prediksi.

3. **_Recall_ (Sensitivitas)**:
   _Recall_ mengukur seberapa baik model dalam menemukan kembali semua instansi kelas positif. Metrik ini dihitung sebagai rasio prediksi benar positif (TP) dengan total kelas positif yang sebenarnya (TP + FN).
   
   $$\text{Recall} = \frac{\text{TP}}{\text{TP} + \text{FN}}$$

   - **Keuntungan**: _Recall_ memberikan informasi tentang seberapa baik model dalam menemukan semua instansi kelas positif. Ini penting dalam kasus di mana mengidentifikasi semua kasus positif (misalnya, peminjam yang akan gagal membayar) lebih penting daripada mengurangi jumlah _false positive_ (FP).
   - **Kerugian**: _Recall_ tidak mempertimbangkan _false positive_ (FP), sehingga tidak memberikan gambaran lengkap tentang kemampuan model dalam menghindari kesalahan prediksi.

4. **_F1 Score_**:
   _F1 score_ adalah rata-rata harmonis dari presisi dan _recall_. Metrik ini memberikan keseimbangan antara presisi dan _recall_.
   
   $$\text{_F1 Score_} = 2 \times \frac{\text{Precision} \times \text{Recall}}{\text{Precision} + \text{Recall}}$$

   - **Keuntungan**: _F1 score_ adalah rata-rata harmonis dari presisi dan _recall_, yang memberikan keseimbangan antara kedua metrik tersebut. Ini berguna saat kita ingin mencari model yang seimbang dalam menghindari _false positive_ dan _false negative_.
   - **Kerugian**: _F1 score_ memberi bobot yang sama pada presisi dan _recall_, yang mungkin tidak selalu sesuai dengan preferensi atau kebutuhan bisnis tertentu.

5. **_Area Under the Receiver Operating Characteristic_ (ROC-AUC)**:
   ROC-AUC mengukur kemampuan model dalam membedakan antara kelas positif dan negatif. Ini adalah area di bawah kurva ROC yang menunjukkan seberapa baik model dapat membedakan antara kelas positif dan negatif.

   - **Keuntungan**: ROC-AUC mengukur kemampuan model dalam membedakan antara kelas positif dan negatif dengan memperhitungkan semua nilai _threshold_. Ini membuatnya cocok untuk mengevaluasi performa model di berbagai _threshold_.
   - **Kerugian**: ROC-AUC tidak memberikan informasi langsung tentang keakuratan kelas positif atau negatif secara terpisah. Selain itu, ROC-AUC tidak sensitif terhadap ketidakseimbangan kelas.

6. **Kolmogorov-Smirnov (KS) _Statistic_**:
   KS Statistik mengukur seberapa baik model memisahkan dua distribusi, dalam konteks ini, pembayar dan peminjam gagal. Ini sering digunakan dalam pemodelan risiko kredit untuk mengevaluasi kualitas prediksi model.

   - **Keuntungan**: KS Statistik mengukur seberapa baik model memisahkan dua distribusi, dalam konteks ini, pembayar dan peminjam gagal. Ini memberikan gambaran tentang seberapa baik model dalam mengidentifikasi perbedaan antara kedua kelas.
   - **Kerugian**: KS Statistik tidak memberikan informasi tentang keakuratan absolut dari model, tetapi lebih fokus pada kemampuannya untuk membedakan antara dua kelas.

### Hasil Evaluasi

Setelah melatih model menggunakan data historis dan melakukan evaluasi menggunakan metrik-metrik di atas, berikut adalah hasil proyek berdasarkan metrik evaluasi yang digunakan:

Tabel 1. Evaluasi model _machine learning_
| _Metrics_               | _XGBoost_ | _Random Forest_ |
|-------------------------|-----------|-----------------|
| Akurasi                 | 0.944     | 0.942           |
| Presisi                 | 0.946     | 0.946           |
| _Recall_                | 0.944     | 0.942           |
| _F1 Score_              | 0.936     | 0.933           |
| AUC                     | 0.910     | 0.872           |
| Kolmogorov-Smirnov (KS) | 0.646     | 0.586           |

|   Gambar 2. Grafik _ROC Curve XGBoost_   | Gambar 3. Grafik _ROC Curve Random Forest_ |
|------------------------------------------|--------------------------------------------|
| ![Gambar 2](img/roc-curve-xgboost.png)   | ![Gambar 3](img/roc-curve-rf.png)          |

| Gambar 4. Grafik Kolmogorov-Smirnov _XGBoost_ | Gambar 5. Grafik Kolmogorov-Smirnov _Random Forest_ |
|-----------------------------------------------|-----------------------------------------------------|
| ![Gambar 4](img/KS-xgb.png)                   | ![Gambar 5](img/KS-rf.png)                          |


#### Analisis Hasil:

- **Akurasi**: Kedua model, _XGBoost_ dan _Random Forest_, memiliki akurasi yang sangat tinggi, dengan nilai di atas 0.94. Ini menunjukkan bahwa kedua model mampu memprediksi dengan sangat baik kelas peminjam yang akan melunasi pinjaman dan yang akan gagal melakukannya.

- **Presisi dan Recall**: _XGBoost_ dan _Random Forest_ memiliki presisi dan recall yang seimbang, menunjukkan bahwa keduanya baik dalam memprediksi kelas positif dan negatif.

- **_F1 Score_**: Keduanya memiliki _F1 score_ yang tinggi, menunjukkan keseimbangan antara presisi dan recall.

- **ROC-AUC**: _XGBoost_ memiliki nilai ROC-AUC yang sedikit lebih tinggi daripada _Random Forest_, menunjukkan bahwa _XGBoost_ lebih baik dalam membedakan antara kelas positif dan negatif.

- **Kolmogorov-Smirnov (KS) _Statistic_**: _XGBoost_ juga memiliki nilai KS yang lebih tinggi daripada _Random Forest_, menunjukkan bahwa _XGBoost_ lebih baik dalam memisahkan dua distribusi, yaitu pembayar dan peminjam gagal.

#### Potensi _Overfitting_:

Meskipun hasil evaluasi menunjukkan performa yang sangat baik dari kedua model, ada potensi untuk _overfitting_ terutama jika model sangat kompleks atau terlalu diperlengkapi dengan data latih. Untuk mengatasi _overfitting_, beberapa langkah yang dapat diambil termasuk:

- **Penyetelan Parameter**: Menyesuaikan parameter model untuk menghindari model menjadi terlalu kompleks.
- **Validasi Silang**: Melakukan validasi silang untuk memeriksa kestabilan performa model pada data yang tidak terlihat.
- **Regularisasi**: Menambahkan regularisasi ke model untuk mengontrol kompleksitasnya.
- **Pemilihan Fitur**: Memilih hanya fitur-fitur yang paling relevan dan meninggalkan fitur-fitur yang tidak memberikan kontribusi signifikan dalam prediksi.

### Kesimpulan
Berdasarkan hasil proyek dan metrik evaluasi yang digunakan, dapat disimpulkan bahwa kedua model (_XGBoost_ dan _Random Forest_) memberikan performa yang sangat baik dalam memprediksi risiko kredit berdasarkan dataset yang diberikan. Tujuan proyek ini, yaitu mengembangkan model yang dapat membantu dalam pengambilan keputusan pemberian pinjaman dengan memprediksi apakah seorang peminjam akan melunasi pinjamannya atau tidak, telah tercapai.

Hasil evaluasi menunjukkan bahwa kedua model memiliki akurasi, presisi, dan _recall_ yang tinggi, serta _F1 score_ yang seimbang. Hal ini menunjukkan bahwa model mampu dengan baik dalam mengidentifikasi kedua kelas, yaitu peminjam yang akan melunasi pinjaman dan yang akan gagal melakukannya. Selain itu, nilai ROC-AUC dan KS _Statistic_ yang tinggi menunjukkan kemampuan model dalam membedakan antara kelas positif dan negatif, serta memisahkan dua distribusi, yaitu pembayar dan peminjam gagal.

Dengan demikian, hasil evaluasi ini dan model yang dikembangkan dapat menjadi solusi yang efektif untuk menyelesaikan permasalahan yang sedang diselesaikan, yaitu membantu perusahaan finansial dalam mengambil keputusan pemberian pinjaman dengan memprediksi risiko kredit secara akurat. Dengan model ini, perusahaan dapat mengidentifikasi peminjam yang berisiko tinggi dan mengurangi risiko potensial dalam portofolio pinjamannya.

Namun demikian, penting untuk terus memantau dan memvalidasi model ini secara berkala menggunakan data yang baru untuk memastikan bahwa performanya tetap konsisten dan relevan terhadap perubahan dalam lingkungan bisnis dan pasar keuangan. Selain itu, langkah-langkah pencegahan _overfitting_ yang disebutkan sebelumnya juga perlu diterapkan untuk memastikan kehandalan dan generalisasi model dalam situasi yang berbeda. Dengan demikian, model ini dapat menjadi alat yang berguna dan efektif bagi perusahaan dalam mengelola risiko kredit dan mengoptimalkan keputusan pemberian pinjaman.

## References
Hasan, M. (2017). Prediksi Tingkat Kelancaran Pembayaran Kredit Bank Menggunakan Algoritma Naïve Bayes Berbasis Forward Selection. ILKOM Jurnal Ilmiah, 9(3), 317-324.