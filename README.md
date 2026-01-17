# Project-UAS-SMT-1

Program Data Mahasiswa
Program sederhana untuk mengelola data nilai mahasiswa menggunakan Python. Program ini dibuat dengan konsep modular dan mengimplementasikan operasi CRUD (Create, Read, Update, Delete).
Fitur Program
Program ini punya beberapa fitur utama:

Create (C) - Menambah data mahasiswa baru
Read (R) - Melihat semua data mahasiswa
Update (U) - Mengubah data mahasiswa yang sudah ada
Delete (D) - Menghapus data mahasiswa
Search (S) - Mencari data mahasiswa tertentu
Quit (Q) - Keluar dari program

Cara Kerja
1. Menambah Data (Create)
Ketika memilih menu Create, program akan meminta input:

Nama mahasiswa
NIM
Nilai Tugas
Nilai UTS
Nilai UAS

Nilai akhir dihitung otomatis dengan rumus:
Nilai Akhir = (Tugas × 30%) + (UTS × 35%) + (UAS × 35%)
Setelah input satu data, ada opsi untuk menambah data lagi atau tidak.
2. Melihat Data (Read)
Menampilkan semua data mahasiswa dalam bentuk tabel yang rapi. Kalau belum ada data sama sekali, akan muncul pesan "Tidak Ada Data".
3. Mengubah Data (Update)
Program akan minta nama mahasiswa yang mau diubah. Kalau nama ditemukan, bisa input semua data baru (NIM dan nilai-nilai). Kalau nama tidak ditemukan, akan muncul pesan error.
4. Menghapus Data (Delete)
Cukup masukkan nama mahasiswa yang mau dihapus. Data akan langsung terhapus dari sistem kalau nama ditemukan.
5. Mencari Data (Search)
Bisa cari data mahasiswa spesifik berdasarkan nama. Hasilnya akan ditampilkan dalam bentuk tabel.
Struktur Program
Program ini dibagi jadi beberapa bagian:

model/daftar_nilai.py - Berisi fungsi-fungsi utama (tambah, ubah, hapus, cari data)
view/input_nilai.py - Mengatur proses input data
view/view_nilai.py - Mengatur tampilan data

Semua data disimpan dalam dictionary data_mahasiswa dengan struktur:
python{
    'nama': (nim, tugas, uts, uas, nilai_akhir)
}
Cara Menjalankan

Pastikan Python sudah terinstall di komputer
Clone repository ini
Jalankan file utama program
Pilih menu sesuai kebutuhan dengan mengetik huruf yang sesuai (c/r/u/d/s/q)

Catatan

Program menggunakan nama mahasiswa sebagai key, jadi pastikan tidak ada nama yang sama
Input NIM dan nilai harus berupa angka
Data hanya tersimpan selama program berjalan (tidak permanen)
Validasi input masih minimal, jadi pastikan input sesuai format yang diminta
