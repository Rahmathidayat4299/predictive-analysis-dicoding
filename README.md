# Predictive-analysis-dicoding
     Domain project ialah keuangan dengan judul Predictive Analysis Prediksi Sales Supermarket
# Latar Belakang

Di era digital saat ini, perusahaan menghadapi tantangan yang semakin kompleks dalam memahami dan memprediksi perilaku konsumen. Dengan meningkatnya persaingan di pasar, penting bagi bisnis untuk dapat membuat keputusan yang tepat berdasarkan analisis data. Salah satu aspek kritis dari strategi bisnis yang efektif adalah kemampuan untuk memprediksi total penjualan, yang merupakan indikator utama keberhasilan finansial suatu perusahaan.

Dalam konteks ini, total penjualan dipengaruhi oleh berbagai faktor, termasuk karakteristik pelanggan, jenis produk yang dijual, dan lokasi cabang. Jenis pelanggan, apakah mereka anggota atau normal, dapat memberikan wawasan tentang perilaku belanja yang berbeda. Jenis produk juga memainkan peran penting, karena berbagai kategori produk memiliki daya tarik dan permintaan yang bervariasi di kalangan konsumen. Selain itu, lokasi cabang dapat memengaruhi aksesibilitas produk dan preferensi lokal, yang semuanya dapat berdampak pada volume penjualan.

Penggunaan teknik analisis data, seperti regresi dan algoritma machine learning, memberikan peluang untuk menggali pola dan hubungan dalam data yang sebelumnya tidak terlihat. Model prediksi yang akurat tidak hanya membantu perusahaan dalam merencanakan strategi penjualan, tetapi juga dalam pengambilan keputusan yang lebih baik terkait dengan stok, pemasaran, dan pengembangan produk.

Dengan memanfaatkan data historis penjualan, serta fitur-fitur terkait seperti harga unit, pajak, dan rating produk, penelitian ini bertujuan untuk mengembangkan model prediksi yang dapat mengidentifikasi faktor-faktor yang paling berpengaruh terhadap total penjualan. Hasil dari penelitian ini diharapkan dapat memberikan wawasan yang berharga bagi perusahaan dalam meningkatkan strategi penjualan dan memaksimalkan pendapatan.

# Business Understanding
Dalam dunia bisnis yang kompetitif, pemahaman yang mendalam tentang faktor-faktor yang mempengaruhi penjualan sangat penting untuk pengambilan keputusan yang efektif. Total penjualan adalah metrik kunci yang mencerminkan kesehatan finansial perusahaan dan merupakan indikator utama dari pertumbuhan dan keberhasilan bisnis.
Untuk meningkatkan performa penjualan, perusahaan perlu memahami perilaku konsumen yang beragam. Dengan menganalisis variabel seperti jenis pelanggan (anggota atau normal), jenis produk yang ditawarkan, dan lokasi cabang, perusahaan dapat mengidentifikasi pola yang dapat memandu strategi pemasaran, pengelolaan inventaris, dan pengembangan produk.
Melalui pendekatan berbasis data, perusahaan dapat membangun model prediksi yang tidak hanya memberikan wawasan tentang proyeksi penjualan, tetapi juga membantu dalam merumuskan strategi yang lebih tepat dan responsif terhadap kebutuhan pasar.

# Problem Statements
Berdasarkan latar belakang di atas, berikut ini merupakan rincian masalah yang dapat diselesaikan pada proyek ini:
bagaimana hasil dari pertanyaan Bagaimana kita bisa memprediksi total penjualan (Total) dari kombinasi variabel seperti jenis pelanggan, jenis produk, dan lokasi cabang?

# Goals
Tujuan dari Analysis ini ialah
* Memahami Faktor yang Mempengaruhi Penjualan:
Mengidentifikasi bagaimana variabel seperti jenis pelanggan, jenis produk, dan lokasi cabang berkontribusi terhadap total penjualan.
* Pengembangan Model Prediksi:
Membangun dan melatih model yang dapat digunakan untuk memprediksi total penjualan berdasarkan data historis.
* Pengambilan Keputusan Berbasis Data:
Memberikan insight yang berguna bagi manajemen untuk membuat keputusan yang lebih baik dalam strategi pemasaran dan penjualan.
Optimisasi Strategi Pemasaran:
Menggunakan hasil prediksi untuk menyesuaikan strategi penjualan dan pemasaran agar lebih efektif dalam mencapai target penjualan.

