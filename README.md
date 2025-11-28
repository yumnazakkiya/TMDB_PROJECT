# 🚀 Automated Movie Genre Classification using NLP & ML
# 1.📖 Overview (Tujuan dan Dampak)
Proyek end-to-end Data Science ini bertujuan membangun sistem klasifikasi genre film otomatis (Horror, Romance, Action, Comedy) berbasis sinopsis teks.

Model yang dikembangkan dirancang untuk efisiensi content tagging, meminimalkan ketergantungan pada data entry manual. Kami membandingkan performa model Machine Learning (ML) Klasik vs. Deep Learning (DL) untuk mengidentifikasi solusi yang paling efisien, siap deploy, dan akurat.

Stack Teknologi Inti: Python, Scikit-learn, Keras/TensorFlow, NLTK, TMDb API.
# 2.⚙️ Metodologi Proyek (Teknis)
Proyek ini mengikuti siklus Data Science penuh, dari akuisisi data hingga evaluasi model.
A. Data Acquisition & Preprocessing
* Data Source: Mengambil 10.500+ sinopsis film unik dari TMDb API, lengkap dengan metadata (rating, popularitas).
* NLP Pipeline: Implementasi preprocessing teks komprehensif: Normalisasi (lowercase), penghapusan tanda baca, dan Stopword Removal menggunakan NLTK.
* Validasi Kualitas: Memastikan dataset bersih dengan 0 Missing Values dan distribusi genre yang seimbang.
B. Feature Engineering & ModelingVektorisasi: Mengubah teks menjadi fitur numerik menggunakan TF-IDF (Term Frequency-Inverse Document Frequency), dengan batasan 5.000 fitur terpenting.Model Komparasi: Dilatih dan diuji 8 model klasifikasi (termasuk Logistic Regression, SVM, Random Forest, dan DL Models seperti LSTM/GRU).
# 3.📈 Hasil Kunci (Kuantitas dan Kualitas)
Analisis kinerja menunjukkan bahwa model klasik, yang dikombinasikan dengan fitur TF-IDF yang kuat, mencapai hasil optimal.
|Model Terbaik|Akurasi (Accuracy)Kinerja Utama & Dampak|
|  ----  |  ----  |  ----  |
|Logistic Regression|70.0%|Puncak Akurasi. Bukti bahwa kualitas fitur TF-IDF menghasilkan classifier yang sangat efisien.|
|SVM|68.1%|Model Klasik terkuat kedua.|
|LSTM|62.0%|Model Deep Learning terbaik, menunjukkan bahwa model klasik lebih optimal pada skala data ini.|
Dampak: Hasil ini menegaskan bahwa solusi berbasis Logistic Regression adalah pilihan yang paling efisien, ringan, dan siap deploy, karena secara signifikan mengungguli model Deep Learning yang membutuhkan lebih banyak sumber daya komputasi.
