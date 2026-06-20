# Manipulasi Citra Digital Menggunakan OpenCV
Repositori ini berisi eksperimen manipulasi citra digital menggunakan Python dan OpenCV. Eksperimen meliputi pembacaan citra, konversi warna BGR ke RGB, resize citra, image blending, image negative, transformasi logaritmik, dan transformasi gamma. Tujuan project ini adalah untuk memahami bagaimana perubahan nilai pixel dapat memengaruhi tampilan visual citra, brightness, contrast, dan detail citra.

## Identitas Mahasiswa
* **Nama Lengkap:** Amira Fathinah
* **NIM:** 452024618075
* **Program Studi:** Teknik Informatika C1
* **Semester:** 5
* **Mata Kuliah:** Pengolahan Sinyal Digital

## Tujuan Eksperimen
Eksperimen ini bertujuan untuk memahami dasar-dasar manipulasi citra digital menggunakan Python dan OpenCV, mulai dari pembacaan citra hingga penerapan beberapa transformasi citra sederhana. Fokus utama eksperimen ini adalah melihat bagaimana operasi matematis pada pixel dapat mengubah karakteristik visual citra seperti warna, brightness, contrast, dan detail.

Secara umum, eksperimen ini mencakup:
- Membaca dan menampilkan citra menggunakan OpenCV
- Melakukan konversi warna dari BGR ke RGB
- Melakukan resize dua citra agar memiliki ukuran yang sama
- Menerapkan image blending dengan beberapa bobot
- Menerapkan image negative
- Menerapkan transformasi logaritmik
- Menerapkan transformasi gamma
- Menganalisis efek setiap transformasi terhadap citra

## Bagian A: Membaca Citra dan Konversi Warna

Bagian ini membahas proses membaca dua citra berbeda menggunakan OpenCV. Setelah citra dibaca, dilakukan konversi warna dari format BGR ke RGB agar citra dapat ditampilkan dengan benar menggunakan Matplotlib.

Pada tahap ini, hasil yang diamati meliputi:
- citra asli sebelum konversi
- citra setelah konversi BGR ke RGB
- ukuran citra menggunakan `shape`
- tipe data citra
- nilai minimum dan maksimum pixel

## Bagian B: Resize Citra

Bagian ini membahas proses menyamakan ukuran dua citra menggunakan fungsi `cv.resize()`. Resize diperlukan karena dua citra harus memiliki ukuran yang sama sebelum dilakukan image blending.

Pada tahap ini, diamati:
- ukuran citra sebelum resize
- ukuran citra setelah resize
- perubahan visual citra setelah dilakukan resize

## Bagian C: Image Blending

Bagian ini membahas penggabungan dua citra menggunakan image blending dengan bobot tertentu. Eksperimen dilakukan menggunakan beberapa kombinasi nilai bobot untuk melihat pengaruh dominasi masing-masing citra terhadap hasil akhir.

Kombinasi bobot yang diuji:
- α = 0.2 dan β = 0.8
- α = 0.5 dan β = 0.5
- α = 0.8 dan β = 0.2

Pada tahap ini, hasil blending dibandingkan untuk melihat perbedaan visual dan dominasi citra berdasarkan bobot yang digunakan.

## Bagian D: Image Negative

Bagian ini membahas transformasi image negative dengan membalik nilai intensitas pixel menggunakan persamaan `255 - I`. Hasil transformasi ini menunjukkan perubahan visual yang berlawanan dengan citra asli.

Pada tahap ini, diamati:
- citra asli
- citra negatif
- histogram citra asli
- histogram citra negatif

## Bagian E: Transformasi Logaritmik

Bagian ini membahas transformasi logaritmik yang digunakan untuk menonjolkan detail pada area gelap citra. Transformasi ini mengubah distribusi pixel sehingga area gelap menjadi lebih terlihat.

Pada tahap ini, diamati:
- citra asli
- citra hasil transformasi logaritmik
- histogram citra asli
- histogram citra hasil transformasi logaritmik
- perbandingan nilai minimum dan maksimum pixel sebelum dan sesudah transformasi

## Bagian F: Transformasi Gamma

Bagian ini membahas transformasi gamma dengan beberapa nilai gamma berbeda untuk melihat pengaruhnya terhadap tingkat kecerahan citra. Nilai gamma yang diuji adalah:
- γ = 0.5
- γ = 1
- γ = 2
- γ = 2.5

Pada tahap ini, diamati:
- citra asli
- citra hasil transformasi gamma untuk setiap nilai gamma
- histogram masing-masing hasil transformasi
- tabel perbandingan efek nilai gamma

## Bagian G: Analisis HOTS dan Studi Kasus

Bagian ini berisi analisis perbandingan empat teknik manipulasi citra, yaitu:
- image blending
- image negative
- transformasi logaritmik
- transformasi gamma

Selain itu, dilakukan analisis pengambilan keputusan untuk memilih teknik yang paling sesuai berdasarkan kondisi citra. Studi kasus yang dibahas berfokus pada citra yang terlalu gelap, citra medis dengan detail samar, serta penggabungan foto dan tekstur visual menggunakan blending.

## Bagian H: Refleksi Pribadi

Bagian ini berisi refleksi pribadi setelah mengerjakan eksperimen manipulasi citra. Refleksi mencakup teknik yang paling mudah dipahami, teknik yang paling menantang, perbedaan antara transformasi logaritmik dan gamma, pemahaman baru tentang nilai pixel, serta teknik yang paling mungkin dipilih jika membuat aplikasi peningkatan kualitas citra.

## Citra yang Digunakan
Project ini menggunakan dua citra digital berbeda yang disimpan di folder `images/`. Kedua citra digunakan untuk eksperimen resize, blending, dan analisis transformasi citra.

Contoh file citra:
- `image1.jpg`
- `image2.jpg`

## Library yang Digunakan
Project ini menggunakan library Python berikut:
- **OpenCV** untuk membaca dan memproses citra
- **NumPy** untuk manipulasi data pixel
- **Matplotlib** untuk visualisasi citra dan histogram

## Cara Menjalankan Notebook
1. Clone repository ini ke komputer kamu.
2. Pastikan Python sudah terpasang.
3. Install library yang dibutuhkan menggunakan perintah berikut:

```bash
pip install -r requirements.txt