# Data UnderStanding
1. Jumlah Data (Baris dan Kolom):
Baris (Jumlah data): Dataset ini menampilkan nomor baris dari 0 hingga 999, yang menunjukkan bahwa ada 1.000 baris (data point).
Kolom: Terdapat 17 kolom dalam dataset ini.
2. Kondisi Data:
Data terlihat cukup rapi, tidak ada nilai yang hilang atau tidak wajar dalam tampilan data ini.
Nilai pada kolom seperti Total, Unit price, dan Quantity tampak konsisten dan realistis.
Kolom Date dan Time memiliki format yang seragam, di mana tanggal menggunakan format MM/DD/YYYY.
3. Tautan Sumber Data:
https://www.kaggle.com/datasets/aungpyaeap/supermarket-sales .
4. Uraian Seluruh Fitur (Kolom) Pada Data:
Penjelasan mengenai setiap fitur dalam dataset:

* Invoice ID: Nomor identifikasi unik untuk setiap transaksi.
* Branch (Cabang): Cabang toko di mana penjualan terjadi (misalnya: 'A', 'B', 'C').
* City (Kota): Kota di mana cabang toko tersebut berada (contoh: 'Yangon', 'Naypyitaw').
* Customer type (Jenis Pelanggan): Jenis pelanggan, yaitu Member (Anggota) atau Normal (Non-anggota).
* Gender (Jenis Kelamin): Jenis kelamin pelanggan (misalnya: 'Male' untuk laki-laki dan 'Female' untuk perempuan).
* Product line (Lini Produk): Kategori produk yang dijual (contoh: 'Health and beauty', 'Fashion accessories').
* Unit price (Harga Satuan): Harga per satuan produk yang dibeli.
* Quantity (Jumlah): Jumlah unit produk yang dibeli dalam satu transaksi.
* Tax 5% (Pajak 5%): Pajak yang diterapkan pada pembelian dengan tarif 5%.
* Total: Jumlah total yang dibayarkan, termasuk pajak.
* Date (Tanggal): Tanggal terjadinya transaksi.
* Time (Waktu): Waktu terjadinya transaksi.
* Payment (Pembayaran): Metode pembayaran yang digunakan (misalnya: 'Cash' untuk tunai, 'Credit card' untuk kartu kredit, atau 'Ewallet').
* COGS (Cost of Goods Sold / Biaya Produksi): Biaya langsung yang dapat dikaitkan dengan produksi barang yang dijual.
* Gross margin percentage (Persentase Margin Kotor): Persentase dari total pendapatan penjualan yang dipertahankan perusahaan setelah mengeluarkan biaya langsung yang terkait dengan produksi barang. (Nilai ini tampaknya konstan pada 4.761905 dalam dataset ini).
* Gross income (Pendapatan Kotor): Pendapatan yang diperoleh dari penjualan, dihitung sebagai Total - COGS.
* Rating: Peringkat yang diberikan pelanggan untuk transaksi tersebut, mungkin dalam skala 1 hingga 10.


