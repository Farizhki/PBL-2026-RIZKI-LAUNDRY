# **WORKBOOK: LEMBAR KERJA MAHASISWA (WS07)**

## **Simple Solution Design — IPO, Flowchart & Pseudocode**

### **INFORMASI UTAMA**

- **Mata Kuliah**: Konsep Sistem Informasi (KSI)
- **Kerangka Kerja**: Project-Based Learning (PBL) Level 1
- **Learning Moment**: _Fase 4: Design (Minggu 5–6)_
- **Sub-CPMK / SFIA**: S-03.1 (Intermediate) | SFIA ARCH L2, DESN L2
- **Keterkaitan Deliverable**: Sumber utama pembuatan **Deliverable D2 (System & Solution Design - TPL-02)**
- **Phase Lead**: **Mahasiswa D** (_Phase Lead 4 — Design_)

### **RUANG KERJA TIM (WORKSPACE)**

#### **1\. IDENTIFIKASI KELOMPOK & SOLUSI**

- **Nama Tim**: Kelompok Tulip / Kelas A
- **Nama UMKM Mitra**: Rizky Laundry
- **Judul Solusi SI**: Sistem Pencatatan dan Pencarian Transaksi Rizky Laundry
- **Phase Lead 4 (Design)**: Farizhki (2600016027)

#### **2\. PEMETAAN ARSITEKTUR 4 LAPISAN SI (M05)**

Petakan solusi Anda ke dalam 4 lapisan arsitektur terintegrasi:

| **Lapisan Arsitektur**                           | **Komponen Solusi Tim**                                             | **Keterangan & Batasan**                                           |
| ------------------------------------------------ | ------------------------------------------------------------------- | ------------------------------------------------------------------ |
| **1\. Process Layer** _(Alur Kerja To-Be)_       | \_**\_**\_**\_**\_**\_**\_**\_**\_**\_**\_**\_**\_**\_**\_**\_**\__ | Alur transaksi kasir To-Be yang lebih efisien dibanding _As-Is_.   |                           |
| **2\. Data Layer** _(Struktur Data Logis)_       | \_**\_**\_**\_**\_**\_**\_**\_**\_**\_**\_**\_**\_**\_**\_**\_**\__ | Entitas data: Tabel Menu/Produk, Tabel Transaksi, & Tabel Stok.    |                           |
| **3\. Application Layer** _(Modul Program)_      | \_**\_**\_**\_**\_**\_**\_**\_**\_**\_**\_**\_**\_**\_**\_**\_**\__ | Modul Utama: Login, Input Transaksi, Hitung Total/Diskon, & Rekap. |                           |
| **4\. Infrastructure Layer** _(Perangkat Fisik)_ | \_**\_**\_**\_**\_**\_**\_**\_**\_**\_**\_**\_**\_**\_**\_**\_**\__ | Hardware: Laptop/Tablet POS; Net: Wi-Fi/4G; OS: Windows/Android.   |
                           |

#### **3\. SPESIFIKASI IPO (INPUT - PROCESSING - OUTPUT - STORAGE - CONTROL)**

##### **Fitur Fungsional Utama 1: Pencatatan Transaksi Pesanan & Kalkulasi Biaya Otomatis**

- **Input**: Nama pelanggan, nomor telepon, jenis paket layanan (express, komplit, cuci saja, setrika saja, atau satuan sprei/selimut), berat pakaian (kg) atau jumlah satuan (pcs), dan status pembayaran (lunas, belum lunas, atau DP).
- **Processing**: Memvalidasi data input, mengalikan berat atau jumlah satuan dengan tarif paket yang dipilih, menghitung total harga tagihan secara otomatis, dan mencatat waktu transaksi.
- **Output**: Tampilan rincian tagihan transaksi pesanan di layar dan pesan konfirmasi bahwa data transaksi berhasil disimpan.
- **Storage**: Berkas data transaksi terstruktur (lembar data spreadsheet).
- **Control (Error Handling)**: Validasi data wajib (nama tidak boleh kosong, berat/jumlah harus berupa angka > 0); jika input tidak valid sistem akan menampilkan input tidak valid, Transaksi tidak dapat disimpan.
##### **Fitur Fungsional Utama 2: Pencarian Data Transaksi & Pembaruan Status Pembayaran**

- **Input**: Kata kunci pencarian (Nama pelanggan atau Nomor telepon).
- **Processing**: Menelusuri berkas data transaksi berdasarkan nama atau nomor telepon yang cocok, menampilkan informasi transaksi yang ditemukan, dan memperbarui kolom status pembayaran.
- **Output**: Tampilan rincian transaksi pesanan pelanggan (nama, tanggal, paket, berat, total harga, status pembayaran) dan pesan konfirmasi pembaruan status berhasil.
- **Storage**: Memperbarui status pembayaran pada baris data transaksi terkait di berkas data (lembar spreadsheet).
- **Control (Error Handling)**: Jika nama atau nomor telepon tidak ditemukan di data, sistem menampilkan pesan bahwa data tidak ditemukan tanpa menyebabkan program terhenti (crash).

#### **4\. DIAGRAM ALIR (FLOWCHART) LOGIKA PROGRAM**

_Petunjuk: Gambarkan diagram alir terstruktur menggunakan simbol standar (Persegi Panjang = Proses, Belah Ketupat = Keputusan IF-ELSE, Jajar Genjang = Input/Output, Oval = Start/End). Lampirkan hasil gambaran digital/foto kertas A3 di bawah ini._

[ TEMPELKAN GAMBAR DIAGRAM FLOWCHART DIGITAL / FOTO DRAF A3 DI SINI ]



#### **5\. PSEUDOCODE TERSTRUKTUR (INDEPENDEN TEKNOLOGI)**

Tuliskan kode semu terstruktur (_pseudocode_) untuk modul logika utama solusi Anda:

ALGORITMA Transaksi_Kasir_Teguk

```
KAMUS DATA:
   kode_produk, nama_produk : STRING
   harga, jumlah, subtotal, total_bayar, uang_tunai, kembalian : REAL
   stok_tersedia : INTEGER
ALUR LOGIKA:
   START
   READ kode_produk, jumlah
```

```
   IF stok_tersedia >= jumlah THEN
      subtotal = harga * jumlah
      total_bayar = subtotal
      PRINT total_bayar
```

```
      READ uang_tunai
      IF uang_tunai >= total_bayar THEN
         kembalian = uang_tunai - total_bayar
         stok_tersedia = stok_tersedia - jumlah
         PRINT "Transaksi Sukses", kembalian
         UPDATE Tabel_Stok, Tabel_Transaksi
      ELSE
         PRINT "ERROR: Uang tunai kurang!"
      ENDIF
   ELSE
      PRINT "ERROR: Stok tidak mencukupi!"
   ENDIF
   END
```



### **CHECKLIST REFLEKSI & PENGESAHAN WS07**

- Arsitektur 4 lapisan SI telah terdefinisi konsisten.
- Tabel IPO mencakup kriteria _Storage_ dan _Control_ (penanganan eror).
- Flowchart menggambarkan logika percabangan (_IF-ELSE_) dan perulangan (_Loops_) tanpa _infinite loop_.
- Pseudocode terstruktur dengan rapi dan independen terhadap bahasa pemrograman.
- Form **TPL-07 (AI Usage Disclosure & Verification Note)** telah dilampirkan.

**Tanggal Pengesahan**: ________________  
**Tanda Tangan Phase Lead 4 (Design)**: ________________  
**Tanda Tangan Dosen Pembimbing / Coach**: ________________
