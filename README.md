# Modul Interaktif Forward Kinematics Franka Panda 7-DOF

Modul pembelajaran berbasis HTML interaktif untuk mempelajari pemodelan matematis dan perhitungan **Forward Kinematics (FK)** pada robot lengan Franka Emika Panda yang memiliki tujuh derajat kebebasan (*Degrees of Freedom/DOF*).

Modul ini dirancang untuk mendukung pembelajaran robotika, khususnya pemahaman hubungan antara sudut rotasi setiap joint, geometri robot, matriks transformasi, dan posisi serta orientasi *end-effector*.

## Tujuan Pembelajaran

Setelah mempelajari modul ini, mahasiswa diharapkan mampu:

1. Mengidentifikasi struktur robot lengan Franka Panda 7-DOF.
2. Memahami konsep joint, link, sumbu rotasi, dan sistem koordinat robot.
3. Menentukan parameter Modified Denavit–Hartenberg (MDH).
4. Menyusun matriks transformasi homogen untuk setiap joint.
5. Menghitung posisi dan orientasi end-effector menggunakan Forward Kinematics.
6. Menganalisis perubahan konfigurasi robot akibat perubahan sudut joint.
7. Membandingkan hasil perhitungan matematis dengan simulasi robot 3D.

## Fitur Modul

### 1. Materi Matematis

Materi mencakup:
- Konversi sudut derajat ke radian.
- Parameter Modified Denavit–Hartenberg (MDH).
- Matriks transformasi homogen.
- Perkalian matriks transformasi tujuh joint.
- Perhitungan posisi dan orientasi end-effector.
- Perbedaan Forward Kinematics dan Inverse Kinematics.
- Penjelasan offset antara flange dan hand mount.

### 2. Simulator Robot Interaktif

Simulator memungkinkan pengguna untuk:
- Mengubah sudut tujuh joint menggunakan slider.
- Mengamati perubahan konfigurasi lengan robot.
- Mengubah parameter MDH untuk eksperimen matematis.
- Menghitung koordinat posisi X, Y, dan Z.
- Melihat orientasi end-effector.
- Menampilkan matriks transformasi \(T_{07}\).
- Melihat koordinat setiap frame.
- Menjalankan animasi beberapa konfigurasi robot.

### 3. Latihan dan Evaluasi

Modul dilengkapi dengan:
- Latihan perhitungan Forward Kinematics.
- Eksperimen perubahan sudut joint.
- Analisis perbedaan posisi flange dan hand mount.
- Kuis interaktif.
- Rubrik penilaian tugas mahasiswa.

### 4. Soal Tugas Mahasiswa

Mahasiswa diminta membuat model matematis Forward Kinematics robot Franka Panda 7-DOF, meliputi diagram kinematika, parameter MDH, matriks transformasi, perhitungan numerik, serta validasi hasil terhadap simulator robot.

## Cara Menggunakan

1. Buka file `modul_forward_kinematics_franka_panda_interaktif.html`.
2. Jalankan file menggunakan browser modern seperti Google Chrome, Microsoft Edge, atau Firefox.
3. Pelajari materi matematis yang tersedia.
4. Geser slider sudut joint untuk mengubah konfigurasi lengan.
5. Amati perubahan posisi, orientasi, dan matriks transformasi.
6. Kerjakan latihan dan kuis yang tersedia.
7. Gunakan simulator robot Rocksi untuk pengamatan dan perbandingan tambahan.

Modul dapat dijalankan secara lokal tanpa instalasi aplikasi tambahan. Perhitungan interaktif dilakukan menggunakan JavaScript di dalam browser.

## Dasar Matematis

Forward Kinematics menghitung posisi dan orientasi end-effector berdasarkan sudut joint yang diketahui.

Untuk robot Franka Panda dengan tujuh joint, transformasi dari base menuju frame joint ketujuh dinyatakan sebagai:

\[
T_{07}=A_1A_2A_3A_4A_5A_6A_7
\]

Setiap \(A_i\) merupakan matriks transformasi yang dibentuk berdasarkan parameter MDH dan sudut joint terkait.

Hasil transformasi memuat informasi posisi dan orientasi frame akhir terhadap sistem koordinat dasar robot.

## Teknologi

- HTML5
- CSS3
- JavaScript
- Canvas API
- Matriks transformasi homogen
- Modified Denavit–Hartenberg (MDH)

## Catatan dan Batasan

Simulator dalam modul ini merupakan visualisasi edukatif dengan model matematis kinematika robot. Visualisasi tersebut bukan model CAD presisi dan tidak digunakan untuk mengendalikan robot fisik.

Parameter MDH dan definisi kerangka koordinat perlu diverifikasi apabila hasil perhitungan akan dibandingkan secara numerik dengan simulator eksternal, termasuk Rocksi. Posisi frame ketujuh, flange, hand mount, dan ujung gripper dapat berbeda karena offset serta geometri alat.

## Referensi

- [Rocksi – Simulator Robot 3D](https://rocksi.net/)
- [Franka Robotics](https://www.franka.de/)
- [Franka ROS Repository](https://github.com/frankaemika/franka_ros)

## Lisensi

Modul ini dapat digunakan sebagai bahan pembelajaran dan praktikum robotika. Ketentuan penggunaan ulang, modifikasi, dan distribusi mengikuti lisensi yang ditetapkan oleh pemilik repositori.
