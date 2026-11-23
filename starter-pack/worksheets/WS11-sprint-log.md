# **LEMBAR KERJA MAHASISWA: WS11**
## **IMPLEMENTATION SPRINT LOG & PROGRESS TRACKING**

* **Mata Kuliah**: Konsep Sistem Informasi (KSI)  
* **Kerangka Kerja**: Project-Based Learning (PBL) Level 1 — Fase 5 (Build)  
* **Fase Learning Spine**: **Fase 5 — Build: Implementation Sprint**  
* **Peran Phase Lead**: **Mahasiswa A (Phase Lead 5 — Build)**  
* **Keterkaitan Artefak**: Pendukung **Deliverable D3 (TPL-03)** & **TPL-09 (Meeting Log)**  

---

### **1. IDENTITAS KELOMPOK**
* **Nama Kelompok / Kelas**: __________________________________________________
* **Objek UMKM Mitra**: __________________________________________________

---

### **2. REKAPITULASI PROGRES IMPLEMENTASI SPRINT MINGGUAN**

| Minggu / Sprint | Target Fitur / Modul | PIC Anggota | Status Progres (%) | Kendala Teknis Yang Dihadapi | Tindakan Solusi / Resolusi |
| :---: | :--- | :--- | :---: | :--- | :--- |
| **M9 / Sprint 1** | Setup File JSON & Menu CLI | Mahasiswa A | 100% | File JSON korupsi saat di-write. | Menggunakan fungsi `json.dump()` dengan indentasi rapi. |
| **M10 / Sprint 2** | Transaksi Kasir & Update Stok | Mahasiswa B | 85% | Stok bernilai minus jika dibeli banyak.| Menambahkan validator `IF stok >= qty_beli`. |
| **M11 / Sprint 3** | Exception Handling & Critique Fix | Mahasiswa C | 90% | Format cetak konsol berantakan. | Menggunakan format string `f-string` dengan lebar kolom tetap. |
| **M12 / Sprint 4** | Laporan Omzet & Validasi UAT | Mahasiswa D | 100% | Pembacaan timestamp JSON eror. | Menggunakan modul standar `datetime` Python. |

---

### **3. LEMBAR PENGESAHAN SPRINT LOG**

* **Phase Lead 5 (Build)**: ________________________ (NIM: _______________)
* **Tanggal Diverifikasi**: _______________
