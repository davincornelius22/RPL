# KantinQ

### Sistem Antrean Digital dan Pemesanan Kantin Kampus Berbasis QR Code

## 1. Deskripsi Singkat

**KantinQ** adalah aplikasi berbasis web yang dirancang untuk membantu mahasiswa melakukan pemesanan makanan dan mengurangi antrean fisik di kantin kampus.

Mahasiswa dapat melakukan scan QR Code yang tersedia di kantin untuk melihat menu, membuat pesanan, mendapatkan nomor antrean, dan memantau status pesanan melalui smartphone.

Penjual kantin dapat menerima pesanan, mengatur antrean, memperbarui status pesanan, serta mengelola menu yang tersedia.

---

## 2. Latar Belakang dan Permasalahan

Pada jam istirahat, kantin kampus sering mengalami antrean panjang. Mahasiswa harus berdiri dan menunggu untuk melakukan pemesanan, sehingga waktu istirahat menjadi kurang efektif.

Selain itu, ketika jumlah pembeli meningkat, penjual dapat mengalami kesulitan dalam mencatat dan mengatur pesanan. Mahasiswa juga tidak selalu mengetahui apakah pesanannya masih menunggu, sedang diproses, atau sudah selesai.

Permasalahan utama yang ingin diselesaikan oleh KantinQ adalah:

* Antrean fisik yang panjang.
* Proses pemesanan yang masih dilakukan secara langsung.
* Kesulitan mengetahui status pesanan.
* Kesulitan penjual dalam mengatur banyak pesanan.
* Potensi kesalahan dalam pencatatan pesanan.

KantinQ menyediakan sistem antrean dan pemesanan digital agar proses tersebut menjadi lebih teratur.

---

## 3. Tujuan Aplikasi

Tujuan utama KantinQ adalah:

1. Mengurangi antrean fisik di kantin.
2. Mempermudah mahasiswa dalam melakukan pemesanan.
3. Memberikan nomor antrean secara digital.
4. Memudahkan mahasiswa memantau status pesanan.
5. Membantu penjual mengelola pesanan dengan lebih teratur.

---

## 4. Profil Target Pengguna

### Mahasiswa

Mahasiswa merupakan pengguna utama sebagai pembeli.

Mahasiswa dapat:

* Scan QR Code.
* Melihat menu.
* Memilih makanan dan minuman.
* Membuat pesanan.
* Mendapatkan nomor antrean.
* Melihat status pesanan.
* Mengambil pesanan setelah selesai.

### Penjual Kantin

Penjual menggunakan aplikasi untuk:

* Melihat pesanan masuk.
* Mengelola antrean.
* Mengubah status pesanan.
* Menambah dan mengubah menu.
* Mengubah ketersediaan makanan.

---

## 5. Manfaat Aplikasi

### Bagi Mahasiswa

* Mengurangi waktu menunggu dalam antrean.
* Dapat memesan melalui smartphone.
* Dapat melihat status pesanan.
* Tidak perlu terus berada di depan kasir untuk mengetahui perkembangan pesanan.

### Bagi Penjual

* Mempermudah pengelolaan pesanan.
* Membantu mengatur antrean.
* Mengurangi kesalahan pencatatan.
* Mempermudah pengelolaan menu dan stok.

### Manfaat Utama

**Membuat proses pemesanan dan antrean kantin menjadi lebih cepat, teratur, dan mudah dipantau.**

---

## 6. Fitur Inti

### 1. Scan QR Code

Mahasiswa melakukan scan QR Code yang tersedia di kantin untuk membuka halaman pemesanan.

### 2. Menu Digital

Menampilkan:

* Nama makanan dan minuman.
* Harga.
* Deskripsi sederhana.
* Ketersediaan menu.

### 3. Pemesanan

Mahasiswa dapat:

* Memilih menu.
* Menentukan jumlah pesanan.
* Melihat total pesanan.
* Mengirim pesanan.

### 4. Nomor Antrean Digital

Setelah melakukan pemesanan, sistem memberikan nomor antrean secara otomatis.

Contoh:

`Nomor Pesanan: A-027`

### 5. Status Pesanan

Status pesanan terdiri dari:

`Menunggu → Diproses → Siap Diambil → Selesai`

### 6. Dashboard Penjual

Penjual dapat melihat:

* Pesanan baru.
* Pesanan yang sedang diproses.
* Pesanan yang sudah siap.
* Riwayat pesanan.

### 7. Pengelolaan Menu

Penjual dapat:

* Menambah menu.
* Mengubah menu.
* Menghapus menu.
* Mengubah harga.
* Mengubah ketersediaan menu.

### 8. Informasi Kondisi Antrean

Sistem menampilkan kondisi antrean berdasarkan jumlah pesanan aktif.

Contoh:

* **Sepi**
* **Sedang**
* **Ramai**

---

## 7. Alur Utama Sistem

```text
Mahasiswa
    ↓
Scan QR Code
    ↓
Melihat Menu
    ↓
Memilih Makanan
    ↓
Membuat Pesanan
    ↓
Mendapatkan Nomor Antrean
    ↓
Menunggu
    ↓
Pesanan Diproses
    ↓
Pesanan Siap
    ↓
Mahasiswa Mengambil Pesanan
```

Alur penjual:

```text
Penjual Login
    ↓
Melihat Pesanan Masuk
    ↓
Menerima Pesanan
    ↓
Memproses Pesanan
    ↓
Mengubah Status Menjadi Siap
    ↓
Pesanan Diambil
    ↓
Status Selesai
```

---

## 8. Fitur yang Tidak Dikerjakan

Untuk menjaga ruang lingkup agar realistis diselesaikan dalam 12 pertemuan, fitur berikut tidak dikerjakan pada versi pertama:

* Pembayaran online.
* Integrasi QRIS, GoPay
