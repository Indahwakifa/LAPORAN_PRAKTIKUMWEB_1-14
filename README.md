# Dokumentasi Praktikum Pemrograman Website

Repositori ini mendokumentasikan serangkaian tugas praktikum **Pemrograman Website** yang berfokus pada pengembangan aplikasi web menggunakan framework **CodeIgniter 4** (Backend) dan **Vue.js** (Frontend).

# IDENTITAS MAHASISWA : 
### Nama : INDAH WAFIKAH

### Nim : 312410559

### Kelas : I241E

### Matkul : Pemrograman Website

# PRAKTIKUM MODUL 1 - 14

## Daftar Modul Praktikum

| Modul | Materi / Topik |
| :--- | :--- |
| **01-03** | Fondasi CI4, Controller, View, Database, & Model |
| **04-06** | Form Handling, CRUD Artikel, & View Layouts |
| **07-09** | Session Auth, Interaktivitas, & AJAX Implementasi |
| **10-12** | REST API CI4, Integrasi Vue.js, State Management |
| **13-14** | Secured SPA, Auth Token, CORS & Middleware |
| **15** | Deployment & Finalisasi Proyek |

## Penjelasan Evolusi Proyek

1. **Fase Fondasi (Modul 1-3):** Mempelajari instalasi lingkungan CI4, konsep *Controller*, *View*, serta konfigurasi *Database* dan *Model*.
2. **Fase CRUD & UX (Modul 4-6):** Implementasi manajemen data artikel dengan sistem *Form Handling* yang valid dan penggunaan *View Layouts* untuk efisiensi tampilan.
3. **Fase Interaktivitas (Modul 7-9):** Transisi dari web tradisional ke web yang responsif menggunakan AJAX agar data dapat diperbarui tanpa perlu melakukan *refresh* halaman secara penuh.
4. **Fase Web API (Modul 10-12):** Mengubah arsitektur menjadi *Decoupled* (terpisah). CI4 difungsikan sebagai penyedia data (*REST API*) dalam format JSON, sementara Vue.js menangani tampilan *Client-side*.
5. **Fase Sekuriti & Finalisasi (Modul 13-15):** Pengamanan aplikasi melalui sistem autentikasi berbasis token dan implementasi *Middleware/Filter* untuk menangani *Cross-Origin Resource Sharing* (CORS) agar komunikasi antara Frontend dan Backend tetap aman.

## Penjelasan Dari Setiap Modul Praktikun 

### Perubahan dari Modul 1 hingga 14 merupakan perjalanan evolusi dari aplikasi web tradisional menjadi aplikasi modern berbasis API. Berikut adalah penjelasan sistematis mengenai setiap fase perubahan tersebut:

### Fase 1: Dasar Pengembangan Web (Modul 1-3)

Modul 01-02 (Fondasi): Mempelajari instalasi lingkungan pengembangan (CodeIgniter 4) dan konsep dasar Controller serta View. Di sini, web masih bersifat statis dan semua logika ditampilkan langsung ke layar.

Modul 03 (Data): Pengenalan Model dan Database. Aplikasi mulai bisa menyimpan dan mengambil data dari MySQL, beralih dari sekadar tampilan statis ke aplikasi berbasis data.

### Fase 2: Interaktivitas & CRUD (Modul 4-6)

Modul 04 (Form): Implementasi Form Handling dan validasi. Aplikasi mulai menangani input pengguna dengan aman.

Modul 05 (CRUD): Implementasi penuh Create, Read, Update, Delete. Ini adalah fase di mana aplikasi memiliki fungsi manajemen data (misal: artikel).

Modul 06 (Layout): Penggunaan sistem View Layouts agar tampilan konsisten (header/footer tidak perlu ditulis berulang).

### Fase 3: User Management & UX (Modul 7-9)

Modul 07 (Auth Web): Implementasi Session untuk Login/Logout. Aplikasi mulai mengenal siapa yang sedang menggunakan sistem.

Modul 08-09 (AJAX): Transisi besar ke arah Asynchronous. Halaman tidak perlu dimuat ulang (refresh) setiap kali ada perubahan data kecil, membuat aplikasi jauh lebih responsif.

### Fase 4: Era Web API (Modul 10-12)

