# **LEMBAR KERJA MAHASISWA: WS10**
## **CODE WALKTHROUGH & INTERNAL TESTING LOG**

* **Mata Kuliah**: Konsep Sistem Informasi (KSI)  
* **Kerangka Kerja**: Project-Based Learning (PBL) Level 1 — Fase 5 (Build)  
* **Fase Learning Spine**: **Fase 5 — Build: Testing & Verification**  
* **Peran Phase Lead**: **Mahasiswa A (Phase Lead 5 — Build)**  
* **Keterkaitan Artefak**: Pendukung **Deliverable D3 (TPL-03)** & Persiapan **Gate 2 Code Walkthrough**  

---

### **1. IDENTITAS KELOMPOK**
* **Nama Kelompok / Kelas**: __________________________________________________
* **Objek UMKM Mitra**: __________________________________________________

---

### **2. MATRIKS LOG PENGUJIANKASUS UJI INTERNAL (INTERNAL TEST CASES LOG)**

Petunjuk: Catat setiap pengujian internal yang dilakukan oleh tim sebelum kunjungan ke lokasi mitra.

| ID Uji | Nama Modul / Fitur | Input Uji Mandiri | Hasil Yang Diharapkan | Hasil Aktual Eksekusi | Status (Lulus / Gagal) | Tindakan Perbaikan (Jika Gagal) |
| :---: | :--- | :--- | :--- | :--- | :---: | :--- |
| **TC-01** | Modul POS / Input Kode | Input kode barang `KOP-01` valid | Nama barang & harga muncul presisi | Sesuai harapan | **LULUS** | Tidak ada. |
| **TC-02** | Modul POS / Validation | Input kode barang `X99` tidak ada | Pesan "Kode barang tidak ditemukan" | Program crash KeyError | **GAGAL** | Menambahkan pengecekan `IF code IN data`. |
| **TC-03** | Modul POS / Error Qty | Input kuantitas `ABC` (string) | Pesan "Input harus berupa angka" | Program crash ValueError | **GAGAL** | Menambahkan penanganan `try-except ValueError`. |
| **TC-04** | Modul Stok / Auto Update | Beli `KOP-01` qty `5` (stok `50`) | Stok di `inventory.json` jadi `45` | Stok berkurang jadi 45 | **LULUS** | Tidak ada. |
| **TC-05** | Modul Bayar / Kembalian | Total `Rp 15.000`, bayar `Rp 20.000` | Kembalian `Rp 5.000` | Kembalian Rp 5.000 | **LULUS** | Tidak ada. |

---

### **3. LEMBAR CODE WALKTHROUGH INDIVIDU (LEMBAR PENALARAN KODE)**

Setiap anggota tim wajib memilih 1 fungsi/modul utama yang ditulis dan menjelaskan penalaran kodenya secara mandiri:

```
+-----------------------------------------------------------------------------------+
| ANGGOTA 1: [Nama Mahasiswa / NIM]                                                 |
+-----------------------------------------------------------------------------------+
| Modul Yang Ditulis: MOD-02 (pos_module.py - Fungsi Hitung Kembalian)              |
| Penjelasan Logika Baris Kode Utama:                                               |
| - Baris 12-15: Membaca total belanjaan dari list keranjang sementara.            |
| - Baris 18: Melakukan perulangan WHILE untuk meminta input uang_bayar.            |
| - Baris 21: Memeriksa kondisi IF uang_bayar < total_belanja. Jika kurang,          |
|   menampilkan pesan error dan mengulang input.                                    |
| - Baris 25: Jika cukup, menghitung kembalian = uang_bayar - total_belanja.        |
+-----------------------------------------------------------------------------------+
```

---

### **4. LEMBAR PENGESAHAN WS10**

* **Phase Lead 5**: ________________________ | **Tanggal**: _______________
* **Catatan Dosen Pengampu**: _________________________________________________________________
