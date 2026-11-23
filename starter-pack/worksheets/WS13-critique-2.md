# **LEMBAR KERJA MAHASISWA: WS13**
## **CRITIQUE II & ITERATION REVIEW**

* **Mata Kuliah**: Konsep Sistem Informasi (KSI)  
* **Kerangka Kerja**: Project-Based Learning (PBL) Level 1 — Fase 6 (Test)  
* **Fase Learning Spine**: **Fase 6 — Test: Peer Critique II**  
* **Peran Phase Lead**: **Mahasiswa B (Phase Lead 6 — Test)**  
* **Keterkaitan Artefak**: Pendukung **Deliverable D3 (TPL-03)** & **TPL-08 (Decision Log)**  

---

### **1. IDENTITAS EVALUASI SILANG**
* **Kelompok Pemaji / Pemilik Prototipe**: Kelompok ____ ("______________________")
* **Kelompok Penilai / Evaluator**: Kelompok ____ ("______________________")
* **Tanggal Sesi Critique II**: ____ / ____ / 2026

---

### **2. MATRIKS EVALUASI SISI CRITIQUE II (IMPLEMENTATION REVIEW)**

Petunjuk: Berikan umpan balik kualitatif berbasis aturan *Be Kind, Be Specific, Be Helpful*.

| Aspek Pengujian Implementasi | Hal Yang Sudah Sangat Baik (*I Like...*) | Area Yang Perlu Diperbaiki (*I Wonder...*) | Usulan Solusi Iterasi (*What If...*) |
| :--- | :--- | :--- | :--- |
| **1. Usability Tampilan CLI** | Tampilan menu rapi dan mudah dibaca. | Tulisan teks terlalu rapat saat memilih menu. | Bagaimana jika diberi pemisah garis bintang/sama dengan? |
| **2. Kebenaran Logika Transaksi** | Kalkulasi total belanja dan kembalian 100% akurat. | Belum ada konfirmasi sebelum transaksi disimpan. | Bagaimana jika ditambah konfirmasi "Proses transaksi? Y/N"? |
| **3. Ketahanan Error Handling** | Aplikasi tidak crash saat diisi input huruf pada nominal. | Jika file `inventory.json` hilang, sistem bingung. | Bagaimana jika dibuat fungsi pembuat file JSON default? |

---

### **3. TINDAK LANJUT REVISI PADA DECISION LOG (TPL-08)**

* **Rencana Perbaikan Yang Diterima**:
  1. Menambahkan garis pemisah rapi pada tampilan menu konsol.
  2. Menambahkan dialog konfirmasi "Y/N" sebelum menyimpan transaksi ke file log.
* **Pengesahan Phase Lead 6**: ________________________ | **Tanggal**: _______________
