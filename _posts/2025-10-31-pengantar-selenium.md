---
layout: post
title: "07 Pengantar Selenium WebDriver"
date: 2025-10-31 09:00:00 +0800
categories: [Sistem Informasi, Software Testing]
tags: [selenium, webdriver, automation, python, end-to-end]
author: Frisilia Kiki
---
![Pengantar Selenium](../assets/img/posts/07.jpg)


## I. Apa Itu Selenium dan Selenium WebDriver?

### A. Apa itu Selenium?

Selenium adalah framework open-source yang digunakan untuk automasi browser. Fungsinya adalah menguji aplikasi web dengan mensimulasikan interaksi pengguna nyata, seperti klik, input teks, dan navigasi.

- Mendukung banyak bahasa pemrograman (Python, Java, C#, PHP, Ruby).
- Mendukung banyak browser (Chrome, Firefox, Edge, Safari).

### B. Apa itu Selenium WebDriver?

WebDriver adalah komponen inti dari Selenium. Ia bertindak sebagai jembatan yang menghubungkan kode skrip pengujian yang Anda tulis dengan browser yang sedang berjalan.

- WebDriver mengontrol browser (melakukan klik, input teks, navigasi, dan validasi).
- Workflow utamanya adalah:  
  **Test Scripts (kode kita) → WebDriver (jembatan) → Browser (target pengujian).**

## II. Mengapa Harus Menggunakan Selenium?

Selenium telah menjadi standar industri untuk pengujian otomatis aplikasi web karena beberapa keunggulan:

- **Open-Source dan Gratis**: Dapat digunakan oleh siapa saja tanpa biaya lisensi.
- **Dukungan Multi-Bahasa**: Fleksibel karena mendukung bahasa pemrograman yang berbeda.
- **Multi-Platform**: Berjalan di berbagai sistem operasi (Windows, macOS, Linux).
- **Integrasi Kuat**: Mudah diintegrasikan dengan framework pengujian lainnya seperti Pytest atau JUnit untuk membuat kerangka pengujian yang komprehensif.
- **Komunitas Besar**: Memiliki komunitas pengguna yang luas dan dokumentasi yang lengkap, memudahkan pemecahan masalah.

## III. Contoh Test Scenario dan Test Case

Selenium biasanya digunakan untuk menguji alur pengguna secara end-to-end (E2E) pada aplikasi web. Berikut adalah contoh Test Scenario dan Test Case untuk menguji fitur Login dan Shopping Cart:

### A. Test Scenario

| ID      | Deskripsi                                |
|---------|------------------------------------------|
| TS-001  | Login berhasil di halaman e-commerce tertentu. |
| TS-002  | Login gagal dengan kredensial salah.     |
| TS-003  | Menambahkan produk ke keranjang belanja. |

### B. Test Case (Contoh Login)

| ID      | Deskripsi         | Steps                                                                 | Expected Result                          |
|---------|-------------------|----------------------------------------------------------------------|------------------------------------------|
| TC-001  | Login sukses      | 1. Input username valid (e.g., standard_user).<br>2. Input password valid (e.g., secret_sauce).<br>3. Klik tombol "Login". | Masuk ke halaman inventory.              |
| TC-002  | Login gagal       | 1. Input username salah.<br>2. Input password salah.<br>3. Klik tombol "Login". | Muncul pesan error yang sesuai.          |
| TC-003  | Tambah produk ke cart | 1. Login sukses.<br>2. Klik tombol "Add to cart" pada produk.         | Cart bertambah 1 dan notifikasi muncul.  |