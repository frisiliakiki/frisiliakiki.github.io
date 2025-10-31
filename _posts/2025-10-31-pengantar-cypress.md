---
layout: post
title: "08 Pengantar Cypress"
date: 2025-10-31 09:00:00 +0800
categories: [Sistem Informasi, Software Testing]
tags: [cypress, end-to-end, testing, javascript, frontend]
author: Frisilia Kiki
---
![Pengantar Cypress](../assets/img/posts/08.jpg)


## I. Apa Itu Cypress?

Cypress adalah framework end-to-end testing (E2E) modern yang dirancang khusus untuk aplikasi web modern (seperti yang dibangun dengan React, Vue, atau Angular).

Cypress memposisikan dirinya di semua level pengujian, mulai dari Unit Testing, Integration Testing, hingga End-to-End Testing, dengan fokus utamanya adalah mensimulasikan interaksi pengguna secara real-time di browser.

## II. Keunggulan Cypress

Cypress sering dianggap unggul dari alat testing lama seperti Selenium karena arsitekturnya yang berbeda (berjalan di dalam browser).

### Keunggulan Cypress

| Keunggulan            | Deskripsi                                                                 |
|------------------------|---------------------------------------------------------------------------|
| Arsitektur Modern      | Berjalan di browser (bukan di luar), menghilangkan masalah sinkronisasi yang sering ditemui pada framework lama. |
| Test Runner Interaktif | Menyediakan dashboard visual yang menunjukkan state aplikasi selama tes berjalan. |
| Time Travel            | Pengembang dapat menggeser kursor waktu di Test Runner untuk melihat setiap langkah pengujian, mempermudah debugging. |
| Automatic Waits        | Cypress secara otomatis menunggu elemen muncul atau transisi selesai, menghilangkan kebutuhan untuk menambahkan perintah wait manual. |
| Setup Mudah            | Hanya membutuhkan Node.js dan dapat diinstal dengan cepat melalui NPM.   |

## III. Perintah Dasar Cypress

Cypress memiliki perintah yang intuitif (mudah dipahami) dan menyerupai perilaku pengguna asli:

| Perintah              | Fungsi                                   |
|-----------------------|------------------------------------------|
| `cy.visit('URL')`     | Membuka halaman web.                    |
| `cy.click()`          | Mengklik tombol atau link.              |
| `cy.get('selector')`  | Mengambil elemen berdasarkan selector (e.g., ID atau Class). |
| `cy.contains('text')` | Mengambil elemen berdasarkan teks yang terkandung di dalamnya. |
| `cy.type('text')`     | Mengetik teks ke dalam input field.     |
| `cy.url()`            | Mendapatkan URL aktif saat ini.         |

## IV. Contoh Test Case (Studi Kasus Login)

Cypress sangat efektif dalam menangani skenario login positif (sukses) maupun negatif (gagal).

| ID    | Test Case                     | Steps                                                                 | Expected Result                              |
|-------|-------------------------------|----------------------------------------------------------------------|----------------------------------------------|
| TC01  | Login dengan kredensial valid | Masukkan username & password valid → Klik login                     | Berhasil masuk ke halaman inventory.         |
| TC02  | Login dengan password salah   | Masukkan username valid & password salah → Klik login               | Muncul error "Username and password do not match". |
| TC03  | Login dengan username kosong  | Kosongkan username → Masukkan password → Klik login                 | Muncul error "Username is required".         |

## V. Kesimpulan

Cypress adalah alat yang andal untuk meningkatkan kualitas dan keandalan aplikasi web Anda. Dengan fitur **Time Travel** dan **Automatic Waits**, ia mempermudah pengujian berbasis UI secara cepat dan efisien, menjadikannya pilihan utama untuk End-to-End Testing aplikasi web modern.