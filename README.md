# Aplikasi CRUD Mahasiswa dengan Login - Flutter + SQLite

Aplikasi Flutter ini merupakan aplikasi **CRUD (Create, Read, Update, Delete)** sederhana untuk mengelola data mahasiswa, dengan sistem **login admin** dan penyimpanan data menggunakan **SQLite lokal**.

##  Fitur Aplikasi

- **Login Admin**
  - Akses aplikasi hanya oleh admin dengan username dan password yang telah ditentukan.
  - Username default: `admin`
  - Password default: `password`

- **Manajemen Data Mahasiswa**
  - Tambah data mahasiswa baru.
  - Lihat daftar seluruh mahasiswa.
  - Edit data mahasiswa.
  - Hapus data mahasiswa.

- **Logout**
  - Keluar dari halaman utama kembali ke halaman login.

## Screenshot
# Halaman Awal
![1st sqlite](https://github.com/user-attachments/assets/ab5b47f4-f25c-4a3d-b331-cd155d399350)

# Halaman Isi
![2nd form](https://github.com/user-attachments/assets/42c8780f-caf0-43d3-89e3-47e03df5fbc5)
![3rd form](https://github.com/user-attachments/assets/12884090-ad97-41e4-92e4-6b1bb6e8e5f7)
![4th form](https://github.com/user-attachments/assets/e2552acc-f01c-4082-93cf-6b77ee0986d6)

##  Alur Program

1. **LoginPage**
   - Halaman awal untuk login.
   - Hanya admin yang dapat mengakses aplikasi.
   
2. **MainPage**
   - Menampilkan daftar mahasiswa dari database lokal.
   - Terdapat tombol:
     -  Tambah mahasiswa baru
     -  Edit data mahasiswa
     -  Hapus mahasiswa
     -  Logout kembali ke LoginPage

3. **StudentFormPage**
   - Form input untuk menambah atau mengedit data mahasiswa.

4. **DatabaseHelper**
   - Singleton class untuk mengelola database SQLite:
     - Membuat tabel jika belum ada.
     - Menyimpan data mahasiswa.
     - Mengambil data mahasiswa.
     - Memperbarui data mahasiswa.
     - Menghapus data mahasiswa.
