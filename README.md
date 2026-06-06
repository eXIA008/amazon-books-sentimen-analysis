<h1 align="center"> Analisis Sentimen Ulasan Pelanggan Amazon Books 
dengan Logistic Regression </h1>

## ⭐ About The Project
Proyek ini bertujuan untuk membangun model *Machine Learning* yang mampu mengklasifikasikan sentimen pada ulasan Buku menggunakan dataset [Amazon US Customer Reviews Dataset](https://www.kaggle.com/datasets/cynthiarempel/amazon-us-customer-reviews-dataset/data?select=amazon_reviews_us_Books_v1_02.tsv).

## 👨🏻‍💻 Team
* Arya Wijaya                             103012330330
* Ghanif Hadiyana Akbar                   103012300018
* Daisaq Hadya Albar                      103012300158 
* Muhammad Zaini                          103012300313

## 🚀 How to Run
Proyek ini dibangun menggunakan Apache Spark (PySpark) untuk menangani pemrosesan Big Data. Karena ukuran dataset yang sangat besar, sangat direkomendasikan untuk menjalankan notebook ini menggunakan Google Colab agar terhindar dari masalah memori (RAM) pada perangkat lokal.

Prasyarat (Prerequisites)
Jika Anda ingin menjalankan secara lokal, pastikan Anda telah menginstal:
- Python 3.8+
- Apache Spark & PySpark
- Library: matplotlib, seaborn, scikit-learn
- Akun Kaggle (untuk mengunduh dataset).

Opsi 1: Menjalankan via Google Colab
1. Buka Notebook di Colab:
Unduh file Sentimen_Sigmoid_StepByStep_Run.ipynb dari repositori ini, lalu unggah ke Google Colab.

2. Persiapkan Token Kaggle (Kaggle API):
   - Notebook ini mengunduh dataset secara otomatis dari Kaggle.
   - Pastikan Anda memiliki file kaggle.json. (Cara mendapatkan: Login Kaggle -> Settings -> Create New Token).
   - Saat Anda menjalankan sel/blok kode pertama, sistem akan meminta Anda untuk mengunggah file kaggle.json ini.

3. Jalankan Notebook:
   - Klik Runtime pada menu atas Colab, lalu pilih Run All (atau jalankan sel satu per satu secara berurutan Shift + Enter).
   - Tunggu hingga Spark selesai mengunduh dataset amazon_reviews_us_Books_v1_02.tsv dan melakukan pemrosesan.

Opsi 2: Menjalankan Secara Lokal (Jupyter Notebook)
1. Clone Repositori:
   - ``git clone https://github.com/username_anda/nama_repositori_anda.git``
   - ``cd nama_repositori_anda``
3. Unduh Dataset Manual:
   - Buka tautan dataset di Kaggle: Amazon US Customer Reviews
   - Unduh file spesifik: amazon_reviews_us_Books_v1_02.tsv.
   - Letakkan file tersebut di dalam folder yang sama dengan file .ipynb.
4. Modifikasi Kode Jalur File (Path):
   - Buka file Sentimen_Sigmoid_StepByStep_Run.ipynb di Jupyter Notebook/JupyterLab lokal Anda.
   - Hapus atau comment (beri tanda #) pada blok kode yang berfungsi untuk mengunggah kaggle.json dan mendownload via API.
   - Pastikan variabel file_path mengarah langsung ke nama file yang sudah Anda unduh secara lokal:
     ``file_path = "amazon_reviews_us_Books_v1_02.tsv"``
5. Jalankan Semua Sel
   - Pilih Cell > Run All dari menu navigasi Jupyter.
