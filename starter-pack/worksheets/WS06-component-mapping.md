# **WORKBOOK: LEMBAR KERJA MAHASISWA WS06**

## **Success Metrics (BPI/DMAIC) & Pemetaan Komponen SI Awal**

Mata Kuliah: **Konsep Sistem Informasi (KSI)**  
Kerangka Kerja: **Project-Based Learning (PBL) Level 1**  
Fase Learning Spine: **Fase 3 — Define (Minggu 4)**  
Sub-CPMK / SFIA: **S-01.1 (Intermediate - Problem Framing) & S-03.1 (Intermediate - Pemetaan SI)** | **SFIA BUSA L1, METR L2**  
Keterkaitan Deliverable: **Bahan Utama Deliverable D1 Final (TPL-01) & D2 Draf (TPL-02)**

### **1\. Identifikasi Kelompok & Rotasi Kepemimpinan**

- **Nama Kelompok**: Kelompok Tulip / Kelas A
- **Objek UMKM Mitra**: Rizky Laundry
- **Phase Lead 3 (Define)**: Deva Nayla Maisya (2600016039)
- **Anggota Tim**: 
1. M. Zacky Alfattah (2600016015)
2. M. Faris Ilham (2600016014)
3. Farizhki (2600016027)
4. Mutia Fatmawati (2600016049)

### **2\. Landasan Konseptual: Metrik BPI & Pemetaan 5 Pilar SI**

- **Business Process Improvement (BPI)** mengukur keberhasilan perbaikan proses bisnis melalui dua dimensi utama (Rainer et al., 2014):
  - **Efisiensi (_Efficiency_)**: Mengukur penghematan sumber daya (_doing things well_), seperti efisiensi waktu siklus transaksi atau reduksi biaya operasional.
  - **Efektivitas (_Effectiveness_)**: Mengukur pencapaian kualitas/tujuan (_doing the right things_), seperti akurasi data transaksi, penurunan angka kesalahan hitung tarif kasir, dan kepuasan pelanggan.
- **Model 5 Pilar SI O'Brien**: Solusi sistem informasi dipetakan ke dalam pilar _People, Hardware, Software, Data,_ dan _Network_ (Marakas & O'Brien, 2013).

### **3\. Workspace A: Matrik Metrik Keberhasilan Bisnis (DMAIC Six Sigma)**

| **Dimensi Metrik** | **Parameter Kinerja** | **Kondisi Baseline (As-Is)** | **Target Solusi (To-Be)** | **Metode Pengukuran** |
| :--- | :--- | :--- | :--- | :--- |
| **Efisiensi (Waktu)** | Durasi pelayanan transaksi input pesanan per pelanggan | 120 detik (2 menit) / transaksi | **< 70 detik / transaksi** | Stopwatch sampel 10 transaksi input pesanan |
| **Efisiensi (Waktu)** | Durasi pencarian data transaksi & status cucian pelanggan | 30–60 detik / pencarian manual di buku besar | **< 10 detik / pencarian** | Uji coba pencarian data berdasarkan nama atau nomor telepon |
| **Efisiensi (Waktu)** | Durasi penyusunan rekapitulasi transaksi mingguan pemilik | Jarang dilakukan / tidak teratur (>30 menit) | **< 15 menit / minggu** | Pengujian simulasi rekapitulasi data transaksi mingguan |
| **Efektivitas (Kualitas & Akurasi)** | Frekuensi kesalahan hitung nota & selisih tagihan | 1–2 kali / bulan (kesalahan hitung manual) | **0 kali / bulan (Akurasi 100%)** | Audit verifikasi kesesuaian tarif dan kalkulasi otomatis sistem |

### **4\. Workspace B: Pemetaan Arsitektur 5 Pilar SI Solusi Awal**

