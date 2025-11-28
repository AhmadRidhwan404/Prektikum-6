# Program Daftar Nilai Mahasiswa

Program sederhana untuk mengelola data nilai mahasiswa menggunakan Python dengan implementasi fungsi-fungsi dasar.

## Deskripsi

Program ini memungkinkan pengguna untuk melakukan operasi CRUD (Create, Read, Update, Delete) pada data nilai mahasiswa. Data disimpan dalam dictionary Python dengan nama mahasiswa sebagai key dan nilai sebagai value.

## Fitur

- **Tambah Data**: Menambahkan data mahasiswa baru beserta nilainya
- **Tampilkan Data**: Menampilkan seluruh daftar mahasiswa dan nilai mereka
- **Hapus Data**: Menghapus data mahasiswa berdasarkan nama
- **Ubah Data**: Mengubah nilai mahasiswa yang sudah ada
- **Keluar**: Keluar dari program

## Cara Menggunakan

1. Jalankan program dengan perintah:
   ```bash
   python nama_file.py
   ```

2. Pilih menu yang tersedia dengan memasukkan angka 1-5:
   - **1**: Untuk menambah data mahasiswa baru
   - **2**: Untuk menampilkan semua data mahasiswa
   - **3**: Untuk menghapus data mahasiswa
   - **4**: Untuk mengubah nilai mahasiswa
   - **5**: Untuk keluar dari program

3. Ikuti instruksi yang muncul di layar

**##FLOWCHART**

```
+----------------+
|     MULAI      |
+----------------+
        |
        v
+----------------------+
|   Tampilkan Menu     |
| 1.Tambah 2.Tampil    |
| 3.Hapus  4.Ubah      |
| 5.Keluar             |
+----------------------+
        |
        v
+----------------------+
|   Input Pilihan      |
+----------------------+
        |
        v
      / |  \  \   \
     /  |   \  \   \
    v   v    v  v   v

(1) Tambah Data?
        |
        v
+----------------------------+
| Input Nama & Nilai         |
| Simpan ke Dictionary       |
+----------------------------+
        |
        v
      (Kembali ke Menu)

(2) Tampilkan Data?
        |
        v
+----------------------------+
| Cek: Data kosong?          |
| Ya -> Tampilkan pesan      |
| Tidak -> Tampilkan semua   |
+----------------------------+
        |
        v
      (Kembali ke Menu)

(3) Hapus Data?
        |
        v
+-------------------------------+
| Input nama yang dihapus       |
| Cek: nama ada?                |
| Ya -> Hapus                   |
| Tidak -> Tampilkan pesan      |
+-------------------------------+
        |
        v
      (Kembali ke Menu)

(4) Ubah Data?
        |
        v
+-------------------------------+
| Input nama yg diubah          |
| Cek: nama ada?                |
| Ya -> Input nilai baru        |
| Tidak -> Tampilkan pesan      |
+-------------------------------+
        |
        v
      (Kembali ke Menu)

(5) Keluar?
        |
        v
+----------------+
|     SELESAI    |
+----------------+


## Contoh Penggunaan

```
Menu:
1. Tambah data mahasiswa
2. Tampilkan data mahasiswa
3. Hapus data mahasiswa
4. Ubah data mahasiswa
5. Keluar
Pilih menu (1-5): 1
Masukkan nama mahasiswa: Budi
Masukkan nilai mahasiswa: 85
Data Budi dengan nilai 85.0 berhasil ditambahkan.

Menu:
1. Tambah data mahasiswa
2. Tampilkan data mahasiswa
3. Hapus data mahasiswa
4. Ubah data mahasiswa
5. Keluar
Pilih menu (1-5): 2
Daftar Nilai Mahasiswa:
- Budi: 85.0
```

## Struktur Program

- `mahasiswa = {}`: Dictionary untuk menyimpan data mahasiswa
- `tambah()`: Fungsi untuk menambah data mahasiswa
- `tampilkan()`: Fungsi untuk menampilkan semua data
- `hapus(nama)`: Fungsi untuk menghapus data berdasarkan nama
- `ubah(nama)`: Fungsi untuk mengubah nilai mahasiswa
- Menu utama dengan loop `while True` untuk interaksi pengguna

## Validasi Input

Program memiliki validasi untuk:
- Memastikan nilai yang diinput adalah angka (float)
- Menangani error dengan `try-except` untuk input nilai
- Mengecek keberadaan nama mahasiswa sebelum menghapus atau mengubah data

## Reminder 

- Data mahasiswa hanya tersimpan selama program berjalan (tidak persisten)
- Setelah program ditutup, semua data akan hilang
- Untuk penyimpanan permanen, pertimbangkan menggunakan file atau database
