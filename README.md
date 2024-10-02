# predictive-analysis-dicoding

# Latar Belakang

Latar belakang pembuatan predictive analysis untuk prediksi BMI didasarkan pada kebutuhan akan alat yang dapat membantu individu dan profesional kesehatan dalam memantau status kesehatan seseorang. BMI (Body Mass Index) adalah indikator yang banyak digunakan untuk menentukan apakah seseorang memiliki berat badan ideal, kekurangan berat badan, kelebihan berat badan, atau obesitas, yang semuanya berhubungan dengan risiko kesehatan seperti penyakit jantung, diabetes, dan hipertensi.

# Business Understanding
Pengembangan model prediksi BMI (Body Mass Index) berdasarkan data tinggi dan berat badan memiliki potensi untuk memberikan manfaat bagi berbagai pihak, termasuk individu yang ingin menjaga kesehatan dan ahli gizi. Model ini dapat membantu meningkatkan kesadaran tentang status kesehatan, memberikan rekomendasi terkait berat badan yang ideal, serta membantu dalam perencanaan diet. Dengan prediksi BMI yang akurat, individu dapat melakukan pemantauan kesehatan dan mencegah risiko penyakit terkait obesitas.

# Problem Statements
Berdasarkan latar belakang di atas, berikut ini merupakan rincian masalah yang dapat diselesaikan pada proyek ini:

1.Bagaimana cara membuat model machine learning yang dapat memprediksi BMI berdasarkan data tinggi badan dan berat badan?</br>
2.Model seperti apa yang memiliki akurasi terbaik dalam memprediksi BMI?</br>
3.Bagaimana model ini dapat membantu individu dan ahli gizi dalam memantau dan meningkatkan kesehatan?

# Data UnderStanding
source data => https://www.kaggle.com/datasets/burnoutminer/heights-and-weights-dataset
# Variabel-variabel pada Data ialah :
height : Tinggi Badan
Weight : Berat badan

# Data Preparation
  ## Crawling Data
  Menyiapkan data yang akan di analysis prediksi.
  ## Cleaning Data
     Cleaning data pada proses ini data dilakukan pengecekan duplikasi data , data null, dan outlier pada data
     proses cleaning data ini sangat penting dilakukan karena akan menjadi hasil yang buruk apabila proses ini dilewati
     ![image](https://github.com/user-attachments/assets/eb925291-1930-467e-ad68-1e4960ed58f3)

  ## Standarization Data
     Mengubah skala data agar lebih konsisten
# Modeling
Saya memilih metode regresi dalam proyek ini karena data yang saya miliki terdiri dari 25.000 sampel yang hanya mencakup dua variabel, yaitu tinggi badan dan berat badan. Regresi sangat cocok untuk menganalisis hubungan antara dua variabel numerik dan memungkinkan saya untuk membuat prediksi terkait nilai Body Mass Index (BMI) berdasarkan tinggi dan berat badan seseorang.

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
Penjelasan mengenai metrik yang digunakan:

BMI (Body Mass Index): BMI dihitung dari berat badan dan tinggi badan seseorang, dengan kategori seperti kekurangan berat badan, berat badan normal, kelebihan berat badan, dan obesitas. Dalam kasus ini, BMI normal adalah antara 18,5 hingga 24,9.
Distribusi berat badan normal dan tidak: Grafik batang akan menunjukkan jumlah individu dalam setiap kategori (normal dan tidak normal). Kamu bisa mengklasifikasikan hasil prediksi BMI ke dalam kelompok "normal" (BMI 18.5–24.9) dan "tidak normal" (kurang dari 18.5 atau lebih dari 24.9).
Menjelaskan hasil proyek berdasarkan metrik evaluasi:

Interpretasi grafik: Jika batang untuk kategori berat badan normal lebih tinggi, itu menunjukkan bahwa mayoritas individu dalam dataset berada dalam rentang BMI sehat. Jika batang kategori "tidak normal" lebih tinggi, itu menandakan lebih banyak individu dengan BMI di luar rentang sehat (baik kekurangan berat badan, kelebihan berat badan, atau obesitas).
Manfaat prediktif: Hasil ini dapat digunakan untuk memberikan panduan kepada individu atau ahli gizi tentang populasi dengan risiko kesehatan berdasarkan prediksi BMI, membantu mereka membuat keputusan terkait program kesehatan atau pola makan yang lebih baik.
Kesimpulan:

Model prediksi BMI ini memberikan gambaran yang jelas tentang distribusi berat badan dalam populasi berdasarkan kategori BMI.
![image](https://github.com/user-attachments/assets/940a44ed-9c15-4aca-8cc8-468a0170f32d)
