# 📋 TaskTrackerK3 — Sistem Manajemen Tugas Mahasiswa

![Java](https://img.shields.io/badge/Java-ED8B00?logo=openjdk&logoColor=white)
![Swing](https://img.shields.io/badge/GUI-Java%20Swing-blue)
![MySQL](https://img.shields.io/badge/Database-MySQL%2FMariaDB-4479A1?logo=mysql&logoColor=white)
![NetBeans](https://img.shields.io/badge/IDE-Apache%20NetBeans-1B6AC6?logo=apache-netbeans-ide&logoColor=white)

Aplikasi desktop berbasis **Java Swing** untuk membantu mahasiswa mengelola data mahasiswa, mata kuliah, tugas, serta notifikasi pengingat dalam satu sistem yang terintegrasi menggunakan **MySQL**.

> **Proyek Akhir Mata Kuliah Pemrograman I**  
> **Kelompok 3 — Universitas Pamulang**

---

## 📖 Deskripsi

TaskTrackerK3 merupakan aplikasi desktop yang dirancang untuk membantu mahasiswa mengelola tugas perkuliahan secara lebih terstruktur. Sistem ini menyediakan pengelolaan data mahasiswa, mata kuliah, tugas, dan notifikasi sehingga proses pemantauan *deadline* serta status pengerjaan tugas menjadi lebih mudah, cepat, dan efisien.

---

## ✨ Fitur

- CRUD Data Mahasiswa
- CRUD Data Mata Kuliah
- CRUD Data Tugas
- CRUD Data Notifikasi
- Live Search menggunakan `PreparedStatement`
- Cetak laporan dalam format HTML
- Date Picker menggunakan `JDateChooser`
- Primary Key dengan `AUTO_INCREMENT`
- Relasi database menggunakan `Foreign Key`
- Tema antarmuka dengan warna kustom

---

## 🛠️ Teknologi

| Komponen | Teknologi |
|-----------|-----------|
| Bahasa Pemrograman | Java |
| GUI | Java Swing |
| IDE | Apache NetBeans |
| Build Tool | Apache Ant |
| Database | MySQL / MariaDB |
| Database Access | JDBC |
| Library | `mysql-connector-java`, `jcalendar` |

---

## 🗂️ Struktur Proyek

```text
TaskTrackerK3/
│
├── nbproject/
├── src/
│   ├── koneksi/
│   │   └── Koneksi.java
│   ├── mahasiswa/
│   ├── matakuliah/
│   ├── tugas/
│   └── notifikasi/
│
├── data_tugas.html
├── laporan_siswa.html
├── laporan_tugas.html
├── build.xml
├── manifest.mf
├── README.md
└── .gitignore
```

---

## 🗄️ Database

**Nama Database**

```text
db_tasktracker
```

**Tabel**

- `tb_mahasiswa`
- `tb_matakuliah`
- `tb_tugas`
- `tb_notifikasi`

### Relasi Database

```text
tb_mahasiswa
      │
      │
      └──────────────┐
                     │
                     ▼
                tb_tugas
               ▲         ▲
               │         │
               │         │
tb_notifikasi  │   tb_matakuliah
```

---

## ⚙️ Instalasi & Menjalankan

### 1. Clone Repository

```bash
git clone https://github.com/zippynx/Pemrograman-I-Kelompok3.git
```

### 2. Buat Database

Buat database dengan nama:

```text
db_tasktracker
```

Kemudian import file SQL yang tersedia pada repository.

### 3. Konfigurasi Database

Sesuaikan konfigurasi koneksi pada file berikut apabila diperlukan.

```text
src/koneksi/Koneksi.java
```

### 4. Tambahkan Library

Tambahkan library berikut ke project NetBeans:

- `mysql-connector-java`
- `jcalendar`

### 5. Jalankan Aplikasi

Buka project menggunakan **Apache NetBeans**, kemudian jalankan salah satu modul berikut:

- Mahasiswa
- Matakuliah
- Tugas
- LihatTugas
- Notifikasi

---

## 🚀 Pengembangan Selanjutnya

- Menambahkan dashboard sebagai halaman utama.
- Mengintegrasikan seluruh modul ke dalam satu menu utama.
- Menampilkan nama mahasiswa dan mata kuliah menggunakan `JOIN`.
- Memindahkan konfigurasi database ke file konfigurasi eksternal.
- Menggunakan Maven atau Gradle untuk pengelolaan dependency.

---

## 👥 Tim Pengembang

| Nama | NIM |
|------|------|
| M. Aziep Musafira | 241011400336 |
| Mohammad Ariq Arrahman Sudrajat | 241011400352 |
| Raihan Al Amin | 241011401546 |
| Nabilah Putri Ramadhan | 241011400350 |
| Nazla Hana Wahyudi | 241011401657 |

---

## 📄 Lisensi

Proyek ini dikembangkan untuk keperluan pembelajaran sebagai **Proyek Akhir Mata Kuliah Pemrograman I** Universitas Pamulang.