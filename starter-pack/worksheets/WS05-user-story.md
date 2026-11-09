# **WORKBOOK: LEMBAR KERJA MAHASISWA WS05**

## **Formulasi Kebutuhan Fungsional: User Story & Acceptance Criteria**

Mata Kuliah: **Konsep Sistem Informasi (KSI)**  
Kerangka Kerja: **Project-Based Learning (PBL) Level 1**  
Fase Learning Spine: **Fase 3 — Define (Minggu 3)**  
Sub-CPMK / SFIA: **S-01.1 (Intermediate - Problem Framing) & S-03.1 (Intermediate - Pemetaan SI)** | **SFIA BUSA L1, REQM L2**  
Keterkaitan Deliverable: **Bahan Utama Deliverable D2 (System & Solution Design - TPL-02)**

### **1\. Identifikasi Kelompok & Rotasi Kepemimpinan**

- **Nama Kelompok**: Kelompok Tulip / Kelas A
- **Objek UMKM Mitra**: Rizky Laundry
- **Phase Lead 3 (Define)**: Deva Nayla Maisya (2600016039)
- **Anggota Tim**: 
1. M. Zacky Alfattah (2600016015)
  2. M. Faris Ilham (2600016014)
  3. Farizhki (2600016027)
  4. Mutia Fatmawati (2600016049)

### **2\. Landasan Konseptual: Analisis Sistem "What" vs "How"**

Dalam tahap _Systems Analysis_, fokus utama tim adalah menentukan **APA (_What_)** yang dibutuhkan pengguna bisnis untuk memecahkan masalahnya, **BUKAN BAGAIMANA (_How_)** sistem dibangun secara teknis (Marakas & O'Brien, 2013).

- **User Story** merepresentasikan kebutuhan fungsional dari sudut pandang pengguna bisnis dengan pola:  
  $$\text{"Sebagai [Peran Pengguna], Saya ingin [Kemampuan/Fitur], Sehingga [Manfaat Bisnis Nyata]"}$$
- **Acceptance Criteria (Given-When-Then)** mendefinisikan batas kondisi kapan sebuah fitur dinyatakan selesai dan memenuhi syarat penerimaan pengguna (Rainer et al., 2021).

### **3\. Workspace A: Formulasi User Story Fungsional**

Petakan minimal **3 User Story Utama** yang langsung menjawab akar masalah pada D1 / WS04:

#### **User Story 1 (Prioritas Utama / Core Feature)**

- **Sebagai (_As a_)**:
Pemilik Laundry
- **Saya ingin (_I want to_)**:
Saya ingin mencatat transaksi pelanggan dan menghitung secara secara otomatis.
- **Sehingga (_So that_)**:
Sehingga pencatatan transaksi lebih terstruktur dan memudahkan dalam pencarian data.

#### **User Story 2 (Fitur Manajemen Data)**
- **Sebagai (_As a_)**:
Pemilik usaha laundry.
- **Saya ingin (_I want to_)**:
Mencari data transaksi pelanggan untuk memeriksa status pembayaran tanpa melihat buku besar secara manual.
- **Sehingga (_So that_)**:
Sehingga saya dapat melihat status pembayaran pelanggan dengan lebih mudah dan cepat.

#### **User Story 3 (Fitur Informasi)**

- **Sebagai (_As a_)**:
Pemilik Usaha.
- **Saya ingin (_I want to_)**:
Saya ingin melihat rekapitulasi transaksi dalam bentuk spreadsheet
- **Sehingga (_So that_)**:
Tidak perlu menghitung nota fisik dan catatan di buku besar secara manual.

### **4\. Workspace B: Acceptance Criteria Berbasis Skenario (Given-When-Then)**

Susun kriteria penerimaan terstruktur untuk **User Story 1** (mencakup Skenario Sukses dan Skenario Penanganan Eror):

#### **Skenario 1A: Transaksi Berhasil Dicatat (Happy Path)**

- **Diberikan (_Given_)**:  
 Pemilik sedang mencatat transaksi pelanggan
- **Ketika (_When_)**:  
  Pemilik memasukkan data pelanggan (nama, nomor telepon), memilih paket layanan (express, komplit, cuci saja, setrika saja, atau satuan), memasukkan berat/jumlah satuan, serta status pembayaran,  pemilik menekan tombol simpan.
- **Maka (_Then_)**:  
 Kemudian sistem menyimpan transaksi dan menampilkan pesan transaksi berhasil.

#### **Skenario 1B: Penanganan / Eror (Exception Path)**

- **Diberikan (_Given_)**:
Pemilik sedang mencatat transaksi pelanggan.
- **Ketika (_When_)**:
Pemilik menekan tombol simpan tanpa mengisi data pelanggan.
- **Maka (_Then_)**:
Sistem menampilkan bahwa data belum lengkap dan tidak dapat disimpan.

### **5\. Workspace C: Catatan Validasi Kebutuhan dengan Mitra (Field Confirmation)**

- **Tanggal Validasi**: _______________
- **Narahubung Mitra**: Rezza Rahayu (Pemilik)
- **Hasil Konfirmasi User Story**:  
  [ ] Seluruh User Story disetujui mitra  
  [ ] Terdapat penyesuaian/revisi kebutuhan (Tuliskan revisi jika ada):

### **6\. Verifikasi Integritas AI (TPL-07) & Pengesahan**

- **Penggunaan AI Co-pilot**:  
  Apakah tim menggunakan AI untuk membantu merumuskan skenario _Given-When-Then_? [ ] Ya [ ] Tidak  
  _(Jika Ya, wajib melampirkan formulir_ **_TPL-07: AI Usage Disclosure & Verification Note_**_)_.

**Tanda Tangan Tim & Pengesahan Dosen**:

- **Phase Lead 3**: Deva Nayla Maisya (Tanggal: 19/10/2026)
- **Dosen Coach**: (Tanggal: _______________) [ ] Approved
