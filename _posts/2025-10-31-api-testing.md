---
layout: post
title: "06 API Testing"
date: 2025-10-31 09:00:00 +0800
categories: [Sistem Informasi, Software Testing]
tags: [api-testing, postman, rest, soap, request, response]
author: Frisilia Kiki
---
![Api Testing](../assets/img/posts/06.jpg)


## I. Apa Itu API Testing?

API Testing adalah proses pengujian yang dilakukan pada Application Programming Interface (API). API berfungsi sebagai perantara komunikasi antar-sistem.

Pengujian ini bertujuan untuk memastikan bahwa:
- API berfungsi sesuai dengan spesifikasi yang ditentukan.
- API dapat menangani berbagai skenario input dengan benar.
- API menghasilkan output yang benar (data atau kode status).

## II. Keunggulan dan Pentingnya API Testing

Pengujian API adalah pondasi penting dalam pengembangan perangkat lunak modern karena API adalah lapisan yang menghubungkan backend (logika bisnis) dengan frontend (antarmuka pengguna).

### Keunggulan API Testing

| Keunggulan            | Deskripsi                                                                 |
|------------------------|---------------------------------------------------------------------------|
| Meningkatkan Keandalan | Mendeteksi bug di lapisan bisnis (server) sejak awal pengembangan, jauh sebelum bug tersebut memengaruhi antarmuka pengguna. |
| Menjamin Keamanan      | Memastikan API terlindungi dari akses tidak sah, injection, atau potensi celah keamanan. |
| Mengukur Performa      | Mengukur kinerja dan stabilitas API di bawah beban tinggi (load testing). |
| Mempercepat Pengembangan | Mempercepat siklus pengembangan karena tester tidak perlu menunggu User Interface selesai untuk memulai pengujian. |
| Pondasi Integrasi      | Menjadi pondasi penting bagi integrasi antar sistem (mikroservis atau layanan pihak ketiga) yang lancar. |

## III. Anatomi Request dan Response API

Komunikasi API terdiri dari dua bagian utama yang harus diuji:

### A. Anatomi Request (Permintaan)

Request adalah permintaan yang dikirimkan dari klien (misalnya browser atau aplikasi mobile) ke server.

| Elemen         | Fungsi                                      | Contoh                                   |
|----------------|---------------------------------------------|------------------------------------------|
| Method (HTTP Verb) | Menentukan aksi yang ingin dilakukan server. | GET (Mengambil data), POST (Mengirim/Membuat data), PUT (Memperbarui data), DELETE (Menghapus data). |
| URL (Resource Locator) | Alamat spesifik dari resource yang ingin diakses atau dimodifikasi. | `https://api.example.com/users/123`     |
| Headers        | Menyediakan metadata tentang transaksi, seperti tipe data yang diharapkan atau token otentikasi. | `Content-Type: application/json`, `Authorization: Bearer <token>` |
| Body (Payload) | Data yang dikirim ke server (khusus untuk metode POST, PUT, atau PATCH). | Data formulir pendaftaran pengguna baru. |

### B. Anatomi Response (Balasan)

Response adalah balasan yang diberikan oleh server setelah memproses request.

| Elemen         | Fungsi                                      | Contoh                                   |
|----------------|---------------------------------------------|------------------------------------------|
| Status Code    | Kode numerik yang menunjukkan hasil eksekusi. | 200 OK (Sukses), 404 Not Found, 401 Unauthorized, 500 Internal Server Error. |
| Headers        | Menyediakan metadata tentang balasan (misalnya tipe data balasan atau caching). | `Content-Type: application/json`        |
| Body           | Data yang dikembalikan oleh server (misalnya daftar pengguna yang diminta). | Data yang diminta dalam format JSON atau XML. |

## IV. Tools Populer untuk API Testing

| Tool     | Keunggulan Utama                                                                 | Cocok Untuk                                                                 |
|----------|----------------------------------------------------------------------------------|-----------------------------------------------------------------------------|
| POSTMAN  | User-Friendly, mendukung berbagai metode HTTP, manajemen Collection, dan Environment (variabel). Memiliki fitur Testing Otomatis dan Visualisasi Response. | Pengujian manual cepat, pengembangan API, dan functional testing sehari-hari. |
| SOAPUI   | Mendukung API berbasis SOAP (XML) dan REST (JSON). Mampu membuat functional testing, security testing, dan load testing. | Enterprise testing dengan skenario yang kompleks, terutama yang menggunakan protokol SOAP. |