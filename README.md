**Aplikasi Web Manajemen Stok Material Toko Bangunan Azwa**

penjelasan : 
Aplikasi ini adalah sistem informasi sederhana (Product Manager) yang dirancang khusus untuk mengelola data material bangunan (seperti semen, cat, pipa, besi, dan kayu) secara digital.

**Fitur yang tersedia :**
1. **Create** : Menambah material baru dengan validasi input ketat (Nama unik, harga `> 0`, stok `≥ 0`).
2. **Read** : Menampilkan katalog material bangunan menggunakan layout grid card responsif.
3. **Update** : Memperbarui informasi material bangunan berdasarkan ID produk.
4. **Delete** : Menghapus material menggunakan metode HTTP **POST** dengan verifikasi **CSRF Token**.


**Cara dan Langkah-langkah menginstalasi (file zip)**

**Langkah-Langkah Instalasi:**

1. **Ekstrak File `.zip` ke Folder `htdocs`**
   
   - Cari file `toko-bangunan.zip` yang telah didownload.
   - Klik kanan pada file `toko-bangunan.zip` lalu pilih **Extract All...** / **Extract Here**.
   - Pastikan folder hasil ekstraksi diletakkan di dalam direktori `htdocs` XAMPP kamu:
     C:\xampp\htdocs\toko-bangunan\
   - *Pastikan struktur foldernya adalah `htdocs/toko-bangunan`

2. **Jalankan Apache & MySQL**

   - Pastikan kamu sudah menginstal aplikasi **XAMPP Control Panel** di device kamu
   - Buka aplikasi **XAMPP Control Panel**.
   - Klik tombol **Start** pada modul **Apache** dan **MySQL** hingga indikator berwarna hijau.

3. **Import Database di phpMyAdmin**
   
   - Buka browser dan akses phpMyAdmin: `http://localhost/phpmyadmin`
   - Pada panel sebelah kiri, buat database baru dengan nama **`db_tokobangunan`**.
   - Klik nama database **`db_tokobangunan`** tersebut, lalu buka tab **Import** di bagian atas.
   - Klik tombol **Choose File** / **Pilih File**, lalu arahkan ke file `schema.sql` yang ada di dalam folder project:
     C:\xampp\htdocs\toko-bangunan\database\schema.sql
   - Gulir ke bawah dan klik tombol **Go** / **Kirim**.

4. **Akses Antarmuka Aplikasi (UI/UX)**
   - Buka tab baru di browser dan buka alamat URL berikut untuk menampilkan antarmuka aplikasi:
     http://localhost/toko-bangunan/tampilan/
