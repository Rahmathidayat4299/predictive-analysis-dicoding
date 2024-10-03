# Predictive-analysis-dicoding
# Domain project ialah keuangan dengan judul Predictive Analysis Prediksi Sales Supermarket
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
source data => https://www.kaggle.com/datasets/aungpyaeap/supermarket-sales
# Variabel-variabel pada Data ialah :
Invoice ID: String (atau kategori) - Merupakan identifikasi unik untuk setiap transaksi dan biasanya dalam format teks.<br>
Branch: Kategori - Menunjukkan cabang tempat transaksi dilakukan, biasanya berupa huruf (misalnya, A, B, C).<br>
City: Kategori - Menunjukkan nama kota tempat cabang berlokasi, berupa teks.<br>
Customer type: Kategori - Mengindikasikan tipe pelanggan, biasanya berupa kategori seperti "Member" atau "Normal".<br>
Gender: Kategori - Menunjukkan jenis kelamin pelanggan, biasanya berupa "Male" atau "Female".<br>
Product line: Kategori - Mengindikasikan kategori produk yang dibeli, berupa teks (misalnya, "Health and beauty").<br>
Unit price: Float - Menunjukkan harga per unit produk, berupa angka desimal.<br>
Quantity: Integer - Menunjukkan jumlah produk yang dibeli, berupa angka bulat.<br>
Tax 5%: Float - Menunjukkan pajak yang dikenakan (5% dari total harga), berupa angka desimal.<br>
Total: Float - Menunjukkan total harga setelah pajak, berupa angka desimal.<br>
Date: Tanggal - Menunjukkan tanggal transaksi, biasanya dalam format teks yang dapat diubah menjadi tipe tanggal.<br>
Time: Waktu - Menunjukkan waktu transaksi, biasanya dalam format teks (jam)<br>
Payment: Kategori - Menunjukkan metode pembayaran yang digunakan (misalnya, "Ewallet", "Cash").<br>
cogs: Float - Menunjukkan biaya barang yang terjual (Cost of Goods Sold), berupa angka desimal.<br>
gross margin percentage: Float - Menunjukkan persentase margin kotor, berupa angka desimal.<br>
gross income: Float - Menunjukkan total pendapatan kotor, berupa angka desimal.<br>
Rating: Float - Menunjukkan rating yang diberikan oleh pelanggan, biasanya dalam skala 1-10, berupa angka desimal.<br>

# Data Preparation
  ## Crawling Data
  Menyiapkan data yang akan di analysis prediksi.
  ## Cleaning Data
     Cleaning data pada proses ini data dilakukan pengecekan duplikasi data , data null, dan outlier pada data
     proses cleaning data ini sangat penting dilakukan karena akan menjadi hasil yang buruk apabila proses ini dilewati
