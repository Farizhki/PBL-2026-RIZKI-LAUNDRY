# **LEMBAR KERJA MAHASISWA: WS09**
## **PROTOTYPE DEVELOPMENT PLAN & MODULE DECOMPOSITION**

* **Mata Kuliah**: Konsep Sistem Informasi (KSI)  
* **Kerangka Kerja**: Project-Based Learning (PBL) Level 1 — Fase 5 (Build)  
* **Fase Learning Spine**: **Fase 5 — Build: Simple CLI Prototype**  
* **Peran Phase Lead**: **Mahasiswa A (Phase Lead 5 — Build)**  
* **Keterkaitan Artefak**: Rencana Pengembangan untuk **Deliverable D3 (Tested Prototype - TPL-03)**  

---

### **1. IDENTITAS KELOMPOK & DOKUMEN RUJUKAN**
* **Nama Kelompok / Kelas**: __________________________________________________
* **Objek UMKM Mitra**: __________________________________________________
* **Phase Lead 5 (Build)**: __________________________________________________ (NIM: __________________)
* **Dokumen Rujukan D2**: Deliverable D2 (System & Solution Design) tanggal: _______________

---

### **2. TABEL DEKOMPOSISI MODUL & PEMBAGIAN OWNERSHIP FITUR**

Petunjuk: Pecah spesifikasi D2 (*IPO & Flowchart*) menjadi 3–5 modul program CLI terisolasi dan alokasikan penanggung jawab (*PIC*) individu secara adil.

| Kode Modul | Nama Modul Program CLI | Deskripsi Fungsi & Fitur Utama | Penanggung Jawab (PIC Individu) | Target Estimasi Waktu (Jam) |
| :---: | :--- | :--- | :--- | :---: |
| **MOD-01** | **Main Menu & Navigation (`main.py`)** | Menampilkan menu utama konsol, mengelola perulangan navigasi, dan *exit application*. | [Nama Mahasiswa / NIM] | ____ Jam |
| **MOD-02** | **Kasir & Transaksi (`pos_module.py`)** | Input kode barang, validasi stok, hitung subtotal, proses bayar/kembalian, & simpan transaksi. | [Nama Mahasiswa / NIM] | ____ Jam |
| **MOD-03** | **Inventaris & Data (`inventory_module.py`)** | Load & save data `inventory.json`, pembaruan sisa stok *real-time*, & tampilan katalog. | [Nama Mahasiswa / NIM] | ____ Jam |
| **MOD-04** | **Laporan & Rekap (`report_module.py`)** | Membaca `sales_log.json`, menghitung total omzet harian, dan menampilkan ringkasan transaksi. | [Nama Mahasiswa / NIM] | ____ Jam |

---

### **3. JADWAL SPRINT & MILESTONE PENGERJAAN**

| Tahapan Sprint | Target Deliverable / Fitur | Tanggal Target Selesai | Kriteria Selesai (*Definition of Done*) |
| :--- | :--- | :---: | :--- |
| **Sprint 1 (M9)** | Skeleton Modul Main & Inisialisasi Data JSON | DD/MM/YYYY | Menu CLI terbuka dan file `inventory.json` terbaca tanpa eror. |
| **Sprint 2 (M10)** | Modul Kasir & Auto Update Stok (POS) | DD/MM/YYYY | Transaksi berjalan, kalkulasi kembalian tepat, stok berkurang otomatis. |
| **Sprint 3 (M11)** | Error Handling, Sesi Critique II & Fix Bugs | DD/MM/YYYY | Bebas crash saat input salah, lulus pengujian teman sejawat. |
| **Sprint 4 (M12)** | Modul Laporan, Validasi UAT Mitra, & D3 Final | DD/MM/YYYY | Laporan omzet tercetak, UAT disetujui pemilik UMKM mitra. |

---

### **4. LEMBAR PENGESAHAN WS09**

| Peran | Nama Mahasiswa | NIM | Tanda Tangan | Tanggal |
| :--- | :--- | :---: | :---: | :---: |
| **Phase Lead 5 (Build)** | ________________________ | ______________ | _______________ | ___________ |
| **Anggota Tim 1** | ________________________ | ______________ | _______________ | ___________ |
| **Anggota Tim 2** | ________________________ | ______________ | _______________ | ___________ |
| **Anggota Tim 3** | ________________________ | ______________ | _______________ | ___________ |

* **Dosen Pengampu / Coach**: ________________________ | **Status Checkpoint WS09**: [  ] Disetujui  [  ] Revisi Minor
