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
* Integrasi QRIS, GoPay, DANA, atau OVO.
* Pengantaran makanan.
* Integrasi WhatsApp atau SMS.
* Notifikasi push kompleks.
* Aplikasi Android/iOS khusus.
* GPS atau pelacakan lokasi.
* Sistem rekomendasi makanan berbasis AI.
* Sistem loyalty atau poin pelanggan.
* Integrasi dengan sistem akademik kampus.
* Sistem multi-kampus.
* Reservasi meja.
* Analisis penjualan yang kompleks.

Pembayaran dilakukan secara langsung di kasir pada versi pertama.

---

## 9. Kriteria Aplikasi Dinyatakan Berhasil

Aplikasi dinyatakan berhasil apabila:

* Mahasiswa dapat membuka sistem melalui QR Code.
* Mahasiswa dapat melihat menu dan harga.
* Mahasiswa dapat membuat pesanan.
* Sistem dapat memberikan nomor antrean secara otomatis.
* Data pesanan tersimpan dengan benar.
* Penjual dapat melihat pesanan masuk.
* Penjual dapat mengubah status pesanan.
* Mahasiswa dapat melihat status pesanannya.
* Penjual dapat mengelola menu.
* Sistem dapat menampilkan kondisi antrean.
* Data tetap tersimpan setelah halaman diperbarui.
* Seluruh fitur utama dapat berjalan tanpa error pada penggunaan normal.
* Aplikasi dapat digunakan melalui browser desktop maupun smartphone.

---

## 10. Ruang Lingkup Pengembangan

Pengembangan KantinQ difokuskan pada:

**QR Code → Pemesanan → Nomor Antrean → Pengelolaan Pesanan → Status Pesanan**

Sistem tidak berfokus pada pembayaran digital atau layanan pengantaran makanan.

---

## 11. Target Pengembangan 12 Pertemuan

| Pertemuan | Fokus                                          |
| --------- | ---------------------------------------------- |
| 1         | Analisis masalah dan kebutuhan sistem          |
| 2         | Perancangan use case dan alur sistem           |
| 3         | Perancangan database dan ERD                   |
| 4         | Perancangan UI/UX                              |
| 5         | Setup project dan database                     |
| 6         | Fitur menu dan data kantin                     |
| 7         | Fitur pemesanan                                |
| 8         | Sistem nomor antrean                           |
| 9         | Dashboard penjual                              |
| 10        | Status dan pengelolaan pesanan                 |
| 11        | Integrasi QR Code dan testing                  |
| 12        | Perbaikan, pengujian akhir, dan persiapan demo |

---

## 12. Kesimpulan

KantinQ merupakan sistem pemesanan dan antrean digital yang ditujukan untuk membantu mahasiswa dan penjual kantin dalam mengatasi permasalahan antrean fisik dan pengelolaan pesanan.

Dengan memanfaatkan QR Code, mahasiswa dapat mengakses menu dan melakukan pemesanan dengan lebih praktis, sementara penjual dapat mengelola antrean dan status pesanan melalui dashboard.