# Variabel-variabel pada Data ialah :
*Invoice ID: String (atau kategori) - Merupakan identifikasi unik untuk setiap transaksi dan biasanya dalam format teks.<br>
*Branch: Kategori - Menunjukkan cabang tempat transaksi dilakukan, biasanya berupa huruf (misalnya, A, B, C).<br>
* City: Kategori - Menunjukkan nama kota tempat cabang berlokasi, berupa teks.<br>
* Customer type: Kategori - Mengindikasikan tipe pelanggan, biasanya berupa kategori seperti "Member" atau "Normal".<br>
* Gender: Kategori - Menunjukkan jenis kelamin pelanggan, biasanya berupa "Male" atau "Female".<br>
* Product line: Kategori - Mengindikasikan kategori produk yang dibeli, berupa teks (misalnya, "Health and beauty").<br>
* Unit price: Float - Menunjukkan harga per unit produk, berupa angka desimal.<br>
* Quantity: Integer - Menunjukkan jumlah produk yang dibeli, berupa angka bulat.<br>
* Tax 5%: Float - Menunjukkan pajak yang dikenakan (5% dari total harga), berupa angka desimal.<br>
* Total: Float - Menunjukkan total harga setelah pajak, berupa angka desimal.<br>
* Date: Tanggal - Menunjukkan tanggal transaksi, biasanya dalam format teks yang dapat diubah menjadi tipe tanggal.<br>
* Time: Waktu - Menunjukkan waktu transaksi, biasanya dalam format teks (jam)<br>
* Payment: Kategori - Menunjukkan metode pembayaran yang digunakan (misalnya, "Ewallet", "Cash").<br>
* cogs: Float - Menunjukkan biaya barang yang terjual (Cost of Goods Sold), berupa angka desimal.<br>
* gross margin percentage: Float - Menunjukkan persentase margin kotor, berupa angka desimal.<br>
* gross income: Float - Menunjukkan total pendapatan kotor, berupa angka desimal.<br>
* Rating: Float - Menunjukkan rating yang diberikan oleh pelanggan, biasanya dalam skala 1-10, berupa angka desimal.<br>

