# **WS04: Problem Identification & Scope**

**Mata Kuliah**: Konsep Sistem Informasi (KSI)  
**Kerangka Kerja**: Project-Based Learning (PBL) Level 1  
**Fase Learning Spine**: **Fase 2 — Frame (Problem Discovery & Scope)**  
**Minggu / Alokasi Waktu**: Minggu 2 / 14 Jam Belajar  
**Sub-CPMK / SFIA**: S-01.1 (Introduce - Problem Framing) | SFIA BUSA L1 (_Business Analysis_), IRMG L1  
**Penanggung Jawab Fase**: **Phase Lead 2 (Frame — Mahasiswa B)**  
**Keterkaitan Deliverable**: Sumber Utama Penyusunan **Deliverable D1 (Problem Brief - TPL-01)**

## **1\. Identifikasi Tim & Objek Proyek**

| **Elemen Informasi**          | **Rincian Identitas Kelompok & Mitra** |
| ----------------------------- | -------------------------------------- |
| **Nama Kelompok / Kelas**     | Kelompok Tulip                         |
| **Phase Lead 2 (Frame - M2)** | Mutia Fatmawati — 2600016049           |
| **Nama UMKM Mitra Lapangan**  | Rizky Laundry                          |
| **Pemilik / Kontak Mitra**    | Rezza Rahayu                           |

## **2\. Matriks Problem Framing & Analisis Akar Masalah (Root Cause Analysis)**

Gunakan temuan kuantitatif dari WS03 untuk memisahkan antara **Gejala Permukaan (_Symptoms_)** dan **Akar Masalah Utama (_Root Cause_)** operasional bisnis mitra:

| **No** | **Kategori Observasi**      | **Gejala Permukaan (_Symptoms_)**                                                                            | **Akar Masalah Operasional (_Root Cause_)**                                                                                                                                    | **Bukti Kuantitatif (_Baseline Data_)**                                                          |
| ------ | --------------------------- | ------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------ |
| **1**  | **Proses Transaksi Kasir**  | Pencatatan transaksi masih dilakukan secara manual.                                                          | Belum ada sistem pencatatan transaksi dan penghitungan total harga yang terstruktur oleh mitra sehingga masih dilakukan manual di buku dan nota.                               | Rata-rata waktu transaksi = **2 menit/orang**                                                    |
| **2**  | **Pengelolaan Stok Barang** | Pembelian bahan baku dilakukan ketika pemilik melihat stock menipis atau habis.                              | Pencatatan stok belum dicatat secara terstruktur untuk memantau persediaan.                                                                                                    | Belum ada data kuantitatif mengenai pengelolaan stock barang persediaan dan pembelian kebutuhan. |
| **3**  | **Rekapitulasi Keuangan**   | Pemilik hanya melakukan rekapitulasi pengeluaran setiap minggu, dan jarang melakukan rekapitulasi transaksi. | Pemilik tidak melakukan rekapitulasi transaksi karena terdapat pelanggan yang belum melunasi pembayaran yang membuat pemilik membuat pemilik memilih untuk tidak melakukannya. | Durasi rekapitulasi penggeluaran mingguan = **30-60 menit/minggu**.                               |

## **3\. Perumusan Problem Statement Kontekstual**

Berdasarkan analisis di atas, rumuskan **Problem Statement** utama dalam 1–2 paragraf terstruktur.  
_Petunjuk_: Hindari mendefinisikan masalah sebagai _"Mitra belum memiliki aplikasi Python/komputer"_. Definisikan dari hambatan bisnis nyata mitra!

**Rumusan Problem Statement Kelompok**:  
"Pencatatan transaksi dan pengeluaran masih dilakukan secara manual menggunakan buku dan kertas nota di Rezza Laundry. Dengan pencatatan stock yang masih belum terstruktur untuk memantau persediaan, sehingga pembelian barang dilakukan ketika pemilik melihat persediaan menipis atau sudah habis.

Sistem pencarian data pelanggan masih dilakukan secara manual, yaitu dengan menelusuri buku catatan untuk memastikan status pembayaran pelanggan saat mengambil pesanan.

Di sisi lain, pemilik juga hanya melakukan rekapitulasi pengeluaran rutin setiap minggu tanpa melakukan rekapitulasi transaksi secara rutin. Karena masih terdapat pelanggan yang belum melunasi pembayaran."

4. Menetapkan Batasan Sistem (System Boundary / Scope Alignment)
Untuk mencegah terjadinya pembengkakan fitur (Scope Creep) yang membahayakan penyelesaian proyek dalam 1 semester, tentukan secara tegas apa yang Masuk Cakupan (In-Scope) dan apa yang Di Luar Cakupan (Out-of-Scope):

 ```text
+-----------------------------------------------------------------------------+
|                      SYSTEM BOUNDARY (BATASAN SISTEM)                       |
+-----------------------------------------------------------------------------+
| [ IN-SCOPE: Fitur yang Akan Dibangun ]                                      |
| 1. Pencatatan transaksi pelanggan.                                          |
| 2. Pencatatan status pembayaran.                                            |
| 3. Pencarian data transaksi.                                                |
| 4. Pencetakan ringkasan rekapitulasi mingguan untuk pemilik.                |
+-----------------------------------------------------------------------------+
| [ OUT-OF-SCOPE: Di Luar Cakupan Proyek ]                                    |
| 1. Integrasi gateway pembayaran e-wallet / QRIS otomatis.                   |
| 2. Rekapitulasi pengeluaran.                                                |
| 3. Pemesanan stok otomatis.                                                 |
+-----------------------------------------------------------------------------+
```
### **Tabel Penegasan Cakupan Proyek (*Scope Alignment Table*)**

