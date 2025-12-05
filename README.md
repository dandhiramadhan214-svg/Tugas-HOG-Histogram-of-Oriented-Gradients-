# Tugas – HOG (Histogram of Oriented Gradients)
Deskripsi

Repository ini berisi implementasi dan penjelasan mengenai Histogram of Oriented Gradients (HOG), sebuah metode ekstraksi fitur yang digunakan dalam komputer visi untuk mendeskripsikan bentuk/struktur pada citra berdasarkan orientasi gradien.

Metode HOG sering digunakan untuk:

Deteksi objek (misalnya deteksi manusia)

Pengenalan pola

Ekstraksi fitur sebelum diterapkan ke model machine learning

Tujuan Tugas

Memahami cara kerja HOG: grayscale → gradient → orientasi → histogram per cell → normalisasi block

Mengimplementasikan HOG menggunakan Python & OpenCV/skimage

Menampilkan hasil visualisasi HOG

Menggunakan fitur HOG sebagai input untuk model/klasifikasi sederhana (opsional)

Struktur Folder
Histogram of Oriented Gradient/
│-- hog.py                # Script utama perhitungan HOG
│-- sample_image.jpg      # Contoh gambar untuk diuji
│-- hasil_hog.png         # Visualisasi HOG (jika ada)
README.md

Cara Menjalankan

Install library yang dibutuhkan:

pip install opencv-python scikit-image matplotlib numpy


Jalankan script:

python hog.py


Hasil gradien & visualisasi HOG akan tampil atau tersimpan sebagai file.

Penjelasan Singkat Cara Kerja HOG

Convert ke grayscale

Hitung gradien (arah & magnitude)

Bagi gambar menjadi cell (misal 8×8 pixel)

Hitung histogram orientasi pada tiap cell

Normalisasi block (untuk mengatasi perubahan cahaya)

Gabungkan semua histogram menjadi feature vector

Hasil

Contoh visualisasi HOG:

Referensi

Dalal & Triggs (2005), Histograms of Oriented Gradients for Human Detection

Dokumentasi Scikit-Image: HOG Feature Descriptor
