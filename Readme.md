=== Klasifikasi Golongan UKT Menggunakan Model MLP dan Algoritma Backpropagation ===

📖 Deskripsi
Proyek ini berfokus pada klasifikasi golongan Uang Kuliah Tunggal (UKT) menggunakan Artificial Neural Network (ANN) dengan arsitektur Multilayer Perceptron (MLP) dan algoritma Backpropagation sebagai metode pembelajaran.

Seluruh proses dilakukan dalam satu file Python Notebook (.ipynb) yang diunggah langsung dari Google Colab ke repository ini. File tersebut memuat seluruh tahapan analisis data mulai dari preprocessing, pelatihan model, hingga evaluasi akhir.

Selain menampilkan model machine learning untuk proses klasifikasi golongan UKT, pada repository ini juga ditampilkan perbandingan hasil akuasi model antara hasil akurasi model jika data pelatihan menggunakan SMOTE dan jika tidak menggunakan SMOTE.

🛠️ Tahapan Analisis Data
1. Eksplorasi Data
  * Pengecekan nilai uniq
  * Pengecekan nilai duplikat
  * Pengecekan nilai tidak valid
  * Pengecekan distribusi statistik
  * Pengecekan nilai hilang
2. Data Preprocessing
  * Label Encoding untuk data kategorikal
  * Penanganan nilai tidak valid pada data numerik
  * Normalisasi dengan model Z-Score pada data numerik
  * Penanganan nilai hilang menggunakan model autoencoder
  * Split data pelatihan (80%) dan data pengujian (20%)
  * Penanganan data inbalance menggunakan teknik oversampling SMOTE pada data pelatihan
3. Pembangunan Model Artificial Neural Network model Multilayer Perceptron
  * Pembangunan arsitektur model MLP secara manual tanpa package
  * Inisiasi hyperparameter
  * Inisiasi bobot awal secara acak
4. Inisiasi Algoritma Backpropagation untuk pembaruan bobot pada proses pelatihan model MLP
  * Inisiasi optimizer Adam dan nilai parameter yang ada pada optimizer Adam
  * Inisiasi parameter cross-entropy yang merupakan fungsi loss dalam proses pembaruan bobot
  * Inisiasi parameter dari gradien loss-entropy dan gradien bobot pada masing-masing neuron pada hidden layer dan output layer
5. Evaluasi Model dan Visualisasi Hasil
  * Confusion Matrix
  * Akurasi skor
  * Grafik dari confusion matrix
  * Grafik perbandingan hasil akurasi model pada pelatihan model dan pengujian model

🛠️ Tools dan Bahasa Pemrograman yang Digunakan
1. Python
  * Numpy
  * Pandas
  * matplotlib.pyplot
  * seaborn
  * sklearn.metrics
  * sklearn.neighbors
  * sklearn.model_selection
2. Google Colab
  * Digunakan sebagai tools untuk bahasa pemrograman Python

📦 repository-ukt-mlp
 ┣ 📜 klasifikasi_ukt_mlp.ipynb   ← File utama dari Google Colab
 ┣ 📜 README.md                   ← Dokumentasi proyek

📈 Bagian Alur Analisis Data
Eksplorasi Dataset Dataset → Data Preprocessing → Pembangunan Model MLP → Backpropagation → Evaluasi → Kesimpulan

📜 Kesimpulan
Penelitian ini melakukan klasifikasi penggolongan UKT dengan metode ANN model MLP. Model MLP dapat mengatasi permasalahan dataset yang besar dan bervariatif serta data inbalance pada dataset mahasiswa UNNES tahun 2024 melalui serangkaian tahapan data preprocessing yang efektif, seperti pelabelan data kategorik dengan label encoding dan pembersihan data pada data numerik, lalu normalisasi pada data numerik dengan model Z-Score, dan inputasi nilai hilang dengan Autoencoder, serta serangkaian turning hyperparameter pada model MLP. Penelitian ini memiliki hasil akurasi model klasifikasi sebesar 88% untuk data pelatihan yang tidak menggunakan SMOTE dan yang menggunakan SMOTE. Hasil akurasi tersebut menunjukan bahwa penggunaan MLP dalam klasifikasi Golongan UKT pada penelitian ini dapat melampaui hasil akurasi model pada penelitian sebelumnya. Kebaruan dari penelitian ini yaitu penerapan autoencoder untuk inputasi nilai hilang dalam data klasifikasi Golongan UKT, memiliki hasil yang efektif dalam mengatasi missing value berdasarkan hasil loss function yang rendah.
