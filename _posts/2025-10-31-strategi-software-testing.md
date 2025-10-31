---
layout: post
title: "01 Strategi Software Testing"
date: 2025-10-31 19:00:00 +0800
categories: [Sistem Informasi, Software Testing]
tags: [software-testing, jekyll, unhas, sdlc, testing-strategy]
author: Frisilia Kiki
---

![Strategi Software Testing](../assets/img/posts/01.jpg)

Halo semua! Kali ini, saya akan merangkum materi penting dari mata kuliah Sistem Informasi 2023, yang membahas secara mendalam mengenai Strategi Testing dalam pengembangan perangkat lunak.

Penting untuk diingat bahwa testing bukan hanya mencari bug, tetapi merupakan tahapan krusial dalam siklus hidup pengembangan (Software Development Life Cycle atau SDLC).

## I. Fase Testing dalam SDLC

Pengembangan perangkat lunak dilakukan melalui tahapan bertahap yang dikenal sebagai Software Development Life Cycle (SDLC). Fase Testing & Integration berada di urutan kelima dalam siklus ini, setelah Planning, Analysis, Design, dan Implementation.

### Apa Itu Testing?

Testing adalah proses mengevaluasi produk perangkat lunak untuk menemukan cacat (defect atau bug) dan memastikan produk bekerja sesuai kebutuhan, baik fungsional maupun non-fungsional.

### Tujuan Utama Testing

Tujuan utama dari Software Testing adalah:
- Menemukan kesalahan atau cacat (bug) dalam perangkat lunak atau sistem.
- Memastikan kualitas produk sebelum produk dirilis.
- Verifikasi dan Validasi: Memastikan perangkat lunak memenuhi spesifikasi.
- Mengurangi Risiko Kegagalan: Meminimalkan kemungkinan kerusakan di lingkungan produksi.
- Meningkatkan Kepercayaan Stakeholder: Memberikan jaminan kualitas kepada pengguna dan pemangku kepentingan.
- Menjamin Keamanan: Mengidentifikasi celah keamanan.
- Efisiensi Biaya: Biaya perbaikan bug di tahap awal lebih murah daripada setelah dirilis.
- Meningkatkan Pengalaman Pengguna (UX).

## II. Software Testing Life Cycle (STLC)

Software Testing Life Cycle adalah pendekatan sistematis untuk menguji perangkat lunak. Proses ini mengikuti serangkaian langkah atau fase, dan setiap fase memiliki tujuan dan hasil yang spesifik. Proses STLC memastikan bahwa software yang dikembangkan berkualitas, andal, dan memenuhi kebutuhan pengguna akhir.

### Fase-fase Utama STLC

#### 1. Test Planning
- Membuat strategi pengujian.
- Mengidentifikasi lingkungan pengujian.
- Memperkirakan waktu dan biaya.

#### 2. Test Design
- Mengidentifikasi dan menulis test case.
- Membuat data dan skenario pengujian.
- Memperbarui dokumen Requirement Traceability Matrix (RTM).

#### 3. Test Execution
- Menjalankan test case di lingkungan pengujian.
- Mencatat hasil tes.

#### 4. Pelaporan & Analisis Testing
- Menyajikan ringkasan hasil (kasus uji berhasil, gagal, atau belum dijalankan).
- Evaluasi kualitas aplikasi terhadap spesifikasi fungsional dan non-fungsional.
- Identifikasi bug dan isu teknis (tingkat keparahan dan status perbaikan).

## III. Klasifikasi Software Testing

Pengujian perangkat lunak dapat diklasifikasikan berdasarkan empat aspek utama: Abstraksi, Fungsi, Domain, dan Struktur.

### A. Berdasarkan Abstraksi (Level Testing)

Klasifikasi ini menguji dari unit terkecil hingga sistem lengkap:
- Unit Testing
  - Fokus: Komponen terkecil (fungsi, metode, kelas).
  - Singkat: Memverifikasi fungsionalitas unit kode secara individual.
- Integration Testing
  - Fokus: Interaksi antar sub-sistem.
  - Singkat: Memastikan modul berbeda bekerja sama dengan benar.
- System Testing
  - Fokus: Sistem secara keseluruhan.
  - Singkat: Menguji sistem holistik terhadap semua persyaratan fungsional dan non-fungsional.
- Acceptance Testing
  - Fokus: Perspektif pengguna akhir (klien).
  - Singkat: Memvalidasi bahwa sistem dapat diterima dan memenuhi kebutuhan bisnis.

### B. Berdasarkan Fungsi

- Functional Testing: Menguji apakah software berfungsi sesuai persyaratan fungsional (misalnya verifikasi login, validasi transaksi).
- Non-Functional Testing: Menguji performa, keamanan, reliabilitas, dan aspek lain non-fungsional (misalnya memastikan website tetap berjalan saat jumlah pengguna melonjak).

### C. Berdasarkan Domain (Contoh Non-Fungsional)

- Performance Testing: Menguji kecepatan, responsivitas, dan stabilitas di bawah beban tertentu.
- Security Testing: Mengidentifikasi celah keamanan (misalnya SQL injection, XSS) untuk melindungi data.
- Usability Testing: Mengevaluasi kemudahan penggunaan perangkat lunak oleh pengguna akhir.

### D. Berdasarkan Struktur

- Black-Box Testing
  - Definisi: Tester tidak mengetahui struktur internal atau kode program.
  - Fokus: Fungsi dan output sistem dari perspektif pengguna akhir.
  - Kelebihan: Tidak perlu detail teknis kode.
- White-Box Testing
  - Definisi: Tester mengetahui struktur internal dan kode program.
  - Fokus: Alur logika, algoritma, dan struktur data di dalam program.
  - Kelebihan: Menjamin cakupan kode lebih luas dan menemukan bug tersembunyi dalam logika program.

## IV. Kesimpulan

Software Testing adalah bagian integral dari SDLC. Dengan menerapkan strategi dan siklus pengujian yang sistematis, kita dapat menghasilkan software yang baik, bebas dari bug yang parah, dan disukai oleh pengguna akhir.