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


# Data UnderStanding
source data => https://www.kaggle.com/datasets/aungpyaeap/supermarket-sales
# Variabel-variabel pada Data ialah :
Invoice ID<br>
Branch
City
Customer type
Gender
Product line
Unit price
Quantity
Tax 5%	
Total	Date	
Time	
Payment	cogs	
gross margin percentage
gross income	
Rating

# Data Preparation
  ## Crawling Data
  Menyiapkan data yang akan di analysis prediksi.
  ## Cleaning Data
     Cleaning data pada proses ini data dilakukan pengecekan duplikasi data , data null, dan outlier pada data
     proses cleaning data ini sangat penting dilakukan karena akan menjadi hasil yang buruk apabila proses ini dilewati
![image](https://github.com/user-attachments/assets/ae761e27-5cae-4054-a15e-bd25a576bd74)


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
Evaluasi model adalah langkah krusial dalam proses pemodelan yang bertujuan untuk mengukur seberapa baik model melakukan prediksi terhadap data yang belum pernah dilihat sebelumnya. Dalam konteks regresi, beberapa metrik evaluasi umum digunakan untuk menilai kinerja model, antara lain:

Mean Squared Error (MSE):

MSE mengukur rata-rata kuadrat dari kesalahan antara nilai yang diprediksi dan nilai aktual. Metrik ini memberikan gambaran seberapa besar kesalahan prediksi model secara keseluruhan. MSE yang lebih rendah menunjukkan bahwa model lebih akurat dalam memprediksi total penjualan.
Mean Absolute Error (MAE):

MAE mengukur rata-rata dari nilai absolut dari kesalahan antara prediksi dan nilai aktual. MAE memberikan gambaran tentang seberapa besar kesalahan prediksi dalam satuan yang sama dengan variabel target. Ini berguna untuk memahami rata-rata kesalahan yang mungkin terjadi.
Root Mean Squared Error (RMSE):

RMSE adalah akar kuadrat dari MSE dan memberikan ukuran kesalahan dalam satuan yang sama dengan variabel target. RMSE sering digunakan karena memberikan penalti yang lebih besar untuk kesalahan yang lebih besar, sehingga lebih sensitif terhadap outlier.
R-squared (R²):

R-squared mengukur proporsi variabilitas dalam data target yang dapat dijelaskan oleh model. Nilai R-squared berkisar antara 0 dan 1, di mana nilai yang lebih dekat ke 1 menunjukkan bahwa model mampu menjelaskan sebagian besar variasi dalam data. R² yang tinggi menunjukkan bahwa model sangat baik dalam memprediksi total penjualan.
Kesimpulan Evaluasi
Dengan menggunakan metrik-metrik ini, model regresi yang telah dilatih dapat dinilai secara komprehensif. Hasil evaluasi menunjukkan seberapa baik model dapat memprediksi total penjualan berdasarkan variabel-variabel yang relevan. Metrik yang baik dan hasil evaluasi yang positif menandakan bahwa model dapat diandalkan untuk memberikan insight dan prediksi yang bermanfaat bagi pengambilan keputusan bisnis.

![image](https://github.com/user-attachments/assets/895830b7-f639-4605-b288-5a95d3be3f37)

