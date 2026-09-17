# 🍽️ KantinQ

### Sistem Pemesanan dan Antrean Digital Kantin Kampus Berbasis QR Code

> **Pesan tanpa harus berdiri di antrean.**

---

## 📑 Daftar Isi

1. [Tentang KantinQ](#1-tentang-kantinq)
2. [Permasalahan yang Diangkat](#2-permasalahan-yang-diangkat)
3. [Tujuan Pengembangan](#3-tujuan-pengembangan)
4. [Manfaat Sistem](#4-manfaat-sistem)
5. [Fitur Utama](#5-fitur-utama)
6. [Alur Kerja Sistem](#6-alur-kerja-sistem)
7. [Arsitektur Aplikasi](#7-arsitektur-aplikasi)
8. [Teknologi yang Digunakan](#8-teknologi-yang-digunakan)
9. [Struktur Proyek](#9-struktur-proyek)
10. [Batasan Sistem](#10-batasan-sistem)
11. [Cara Menjalankan](#11-cara-menjalankan)
12. [Rencana Pengembangan](#12-rencana-pengembangan)
13. [Kriteria Keberhasilan](#13-kriteria-keberhasilan)
14. [Kontributor](#14-kontributor)

---

# 1. Tentang KantinQ

**KantinQ** merupakan aplikasi web yang dirancang untuk membantu proses pemesanan makanan dan pengelolaan antrean di kantin kampus.

Sistem memanfaatkan **QR Code** sebagai akses utama untuk masuk ke halaman pemesanan. Mahasiswa cukup memindai QR Code yang tersedia pada stan kantin, kemudian memilih makanan atau minuman yang diinginkan.

Setelah pesanan dibuat, sistem akan menghasilkan **nomor antrean digital**. Mahasiswa dapat melihat status pesanan secara langsung melalui halaman web tanpa harus terus berdiri di depan penjual.

Di sisi penjual, tersedia dashboard untuk melihat pesanan yang masuk, mengatur status pesanan, mengelola menu, dan memantau antrean yang sedang berjalan.

Secara umum, KantinQ memiliki alur:

```text
Scan QR
   ↓
Lihat Menu
   ↓
Pilih Pesanan
   ↓
Konfirmasi
   ↓
Nomor Antrean
   ↓
Pesanan Diproses
   ↓
Siap Diambil
   ↓
Selesai
```

---

# 2. Permasalahan yang Diangkat

Pada jam istirahat, jumlah mahasiswa yang datang ke kantin biasanya meningkat dalam waktu yang hampir bersamaan. Kondisi ini dapat menyebabkan antrean panjang dan membuat proses pemesanan menjadi kurang efisien.

Beberapa permasalahan yang menjadi dasar pengembangan KantinQ adalah:

### 2.1 Antrean Fisik

Mahasiswa harus berdiri langsung di depan stan untuk memesan makanan. Ketika jumlah pembeli meningkat, waktu tunggu menjadi lebih lama.

### 2.2 Pemesanan Secara Langsung

Pesanan disampaikan secara verbal kepada penjual. Dalam kondisi ramai, cara ini dapat menyebabkan kesalahan pencatatan atau pesanan tertukar.

### 2.3 Tidak Ada Informasi Status Pesanan

Setelah memesan, mahasiswa biasanya hanya menunggu atau bertanya kembali kepada penjual untuk mengetahui apakah makanannya sudah selesai.

### 2.4 Pengelolaan Antrean Kurang Terstruktur

Penjual harus mengingat dan mengatur banyak pesanan sekaligus, terutama ketika jumlah pembeli meningkat.

### 2.5 Tidak Ada Informasi Kondisi Antrean

Mahasiswa tidak mengetahui kondisi antrean sebelum memesan, sehingga sulit memperkirakan waktu tunggu.

### 💡 Pendekatan Solusi

KantinQ mengubah proses tersebut menjadi alur digital:

```mermaid
flowchart TD
    A[Mahasiswa] --> B[Scan QR Code]
    B --> C[Menu Digital]
    C --> D[Pilih Makanan]
    D --> E[Buat Pesanan]
    E --> F[Nomor Antrean]
    F --> G[Dashboard Penjual]
    G --> H[Pesanan Diproses]
    H --> I[Siap Diambil]
    I --> J[Pesanan Selesai]
```

---

# 3. Tujuan Pengembangan

KantinQ dikembangkan dengan beberapa tujuan utama:

* Mengurangi ketergantungan pada antrean fisik saat melakukan pemesanan.
* Membuat proses pemesanan lebih cepat dan terstruktur.
* Memberikan nomor antrean secara otomatis.
* Memberikan informasi status pesanan kepada mahasiswa.
* Membantu penjual mengelola antrean dan pesanan melalui satu dashboard.
* Menyediakan sistem yang sederhana dan mudah digunakan melalui smartphone.

---

# 4. Manfaat Sistem

## 👨‍🎓 Bagi Mahasiswa

* Tidak perlu berdiri dalam antrean hanya untuk melakukan pemesanan.
* Dapat melihat menu dan harga melalui smartphone.
* Mendapatkan nomor antrean secara otomatis.
* Dapat memantau perkembangan pesanan.
* Mengetahui kapan pesanan sudah dapat diambil.

## 👨‍🍳 Bagi Penjual

* Pesanan masuk dalam sistem secara terstruktur.
* Lebih mudah melihat urutan antrean.
* Status pesanan dapat diperbarui dengan mudah.
* Data menu dapat dikelola melalui dashboard.
* Mengurangi kemungkinan kesalahan pencatatan.

## 🎯 Manfaat Utama

> **KantinQ membantu membuat proses pemesanan dan antrean makanan di lingkungan kampus menjadi lebih terorganisir dan mudah dipantau.**

---

# 5. Fitur Utama

| Fitur                | Deskripsi                                                     |
| -------------------- | ------------------------------------------------------------- |
| 📱 QR Ordering       | QR Code menjadi pintu masuk ke halaman pemesanan              |
| 🍔 Menu Digital      | Menampilkan daftar makanan, minuman, harga, dan ketersediaan  |
| 🛒 Keranjang Pesanan | Pengguna dapat memilih item dan menentukan jumlah             |
| 🔢 Nomor Antrean     | Sistem membuat nomor antrean secara otomatis                  |
| 🔄 Status Pesanan    | Pesanan berpindah dari menunggu hingga selesai                |
| 📋 Dashboard Penjual | Menampilkan seluruh pesanan aktif                             |
| 🍜 Manajemen Menu    | Menambah, mengubah, menghapus, dan mengatur ketersediaan menu |
| 📢 Kondisi Antrean   | Menampilkan kondisi antrean berdasarkan jumlah pesanan aktif  |
| 📜 Riwayat Pesanan   | Menyimpan daftar pesanan yang telah selesai atau dibatalkan   |
| 🧾 Detail Pesanan    | Menampilkan item, jumlah, harga, total, dan nomor antrean     |

### Status Pesanan

```text
WAITING
   ↓
PROCESSING
   ↓
READY
   ↓
COMPLETED
```

Pesanan juga dapat berakhir dengan status:

```text
CANCELLED
```

---

# 6. Alur Kerja Sistem

## 6.1 Alur Mahasiswa

```mermaid
flowchart LR
    A[Scan QR] --> B[Buka Halaman Kantin]
    B --> C[Lihat Menu]
    C --> D[Pilih Menu]
    D --> E[Konfirmasi Pesanan]
    E --> F[Sistem Membuat Nomor Antrean]
    F --> G[Lihat Status Pesanan]
    G --> H[Ambil Pesanan]
```

## 6.2 Alur Penjual

```mermaid
flowchart LR
    A[Dashboard] --> B[Pesanan Masuk]
    B --> C[Proses Pesanan]
    C --> D[Ubah Status]
    D --> E[Pesanan Siap]
    E --> F[Pesanan Diambil]
    F --> G[Selesai]
```

## 6.3 Kondisi Antrean

Sistem memberikan indikator sederhana berdasarkan jumlah pesanan aktif:

```text
0 - 5 pesanan       → 🟢 Sepi
6 - 15 pesanan      → 🟡 Sedang
16+ pesanan         → 🔴 Ramai
```

Nilai tersebut dapat disesuaikan selama tahap pengujian berdasarkan kondisi penggunaan aplikasi.

---

# 7. Arsitektur Aplikasi

KantinQ menggunakan arsitektur sederhana yang memisahkan antarmuka pengguna, backend, dan database.

```mermaid
flowchart TB
    A[Mahasiswa / Smartphone]
    B[Penjual / Browser]

    A --> C[React Web Application]
    B --> C

    C --> D[REST API]
    D --> E[Express Backend]
    E --> F[Prisma ORM]
    F --> G[(MySQL)]
```

### Alur Data Pemesanan

```mermaid
flowchart TD
    A[User Scan QR] --> B[Frontend]
    B --> C[POST Order]
    C --> D[Backend]
    D --> E[Validasi Pesanan]
    E --> F[Generate Queue]()
```