| **No** | **Modul / Fitur Sistem**            | **Status Cakupan (_In-Scope / Out-of-Scope_)** | **Alasan Pertimbangan Kelayakan (O'Brien)**                                                                                                                                          |
| ------ | ----------------------------------- | ---------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| **1**  | Pencatatan transaksi pelanggan      | **IN-SCOPE**                                   | Dibutuhkan karena pencatatan transaksi masih dilakukan manual, sehingga fitur ini dapat membuat pencatatan menjadi lebih terstruktur.                                                |
| **2**  | Pencatatan status pembayaran        | **IN-SCOPE**                                   | Dapat mempermudah pemilik untuk melihat status pembayaran setiap pelanggan, apakah lunas, belum lunas, atau dp.                                                                      |
| **3**  | Pencarian data transaksi            | **IN-SCOPE**                                   | Membantu pemilik agar lebih mudah menemukan data pelanggan tanpa harus membuka dan mencari data pelanggan secara manual di buku besar.                                               |
| **4**  | Pembayaran Online / Payment Gateway | **OUT-OF-SCOPE**                               | Keterbatasan waktu 1 semester & kompleksitas API luar di PBL Level 1.                                                                                                                |
| **5**  | Rekapitulasi pengeluaran            | **OUT-OF-SCOPE**                               | Rekapitulasi pengeluaran tidak dilakukan karena focus utama pada pencatatan transaksi, juga karena rekapitulasi pengeluaran membutuhkan data yang berbeda dari pencatatan transaksi. |
| **6**  | Pemesanan stock otomatis            | **OUT-OF-SCOPE**                               | Pembelian masih dilakukan ketika diketahui stock menipis atau habis, juga karena belum ada pencatatan stock yang terstruktur.                                                        |

## **5\. Target Metrik Keberhasilan Solusi (To-Be Targets)**

Tentukan target kuantitatif perbaikan yang ingin dicapai melalui solusi sistem informasi To-Be:

.

| **Indikator Kinerja**               | **Kondisi As-Is (Baseline)** | **Target To-Be (Expected)** | **Estimasi Persentase Peningkatan**      |
| ----------------------------------- | ---------------------------- | --------------------------- | ---------------------------------------- |
| **Waktu Pelayanan Transaksi Kasir** | 90 detik / pelanggan         | **< 30 detik / pelanggan**  | Peningkatan efisiensi **66.7%**          |
| **Durasi Rekapitulasi Harian**      | 60–90 menit / malam          | **< 10 menit / malam**      | Penghematan waktu **83.3%**              |
| **Akurasi Pencatatan Stok**         | Selisih 12% / bulan          | **Akurasi > 98%**           | Penurunan tingkat kesalahan selisih stok |

## **6\. Refleksi & Lembar Pengesahan Phase Lead**

### **A. Pertanyaan Refleksi Tim**

1. _Bagaimana tim memastikan bahwa batasan proyek yang ditetapkan realistis untuk diselesaikan dalam 16 minggu?_
   - **Jawab**: kami memastikan batasan project tetap realistis dan dapat di selesaikan dalam waktu 16 minggu, dengan mempertimbangkan hasil observasi dan wawancara yang telah dilakukan dengan mitra juga kemampuan teknis kami yang masih awam untuk pengembangannya.
2. _Apakah pemilik usaha mitra telah menyetujui batasan sistem yang diusulkan oleh kelompok?_
   - **Jawab**: Kami telah berdiskusi dengan mitra dan menyampaikan batasan project agar fitur yang dikembangkan dapat sesuai dengan kebutuhan mitra dan realistis untuk di selesaikan.

### **B. Tanda Tangan Pengesahan Phase Lead 2**

Disusun oleh Phase Lead 2 (Frame): [ Mutia Fatmawati — 2600016049 ]

---

Tanggal Penyusunan: [ 19/10/2026 ]

Tanda Tangan Phase Lead 2: [Tanda Tangan Digital](https://github.com/Farizhki/PBL-2026-RIZKI-LAUNDRY/blob/8a9ce284bf71a97ea6a02604783b00ed73916244/starter-pack/assets/tanda_tangan/Tanda%20tangan%20Mutia.jpeg)

Diverifikasi oleh Dosen Pengampu / Coach:

Tanggal: [ 20/10/2026 ] | Status Checkpoint: [ APPROVED ]
Catatan Dosen: __________________________________________________

---