```text
┌──────────────────────────────────────────────────────────────────────────────┐
│                    PETA 5 PILAR SISTEM INFORMASI O'BRIEN                    │
├──────────────────────────────────────────────────────────────────────────────┤
│ 1. PEOPLE RESOURCES (Pengguna & Spesialis)                                   │
│ • Pengguna Akhir (End User):                                                │
│   Pemilik Rizky Laundry (Rezza Rahayu) sebagai kasir dan operator harian     │
│   yang melayani pelanggan, menginput data transaksi pesanan, mengecek status │
│   pembayaran saat pengambilan pakaian, dan memantau rekapitulasi pendapatan. │
│ • Spesialis SI (IS Specialist):                                              │
│   Tim Pengembang Mahasiswa (Kelompok Tulip) bertindak sebagai System Analyst │
│   dan Program Developer untuk merancang, menguji, dan memelihara sistem.     │
├──────────────────────────────────────────────────────────────────────────────┤
│ 2. HARDWARE RESOURCES (Perangkat Mesin & Media)                              │
│ • Perangkat Fisik Input:                                                     │
│   - Laptop untuk input data transaksi                                        │
│   - Timbangan cucian manual/digital untuk menimbang berat pakaian pelanggan  │
│ • Perangkat Fisik Output:                                                    │
│   - Layar monitor laptop untuk menampilkan antarmuka data transaksi,     │
│     total tagihan, status pembayaran, dan ringkasan rekapitulasi             │
│   - Smartphone pemilik untuk konfirmasi status cucian selesai via WhatsApp   │
├──────────────────────────────────────────────────────────────────────────────┤
│ 3. SOFTWARE RESOURCES (Aplikasi & Prosedur Operasional)                      │
│ • Aplikasi Program:                                                          │
│   - Program aplikasi pencatatan transaksi terstruktur (berbasis antarmuka    │
│     CLI Python / Spreadsheet) dengan fitur kalkulasi otomatis, pencarian     │
│     data pelanggan, dan rekapitulasi periode                                 │
│ • Prosedur Pengguna (SOP):                                                   │
│   1. Penerimaan pakaian kotor dari pelanggan                                 │
│   2. Penimbangan berat pakaian dan penentuan paket layanan                   │
│   3. Input data nama, nomor HP, paket, dan berat ke dalam sistem             │
│   4. Sistem menghitung total harga tagihan secara otomatis                   │
│   5. Konfirmasi status pembayaran (Lunas, Belum Lunas)                       │
│   6. Penyimpanan data transaksi ke berkas data                               │
│   7. Pencarian data pesanan secara cepat saat pelanggan mengambil cucian     │
├──────────────────────────────────────────────────────────────────────────────┤
│ 4. DATA RESOURCES (Struktur Data & Basis Data)                               │
│ • Data Transaksi:                                                            │
│   Berkas data transaksi terstruktur (Spreadsheet) dengan field:              │
│   - ID/Waktu Transaksi (Timestamp)                                           │
│   - Nama Pelanggan (String)                                                  │
│   - Nomor Telepon / WhatsApp (String)                                        │
│   - Pilihan Paket Layanan (Express / Komplit / Cuci Saja / Setrika Saja)     │
│   - Berat Cucian (Float, dalam Kg) atau Jumlah Satuan Sprei/Selimut (Pcs)    │
│   - Total Tagihan Biaya (Integer / Currency)                                 │
│   - Metode Pembayaran (Tunai / QRIS GoPay Merchant)                          │
│   - Status Pembayaran (Lunas / Belum Lunas / DP)                             │
│ • Data Produk / Layanan & Tarif:                                             │
│   Daftar katalog tarif layanan laundry:                                      │
│   - Paket Express (1 hari): Rp8.000 / kg                                     │
│   - Paket Komplit Cuci-Setrika (2–3 hari): Rp6.000 / kg                      │
│   - Paket Cuci Kering Saja: Rp4.000 / kg                                     │
│   - Paket Setrika Saja: Rp5.000 / kg                                         │
│   - Sprei/Selimut Kecil: Rp5.000 / pcs; Sprei/Selimut Besar: Rp10.000 / pcs  │
│   *(Catatan: Pengelolaan stok bahan baku berada di luar cakupan sistem)*     │
├──────────────────────────────────────────────────────────────────────────────┤
│ 5. NETWORK RESOURCES (Jaringan Komunikasi & Media)                           │
│ • Konektivitas:                                                              │
│   - Internet Seluler 4G pada perangkat laptop/ponsel                         │
│     pemilik untuk pengiriman notifikasi pengambilan cucian via WhatsApp      │
│   - Sistem pencatatan berjalan secara mandiri (Local)                        │
└──────────────────────────────────────────────────────────────────────────────┘
```

### **5\. Workspace C: Lembar Persetujuan Formal Mitra (Sign-Off)**

Dengan ini, pemilik / manajer UMKM mitra menyatakan setuju atas rumusan kebutuhan fungsional, target metrik keberhasilan, dan batas cakupan sistem yang dirancang oleh tim mahasiswa.

- **Nama UMKM Mitra**: Rizky Laundry
- **Nama Pemilik / Pengelola**: Rezza Rahayu
- **Tanggal Persetujuan**: 24/10/2026

**Tanda Tangan Persetujuan Mitra**:

*(Rezza Rahayu — Pemilik Rizky Laundry)*

### **6\. Verifikasi Integritas AI (TPL-07) & Pengesahan**

- **Penggunaan AI Co-pilot**:  
  Apakah tim menggunakan AI untuk membantu merumuskan metrik BPI / diagram 5 pilar SI? [ ] Ya [ ] Tidak  
  _(Jika Ya, wajib melampirkan formulir **TPL-07: AI Usage Disclosure & Verification Note**)_

**Tanda Tangan Tim & Pengesahan Dosen**:

- **Phase Lead 3 (Define)**: Deva Nayla Maisya — 2600016039 (Tanggal: 24/10/2026)
- **Dosen Coach**: Muhammad Ibnu Zappriliannur Syadin — 2300016045 (Tanggal: 26/10/2026) [x] Approved