![image](https://github.com/user-attachments/assets/27e9c67e-a695-4409-8b63-c4e9b5ca6b1d)
berikut jumlah outlier pada dataset
![image](https://github.com/user-attachments/assets/3dd63248-a440-4bf0-9f77-bfd2b1f1f6b4)




  ## Standarization Data
     Mengubah skala data agar lebih konsisten

## Modeling: Regresi
Dalam proyek ini, model regresi digunakan untuk memprediksi total penjualan berdasarkan kombinasi variabel yang berpengaruh, seperti jenis pelanggan, jenis produk, dan lokasi cabang. Regresi adalah teknik analisis statistik yang memungkinkan kita untuk memahami hubungan antara satu variabel dependen (dalam hal ini, total penjualan) dan satu atau lebih variabel independen (fitur yang mempengaruhi penjualan).

Mengapa Memilih Regresi?
Keterhubungan yang Jelas: Regresi sangat berguna ketika ada harapan bahwa variabel independen akan memiliki pengaruh yang signifikan terhadap variabel dependen. Dalam konteks ini, kami percaya bahwa faktor-faktor seperti jenis pelanggan dan jenis produk dapat memengaruhi total penjualan.

Prediksi Nilai Kontinu: Total penjualan adalah variabel kontinu yang dapat diprediksi dengan baik menggunakan model regresi. Ini memungkinkan perusahaan untuk meramalkan penjualan di masa depan berdasarkan faktor-faktor yang telah dianalisis.

Interpretabilitas: Model regresi memberikan koefisien untuk setiap fitur, yang memungkinkan analisis mendalam tentang seberapa besar setiap faktor memengaruhi total penjualan. Ini memberikan wawasan yang dapat diterapkan dalam pengambilan keputusan bisnis.

Jenis Regresi yang Digunakan
Regresi Linier: Digunakan untuk model dasar yang memberikan gambaran awal tentang hubungan antara variabel. Ini berguna untuk memahami pola umum dalam data.

Regresi XGBoost: Model ini diterapkan setelah pengujian regresi linier untuk mendapatkan hasil yang lebih akurat dan mempertimbangkan interaksi antara fitur. XGBoost adalah algoritma boosting yang dikenal karena kemampuannya dalam menangani kompleksitas data dan memberikan prediksi yang lebih baik.

Proses Modeling
Pemisahan Data: Dataset dibagi menjadi dua bagian: data pelatihan dan data pengujian. Model dilatih menggunakan data pelatihan dan dievaluasi menggunakan data pengujian.

Pelatihan Model: Model regresi dilatih dengan menggunakan variabel independen untuk memprediksi total penjualan.

Evaluasi Model: Model dievaluasi dengan metrik seperti Mean Squared Error (MSE), Mean Absolute Error (MAE), dan R-squared untuk mengukur kinerja model.

Hyperparameter Tuning: Untuk meningkatkan performa model, hyperparameter tuning dilakukan menggunakan teknik seperti Grid Search untuk menemukan kombinasi parameter terbaik.

Hasil
Model regresi XGBoost menunjukkan hasil yang sangat baik dengan nilai R-squared mendekati 1, menunjukkan bahwa model mampu menjelaskan hampir semua variabilitas dalam data. Dengan menggunakan model ini, perusahaan dapat membuat proyeksi penjualan yang lebih akurat dan mengambil langkah strategis yang tepat untuk meningkatkan kinerja penjualan.

Regresi linier sederhana dapat menangkap hubungan linier antara dua variabel tersebut secara efektif dan memberikan interpretasi yang mudah dipahami. Dengan data terbatas hanya pada tinggi dan berat, regresi merupakan pilihan yang tepat karena mampu menghasilkan model prediktif dengan akurasi yang baik dan tidak memerlukan fitur tambahan atau algoritma yang lebih kompleks.
  ## Kelebihan Regresi:
      Sederhana dan mudah diimplementasikan: Regresi linier mudah dipahami dan digunakan.
      Interprestasi yang jelas: Hasil regresi memberikan informasi yang jelas tentang hubungan antara variabel independen dan dependen.
      Performa baik untuk data linier: Bekerja baik jika ada hubungan linier antara variabel.
  ## Kekurangan Regresi:

      Sensitif terhadap outlier: Regresi sangat terpengaruh oleh data outlier yang dapat menyebabkan model menjadi tidak akurat.
      Keterbatasan untuk data non-linier: Regresi linier tidak mampu menangani hubungan non-linier tanpa penyesuaian khusus.
      Multikolinearitas: Jika fitur saling berkorelasi, hasil regresi bisa menjadi tidak stabil.
# Evaluation
* Jawaban dari goals
* ![image](https://github.com/user-attachments/assets/0fda6e0f-b4f2-4731-bc97-f58b01facb24)

Memahami Faktor yang Mempengaruhi Penjualan:

Melalui analisis data, model regresi XGBoost menunjukkan bahwa kombinasi variabel seperti jenis pelanggan, jenis produk, dan lokasi cabang memiliki pengaruh signifikan terhadap total penjualan. Misalnya, model dapat mengidentifikasi bahwa jenis produk tertentu lebih populer di lokasi cabang tertentu, dan bahwa pelanggan dengan profil tertentu cenderung melakukan pembelian dengan nilai yang lebih tinggi.
Pengembangan Model Prediksi:

Dengan melatih model regresi menggunakan dataset yang mencakup variabel-variabel kunci, kami berhasil membangun model yang dapat memprediksi total penjualan dengan akurasi tinggi. Hasil evaluasi menunjukkan Mean Squared Error (MSE) yang rendah dan R-squared yang sangat tinggi (0.9999), yang menunjukkan kemampuan model dalam menjelaskan variabilitas penjualan.
Pengambilan Keputusan Berbasis Data:

Hasil dari model prediksi memberikan dasar yang kuat bagi manajemen untuk membuat keputusan strategis. Misalnya, jika model menunjukkan bahwa penjualan meningkat pada jenis pelanggan tertentu selama periode tertentu, perusahaan dapat memfokuskan upaya pemasaran dan penjualan kepada segmen tersebut untuk memaksimalkan pendapatan.
Optimisasi Strategi Pemasaran:

Dengan wawasan yang diperoleh dari model prediksi, perusahaan dapat mengoptimalkan strategi pemasaran mereka. Misalnya, jika analisis menunjukkan bahwa jenis produk A lebih banyak dibeli oleh pelanggan B di cabang C, perusahaan dapat merancang promosi khusus atau penawaran untuk menarik lebih banyak pelanggan di segmen ini. Selain itu, hasil model dapat digunakan untuk merencanakan stok produk secara lebih efektif, menghindari kehabisan stok atau overstocking.

![image](https://github.com/user-attachments/assets/895830b7-f639-4605-b288-5a95d3be3f37)

