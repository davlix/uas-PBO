# 📌 Pembayaran SPP

## 📖 Deskripsi
Aplikasi **Pembayaran SPP** adalah sistem berbasis Java yang menggunakan database untuk mengelola pembayaran SPP siswa. Aplikasi ini memiliki fitur utama seperti:
- Login Admin
- Manajemen Data Siswa
- Input dan Pembayaran SPP
- Riwayat Pembayaran
- Pencarian Data

## 🛠️ Teknologi yang Digunakan
- **Java (Swing & AWT)** - Untuk tampilan antarmuka pengguna (GUI)
- **MySQL Database** - Untuk menyimpan data
- **JDBC** - Untuk koneksi antara Java dan MySQL
- **NetBeans/IntelliJ IDEA** - IDE yang direkomendasikan

---

## 🚀 Instalasi & Konfigurasi

### 1️⃣ **Clone atau Download Repository**
```sh
 git clone https://github.com/davlix/uas-PBO.git
```

### 2️⃣ **Import ke IDE**
1. Buka **NetBeans** atau **IntelliJ IDEA**
2. Pilih **Open Project** dan arahkan ke folder proyek
3. Pastikan semua dependensi sudah terinstal

### 3️⃣ **Konfigurasi Database**
1. Buka MySQL dan buat database baru:
   ```sql
   CREATE DATABASE pembayaran_spp;
   ```
2. Import file `dbprojectsiswa.sql` ke dalam MySQL
3. Pastikan konfigurasi koneksi database di **Koneksi.java** sudah sesuai:
   ```java
   String url = "jdbc:mysql://localhost:3306/pembayaran_spp";
   String user = "root";
   String pass = "";
   ```

---

## 🎯 Fitur

### ✅ **1. Login Admin**
- Admin dapat login menggunakan **username dan password**
- Validasi input dan autentikasi
- user : admin
- pass : admin123

### ✅ **2. Manajemen Data Siswa**
- Tambah, edit, hapus, dan lihat daftar siswa
- Pencarian data siswa

### ✅ **3. Pembayaran SPP**
- Input transaksi pembayaran siswa
- Update status pembayaran
- Cetak struk pembayaran

### ✅ **4. Riwayat Pembayaran**
- Menampilkan daftar pembayaran yang sudah dilakukan
- Filter berdasarkan bulan/tahun

### ✅ **5. Pencarian Data**
- Fitur pencarian untuk siswa dan pembayaran

---

## 🔧 Struktur Proyek
```
PembayaranSPP/
│── src/
│   ├── LoginAdmin.java    # Form login admin
│   ├── PembayaranSPP.java # Main class
│   ├── Koneksi.java       # Koneksi database
│── database.sql          # Skrip database
│── README.md             # Dokumentasi
```

---

## 📌 Cara Menjalankan Aplikasi
1. Jalankan **MySQL** dan pastikan database sudah dikonfigurasi
2. Buka proyek di **IDE** dan jalankan `PembayaranSPP.java`
3. Masukkan **username dan password admin** untuk login
4. Gunakan fitur yang tersedia sesuai kebutuhan

---

## 🛠️ Perbaikan Bug & Update
### 🔹 **Bug yang Diperbaiki:**
- **(FIXED)** NullPointerException pada koneksi database
- **(FIXED)** Error saat menampilkan data siswa

### 🆕 **Fitur yang Ditambahkan:**
- **Login Admin** sebagai main login
- **Manajemen Siswa & Pembayaran**
- **Validasi Input & Keamanan Data**

---