# Data Preparation
1. Cek Nilai Null dan Duplikat
Tujuan: Untuk memeriksa apakah terdapat nilai kosong (null) atau baris duplikat dalam dataset yang dapat mempengaruhi kualitas data.
Langkah:
Menggunakan .isnull().sum() untuk menghitung jumlah nilai null pada setiap kolom.
Menggunakan .duplicated().sum() untuk menghitung jumlah baris duplikat.
Hasil: Tidak ditemukan nilai null maupun duplikat dalam dataset, sehingga tidak perlu melakukan imputasi atau penghapusan baris.
2. Menghitung Statistik Deskriptif
Tujuan: Untuk memahami distribusi data seperti mean, standar deviasi, dan kuartil dari kolom numerik.
Langkah:
Menggunakan .describe() untuk melihat statistik dasar, seperti rata-rata (mean), nilai minimum (min), maksimum (max), dan kuartil (Q1, Q3).
Hasil: Statistik ini memberikan gambaran umum tentang distribusi nilai pada setiap kolom numerik.
3. Deteksi dan Penanganan Outlier
![image](https://github.com/user-attachments/assets/3dd63248-a440-4bf0-9f77-bfd2b1f1f6b4)
Tujuan: Untuk mendeteksi data yang berada di luar batas normal atau rentang data yang wajar (outlier).
Langkah:
Menentukan numerical columns yang relevan untuk outlier (misalnya, Unit price, Quantity, Total, dan Rating).
Menghitung Kuartil Pertama (Q1) dan Kuartil Ketiga (Q3) menggunakan .quantile().
Menghitung Interquartile Range (IQR) dengan rumus IQR = Q3 - Q1.
Menentukan batas bawah dan batas atas outlier menggunakan rumus Q1 - 1.5 * IQR dan Q3 + 1.5 * IQR.
Mendeteksi outlier dengan memeriksa apakah ada nilai di bawah batas bawah atau di atas batas atas pada setiap kolom.
Hasil: Terdeteksi 9 outlier yang kemudian bisa dianalisis lebih lanjut, apakah akan dihapus atau diperbaiki.
4. Encoding (One-Hot Encoding)
Tujuan: Mengubah data kategorikal menjadi bentuk numerik agar dapat digunakan dalam model machine learning.
Langkah:
Menggunakan One-Hot Encoding dengan fungsi pd.get_dummies() untuk variabel kategorikal, yaitu Customer type, Product line, Branch, City, Gender, dan Payment.
Parameter drop_first=True digunakan untuk menghindari multikolinearitas dengan membuang salah satu kategori sebagai referensi.
Hasil: Variabel kategorikal dikonversi menjadi variabel dummy (0 atau 1), dan dataset siap digunakan dalam pemodelan.
5. Split Data (Pemecahan Data)
Tujuan: Memisahkan dataset menjadi data latih (training set) dan data uji (test set) untuk memvalidasi performa model.
Langkah:
Biasanya menggunakan train_test_split() dari Scikit-Learn untuk membagi dataset menjadi dua bagian.
Proporsi umum yang digunakan adalah 80% untuk data latih dan 20% untuk data uji.
Hasil: Dataset terbagi dengan baik sehingga model dapat dilatih pada data latih dan divalidasi pada data uji.
6. Kesimpulan Data Preparation
Dataset sudah melalui berbagai tahap persiapan, termasuk pengecekan kualitas data (null dan duplikat), deteksi outlier, encoding variabel kategorikal, dan pembagian dataset untuk pelatihan dan pengujian. Setiap tahap dilakukan untuk memastikan data bersih dan siap digunakan dalam pemodelan machine learning.
![image](https://github.com/user-attachments/assets/27e9c67e-a695-4409-8b63-c4e9b5ca6b1d)

## Standarization Data
     Mengubah skala data agar lebih konsisten

## Modeling: Regresi
1. Regresi Linier
Regresi Linier adalah salah satu algoritma dasar dalam supervised learning yang bertujuan untuk memprediksi variabel target kontinu (numerik) berdasarkan variabel prediktor (fitur). Model ini mengasumsikan adanya hubungan linear antara variabel prediktor (X) dan target (y), dan menghasilkan garis lurus yang mendekati titik-titik data sebaik mungkin.

Cara Kerja:
Regresi linier menghitung koefisien (slope) dan konstanta (intercept) untuk setiap fitur dalam dataset dengan tujuan meminimalkan perbedaan antara prediksi model dan nilai aktual. 
Parameter Utama:
fit_intercept: Menentukan apakah model harus menghitung intercept atau tidak. Jika False, maka garis akan melalui titik asal.
normalize: Menentukan apakah input harus dinormalisasi sebelum melakukan regresi.
n_jobs: Menentukan jumlah thread yang digunakan untuk komputasi, default adalah None, yang berarti hanya menggunakan satu thread.

2. XGBoost Regressor
XGBoost (Extreme Gradient Boosting) adalah algoritma ensemble yang sangat populer dalam kompetisi data science. Ini menggunakan teknik boosting yang bertujuan untuk meningkatkan performa model dengan membangun model regresi atau klasifikasi secara bertahap, di mana setiap model mencoba memperbaiki kesalahan dari model sebelumnya.

Cara Kerja:
Boosting: XGBoost menggabungkan beberapa model keputusan (decision tree) secara bertahap. Setiap model baru fokus pada memperbaiki kesalahan model sebelumnya dengan menambahkan bobot lebih pada observasi yang sulit diprediksi.
Gradient Descent: Algoritma ini menggunakan gradient descent untuk mengoptimalkan fungsi loss dan secara bertahap mengurangi error dari model.
Regularisasi: XGBoost menggunakan regularisasi L1 (Lasso) dan L2 (Ridge) untuk mengurangi risiko overfitting dengan menghukum model yang terlalu kompleks.
Parameter Utama:
n_estimators: Jumlah pohon keputusan yang dibangun secara bertahap.
learning_rate: Mengontrol ukuran langkah yang diambil dalam setiap iterasi boosting. Nilai yang lebih kecil menghasilkan proses yang lebih lambat tetapi lebih stabil.
max_depth: Kedalaman maksimum pohon keputusan. Nilai yang lebih besar memungkinkan pohon menjadi lebih kompleks.
objective: Fungsi loss yang akan dioptimalkan. Dalam kasus regresi, kita menggunakan 'reg:squarederror', yang berarti meminimalkan mean squared error.
random_state: Seed yang digunakan untuk pengacakan, memastikan hasil yang dapat direproduksi.
subsample: Persentase sampel data yang digunakan untuk membangun setiap pohon. Nilai yang lebih rendah dapat membantu mengurangi overfitting.
3. Optimasi Hyperparameter (Hyperparameter Tuning)
Setelah membangun model, optimasi hyperparameter sangat penting untuk meningkatkan performa model. Hyperparameter adalah parameter yang tidak dipelajari langsung dari data, melainkan harus ditentukan sebelum pelatihan. Proses tuning melibatkan mencoba beberapa kombinasi nilai hyperparameter untuk menemukan pengaturan terbaik.

Langkah-Langkah Hyperparameter Tuning:
Grid Search: Mencoba semua kombinasi dari daftar nilai hyperparameter yang telah didefinisikan sebelumnya.
![image](https://github.com/user-attachments/assets/706a89de-2bee-40eb-8754-f87c84c3f618)

Contoh Hyperparameter Tuning untuk XGBoost:
Mencoba berbagai nilai untuk n_estimators (misalnya 100, 200, 300).
Menyesuaikan learning_rate (misalnya 0.01, 0.1, 0.2).
Mengatur kedalaman maksimal dari pohon (max_depth), misalnya 3, 5, 7.
Mencoba subsample (misalnya 0.6, 0.8, 1.0) untuk mengurangi overfitting.
# Evaluation
Setelah membangun beberapa model, yaitu Linear Regression dan XGBoost Regressor, langkah berikutnya adalah mengevaluasi performa masing-masing model untuk menentukan mana yang paling sesuai dalam menjawab problem statement dan apakah model tersebut telah mencapai goals yang diharapkan.

1. Evaluasi Model: Linear Regression
Pada bagian sebelumnya, kita telah menggunakan model Linear Regression, dan hasil evaluasinya adalah:

Mean Squared Error (MSE): 5.96e-27 (hampir nol, yang berarti model ini sangat baik dalam memprediksi nilai target pada data uji).
R-squared (R²): 1.0 (menunjukkan bahwa model mampu menjelaskan 100% variansi dalam data, yang merupakan nilai ideal).
Analisis:
Nilai R-squared yang sempurna (1.0) menunjukkan bahwa Linear Regression memberikan hasil yang sangat baik pada data uji, namun ini juga bisa menandakan overfitting jika performanya terlalu sempurna. Model yang terlalu overfitted dapat bekerja dengan sangat baik pada data uji, tetapi kurang optimal pada data baru.

2. Evaluasi Model: XGBoost Regressor
Setelah melakukan hyperparameter tuning menggunakan GridSearchCV, kita melatih kembali model XGBoost Regressor dengan parameter terbaik yang ditemukan. Hasil evaluasinya adalah:

Mean Squared Error (MSE): 10.015
R-squared (R²): 0.9998
Analisis:
Meskipun XGBoost memiliki MSE yang lebih besar dibandingkan Linear Regression, R-squared model XGBoost mendekati nilai sempurna (0.9998), menunjukkan bahwa model ini juga memiliki kemampuan prediksi yang sangat baik dan hampir setara dengan Linear Regression.

Namun, XGBoost biasanya lebih robust terhadap data yang memiliki non-linearitas, sehingga model ini bisa lebih baik dalam menangani data baru yang lebih kompleks dibanding Linear Regression.

Komparasi Model
![image](https://github.com/user-attachments/assets/ede81ddd-8880-421d-9b5b-cae3b6c885ff)

Linear Regression memiliki MSE yang sangat kecil dan R-squared yang sempurna, namun ini bisa menjadi indikasi overfitting, terutama jika data yang dilatih bersifat sangat linear atau terlalu sederhana.
XGBoost memiliki MSE yang sedikit lebih besar dan R-squared yang hampir sempurna, namun model ini lebih fleksibel dalam menangani data yang lebih kompleks.
Kesimpulan dari Komparasi:

XGBoost Regressor mungkin adalah pilihan yang lebih baik jika data nyata memiliki kompleksitas yang lebih tinggi dan tidak selalu mengikuti pola linear.
Sementara Linear Regression lebih sederhana dan memberikan hasil yang baik, model ini mungkin tidak bertahan dengan baik pada data yang lebih bervariasi.
Melalui evaluasi model Linear Regression dan XGBoost Regressor, kita dapat menjawab problem statement ini dengan baik. Kedua model menunjukkan kemampuan prediktif yang tinggi dengan nilai R-squared yang mendekati sempurna. Ini berarti bahwa variabel-variabel seperti jenis pelanggan, jenis produk, dan lokasi cabang memberikan pengaruh yang signifikan terhadap total penjualan dan mampu dijelaskan dengan baik oleh model yang dibangun.

Hasil Evaluasi Model:
Linear Regression memberikan hasil evaluasi dengan R-squared sebesar 1.0, yang menunjukkan bahwa model ini dapat menjelaskan 100% variasi dalam total penjualan.
XGBoost Regressor dengan R-squared sebesar 0.9998 juga hampir sempurna dan lebih robust terhadap kemungkinan variasi dalam data.

