# Modul Praktikum OOP Python & Studi Kasus MyEdotel

Dokumentasi ini berisi materi pembelajaran **Object-Oriented Programming (OOP)** menggunakan bahasa pemrograman Python, dari konsep dasar hingga implementasi nyata berupa proyek sistem manajemen pemesanan hotel **MyEdotel**.

---

## 📌 Daftar Isi
1. [Tentang Proyek](#-tentang-proyek)
2. [Materi Pembelajaran & Latihan](#-materi-pembelajaran--latihan)
3. [Studi Kasus Utama: MyEdotel](#-studi-kasus-utama-myedotel)
4. [Prasyarat & Cara Menjalankan](#-prasyarat--cara-menjalankan)
5. [Struktur File Notebook](#-struktur-file-notebook)

---

## 📖 Tentang Proyek

Proyek ini dirancang sebagai panduan hands-on untuk mempelajari 4 Pilar Utama Object-Oriented Programming (OOP):
* **Encapsulation** (Enkapsulasi & Proteksi Data)
* **Inheritance** (Pewarisan Karakteristik & Method)
* **Abstraction** (Abstraksi & Kontrak Interface)
* **Polymorphism** (Polimorfisme & Dynamic Method Overriding)

Setiap materi dilengkapi dengan latihan praktis, tugas analisis interaktif, serta diakhiri dengan studi kasus pembuatan aplikasi simulasi pemesanan kamar hotel (MyEdotel).

---

## 📚 Materi Pembelajaran & Latihan

### 1. Dasar Class & Object
* **Konsep**: Membuat cetak biru (*class*), atribut, *method*, dan instansiasi *object*.
* **Contoh**: Implementation `Class Kucing` dan `Class Hero` (Latihan 1 & 2).

### 2. Pewarisan (Inheritance) & Interaction
* **Konsep**: Menurunkan atribut dan method dari *Parent Class* ke *Child Class* serta interaksi antar-objek.
* **Contoh**: `Burung` mewarisi `Hewan`, class `Mage` mewarisi `Hero` dengan penambahan *attribute* `mana` dan *method* `skill_fireball()`.

### 3. Enkapsulasi (Encapsulation)
* **Konsep**: Proteksi data internal dengan atribut privat (`__atribut`), penggunaan *Getter* dan *Setter*, serta validasi data.
* **Analisis**: Pemahaman *Name Mangling* (`_NamaClass__namaAtribut`) dan pentingnya *Setter* untuk menjaga integritas data.

### 4. Abstraksi (Abstraction & Interface)
* **Konsep**: Penggunaan modul `abc` (`ABC`, `@abstractmethod`) untuk membuat kontrak mentah yang wajib diimplementasikan oleh *Child Class*.
* **Contoh**: Class abstrak `GameUnit` yang diturunkan ke `Hero` dan `Monster`.

### 5. Polimorfisme (Polymorphism)
* **Konsep**: Kemampuan *method* bertindak berbeda sesuai dengan kelas turunan yang memanggilnya.
* **Contoh**: Iterasi array `pasukan` yang berisi `Mage`, `Archer`, `Fighter`, dan `Healer`, di mana masing-masing mengeksekusi method `serang()` khas kelasnya.

---

## 🏨 Studi Kasus Utama: MyEdotel

**MyEdotel** merupakan sistem manajemen kamar hotel sederhana berbasis Python. Sistem ini dirancang untuk mengelola data jenis kamar, stok, harga dasar, serta perhitungan otomatis transaksi pemesanan berbasis OOP.

### Fitur Utama MyEdotel:
* **Abstract Base Class (`KamarHotel`)**: Menjadi fondasi untuk semua tipe kamar dengan proteksi stok dan harga dasar (*Encapsulation*).
* **Varian Kamar (`KamarDeluxe` & `KamarStandard`)**: Mengimplementasikan perbedaan besaran pajak (10% untuk Deluxe, 5% untuk Standard) dan informasi fasilitas/kapasitas (*Inheritance & Polymorphism*).
* **Validasi Stok**: Mencegah penginputan stok negatif saat pembaruan data oleh admin.
* **Pemroses Transaksi (`proses_transaksi`)**: Menghitung *subtotal* per unit kamar sesuai durasi menginap (malam) serta total tagihan *struk pemesanan*.

---

## 🚀 Prasyarat & Cara Menjalankan

### Prasyarat System
* **Python 3.x**
* **Jupyter Notebook** / **VS Code** / **Google Colab**

### Cara Menjalankan

#### Menggunakan Google Colab (Rekomendasi):
Klik badge di bawah untuk membuka notebook secara langsung melalui Google Colab:

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/adityarahman09-max/Modul-KKA-Pak-Arifin/blob/main/Modul1_KKA.ipynb)

#### Menggunakan Lokal (Jupyter Notebook / VS Code):
1. Clone repositori ini:
   ```bash
   git clone https://github.com/adityarahman09-max/Modul-KKA-Pak-Arifin.git
   cd Modul-KKA-Pak-Arifin
   ```
2. Buka berkas `Modul1_KKA.ipynb` di Jupyter Notebook atau VS Code.
3. Jalankan sel kode (*Cell*) secara berurutan dari atas ke bawah (`Shift + Enter`).

---

## 📄 Struktur File Notebook

| Kode / Sel | Topik Latihan | Deskripsi Singkat |
| :--- | :--- | :--- |
| **Latihan 1** | Class & Attribute | Pembuatan `Hero` awal & uji coba perubahan atribut langsung |
| **Latihan 2** | Interaksi Objek | Method `serang(lawan)` antar-objek |
| **Latihan 3** | Inheritance | Class `Mage(Hero)` & penggunaan `super().__init__()` |
| **Latihan 4** | Encapsulation | Private attribute `__hp`, *getter*, dan *setter* |
| **Latihan 5** | Abstraction | Abstract class `GameUnit` & `@abstractmethod` |
| **Latihan 6** | Polymorphism | Array/List `pasukan` dengan overriding method |
| **Project** | **MyEdotel** | Sistem pemesanan kamar hotel berorientasi objek lengkap |

---
*Dibuat untuk keperluan materi pembelajaran Modul KKA.*