Modul 10 (REST API): CodeIgniter mulai berperan sebagai "penyedia data" (API), bukan lagi pengatur tampilan. Data dikirim dalam format JSON agar bisa dibaca oleh aplikasi lain (seperti Vue.js).

Modul 11 (Vue.js Dasar): Integrasi Frontend menggunakan Vue.js. Aplikasi dipisah menjadi dua: sisi Client (Vue) dan sisi Server (CodeIgniter).

Modul 12 (State & Axios): Memperkenalkan Axios untuk komunikasi data antara Vue.js dan API. State management dimulai untuk menyimpan data sesi secara client-side.

### Fase 5: Keamanan & SPA Lanjutan (Modul 13-14)

Modul 13 (Secured SPA): Implementasi Authentication yang aman untuk Single Page Application. Ini adalah fase yang sedang kamu alami, di mana pertukaran data (Login/Token) harus melewati validasi CORS agar browser mengizinkan komunikasi antar port yang berbeda.

Modul 14 (Middleware/Filter): Penguatan keamanan melalui Filters. Middleware bertindak sebagai satpam yang memeriksa setiap request yang masuk (Auth/CORS) sebelum data sampai ke Controller.

## Arsitektur Komunikasi Data
Aplikasi ini menggunakan komunikasi *asynchronous* antara Frontend dan Backend. Untuk memahami bagaimana browser memproses izin akses antar-port yang berbeda, lihat diagram berikut:

## Teknologi yang Digunakan
* **Backend:** PHP 8.2, CodeIgniter 4
* **Frontend:** Vue.js 3, Axios
* **Database:** MySQL
* **Tools:** XAMPP, VS Code, Postman

## Cara Menjalankan Proyek

### 1. Menjalankan Backend (CI4)
Masuk ke direktori `ci4`, kemudian jalankan server lokal:
```bash
# Gunakan perintah berikut di terminal
php spark serve --port 8080
```

Pastikan terminal backend tetap terbuka selama proses pengembangan.

2. Menjalankan Frontend
Gunakan server lokal untuk file statis di folder frontend. Pastikan konfigurasi Base URL di Axios pada file Login.js mengarah ke http://localhost:8080 untuk memastikan koneksi API berhasil.

Dibuat oleh: Fajar Fawwaz Atallah

Mata Kuliah: Pemrograman Website

## DIBAWAH INI ADALAH DOKUMENTASI SETIAP HALAMAN 

## HALAMAN Lab_Ci11

### Halaman Home 
<img width="960" height="540" alt="Screenshot 2026-06-25 160636" src="https://github.com/user-attachments/assets/7f12a0c5-b00f-40e7-ae7a-d7610172de8f" />


### Halaman Artikel 
<img width="960" height="540" alt="Screenshot 2026-06-25 161010" src="https://github.com/user-attachments/assets/aa77dca2-1eab-4384-9e64-dca52d0f1c9b" />


### Halaman Ajax 
<img width="960" height="540" alt="Screenshot 2026-06-25 161031" src="https://github.com/user-attachments/assets/2cb03924-f2a4-4685-935e-663338d9334b" />

### Halaman Dashboard Admin 
<img width="960" height="540" alt="Screenshot 2026-06-25 161031" src="https://github.com/user-attachments/assets/a190b40c-b28b-4582-9b1d-a6bf6357f63b" />


### Halaman Tambah Artikel 
<img width="960" height="540" alt="image" src="https://github.com/user-attachments/assets/d9cffa92-e8da-49f9-be80-5b4381244abc" />

## Halaman Lab8_VueJs

### Halaman Home / Beranda
<img width="959" height="491" alt="image" src="https://github.com/user-attachments/assets/cb4b9fcb-865e-4b19-b3d4-0630de501a09" />

### Halaman Kelola Artikel 
<img width="959" height="466" alt="image" src="https://github.com/user-attachments/assets/769479c4-c6ea-4e9d-9bb7-f3519f73c7d5" />

### Halanman Tentang Saya 
<img width="955" height="479" alt="image" src="https://github.com/user-attachments/assets/45efd97d-e2a6-4434-bcad-abd96cbbf540" />

### Halaman Post 
<img width="386" height="257" alt="image" src="https://github.com/user-attachments/assets/40496903-bc04-4abc-8b27-361adf494b26" />
