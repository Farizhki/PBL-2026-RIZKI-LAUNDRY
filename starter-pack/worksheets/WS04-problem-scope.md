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
| **Nama Kelompok / Kelas**     | Kelompok Tulip / Kelas A               |
| **Phase Lead 2 (Frame - M2)** | Mutia Fatmawati — 2600016049           |
| **Nama UMKM Mitra Lapangan**  | Rizky Laundry                          |
| **Pemilik / Kontak Mitra**    | Rezza Rahayu (082317480455)            |

## **2\. Matriks Problem Framing & Analisis Akar Masalah (Root Cause Analysis)**

Gunakan temuan kuantitatif dari WS03 untuk memisahkan antara **Gejala Permukaan (_Symptoms_)** dan **Akar Masalah Utama (_Root Cause_)** operasional bisnis mitra:

| **No** | **Kategori Observasi**      | **Gejala Permukaan (_Symptoms_)**                                                                            | **Akar Masalah Operasional (_Root Cause_)**                                                                                                                                    | **Bukti Kuantitatif (_Baseline Data_)**                                                          |
| ------ | --------------------------- | ------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------ |
| **1**  | **Proses Transaksi Kasir**  | Pencatatan transaksi masih dilakukan secara manual menggunakan nota dan buku besar.                         | Belum ada sistem pencatatan transaksi terstruktur dan penghitungan harga otomatis, sehingga perhitungan manual memakan waktu dan berisiko salah hitung.                         | Rata-rata waktu transaksi = **2 menit (120 detik)/orang**.                                       |
| **2**  | **Pencarian Data Pelanggan**| Pemilik harus membalik-balik buku besar lembar demi lembar saat pelanggan mengambil pakaian.               | Data transaksi tidak terindeks digital sehingga pencarian status pembayaran dan data pelanggan lambat dan merepotkan.                                                         | Pencarian status pembayaran manual dilakukan pada setiap pengambilan cucian.                     |
| **3**  | **Rekapitulasi Transaksi**  | Pemilik jarang merekap transaksi berkala; hanya rekap pengeluaran yang dilakukan rutin seminggu sekali.     | Rekapitulasi transaksi belum terlaksana karena terhambat status cucian pelanggan yang belum lunas, sehingga pemilik kesulitan mengakumulasi total penerimaan secara manual.    | Rekapitulasi transaksi harian/mingguan belum berjalan teratur.                                   |

## **3\. Perumusan Problem Statement Kontekstual**

Berdasarkan analisis di atas, rumuskan **Problem Statement** utama dalam 1–2 paragraf terstruktur.  
_Petunjuk_: Hindari mendefinisikan masalah sebagai _"Mitra belum memiliki aplikasi Python/komputer"_. Definisikan dari hambatan bisnis nyata mitra!

**Rumusan Problem Statement Kelompok**:  
"Pencatatan transaksi pesanan pelanggan masih dilakukan secara manual menggunakan buku catatan dan kertas nota di Rizky Laundry. Ketiadaan kalkulasi otomatis berisiko menimbulkan kesalahan hitung tarif (1–2 kali per bulan) dan memerlukan waktu pencatatan rata-rata 2 menit per transaksi.

Selain itu, sistem pencarian status pesanan pelanggan masih dilakukan secara manual dengan menelusuri halaman buku catatan satu per satu saat pelanggan datang mengambil pakaian. Di sisi lain, pemilik belum dapat melakukan rekapitulasi transaksi secara rutin karena terkendala oleh status cucian pelanggan yang belum melunasi pembayaran saat transaksi awal dicatat."

## **4\. Menetapkan Batasan Sistem (System Boundary / Scope Alignment)**

Untuk mencegah terjadinya pembengkakan fitur (_Scope Creep_) yang membahayakan penyelesaian proyek dalam 1 semester, tentukan secara tegas apa yang Masuk Cakupan (_In-Scope_) dan apa yang Di Luar Cakupan (_Out-of-Scope_):

```text
+-----------------------------------------------------------------------------+
|                      SYSTEM BOUNDARY (BATASAN SISTEM)                       |
+-----------------------------------------------------------------------------+
| [ IN-SCOPE: Fitur yang Akan Dibangun ]                                      |
| 1. Pencatatan transaksi pelanggan (dilengkapi kalkulator hitung otomatis).  |
| 2. Pencatatan dan pembaruan status pembayaran (lunas, belum lunas, DP).    |
| 3. Pencarian data transaksi berdasarkan nama atau nomor telepon.            |
| 4. Pencetakan ringkasan rekapitulasi transaksi mingguan untuk pemilik.      |
+-----------------------------------------------------------------------------+
| [ OUT-OF-SCOPE: Di Luar Cakupan Proyek ]                                    |
| 1. Integrasi gateway pembayaran e-wallet / QRIS otomatis.                   |
| 2. Rekapitulasi pengeluaran operasional usaha.                              |
| 3. Pemesanan dan manajemen stok barang otomatis.                            |
+-----------------------------------------------------------------------------+
```

### **Tabel Penegasan Cakupan Proyek (*Scope Alignment Table*)**

| **No** | **Modul / Fitur Sistem**            | **Status Cakupan (_In-Scope / Out-of-Scope_)** | **Alasan Pertimbangan Kelayakan (O'Brien)**                                                                                                                                          |
| ------ | ----------------------------------- | ---------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| **1**  | Pencatatan transaksi pelanggan      | **IN-SCOPE**                                   | Dibutuhkan karena pencatatan transaksi masih dilakukan manual, sehingga fitur ini dapat membuat pencatatan menjadi lebih terstruktur.                                                |
| **2**  | Pencatatan status pembayaran        | **IN-SCOPE**                                   | Dapat mempermudah pemilik untuk melihat status pembayaran setiap pelanggan, apakah lunas atau belum lunas.                                                                      |
| **3**  | Pencarian data transaksi            | **IN-SCOPE**                                   | Membantu pemilik agar lebih mudah menemukan data pelanggan tanpa harus membuka dan mencari data pelanggan secara manual di buku besar.                                               |
| **4**  | Pembayaran Online / Payment Gateway | **OUT-OF-SCOPE**                               | Keterbatasan waktu 1 semester & kompleksitas API luar di PBL Level 1.                                                                                                                |
| **5**  | Rekapitulasi pengeluaran            | **OUT-OF-SCOPE**                               | Rekapitulasi pengeluaran tidak dilakukan karena focus utama pada pencatatan transaksi, juga karena rekapitulasi pengeluaran membutuhkan data yang berbeda dari pencatatan transaksi. |
| **6**  | Pemesanan stock otomatis            | **OUT-OF-SCOPE**                               | Pembelian masih dilakukan ketika diketahui stock menipis atau habis, juga karena belum ada pencatatan stock yang terstruktur.                                                        |                                                |

## **5\. Target Metrik Keberhasilan Solusi (To-Be Targets)**

Tentukan target kuantitatif perbaikan yang ingin dicapai melalui solusi sistem informasi To-Be:

| **Indikator Kinerja**                            | **Kondisi As-Is (Baseline)** | **Target To-Be (Expected)** | **Estimasi Persentase Peningkatan**                      |
| ------------------------------------------------ | ---------------------------- | --------------------------- | -------------------------------------------------------- |
| **Waktu Pelayanan Transaksi Kasir**              | 120 detik / pelanggan        | **< 70 detik / pelanggan**  | Efisiensi waktu pelayanan **41.7%**                     |
| **Durasi Pencarian Status Transaksi Pelanggan**  |  / pencarian manual | ** / pencarian**  | Efisiensi pencarian data > ****                       |
| **Frekuensi Kesalahan Pencatatan/Selisih**   | 1–2 kali / bulan             | **Mengurangi Frekuensi Pencatatan** | Penurunan tingkat frekuensi kesalahan Pencatatan/selisih |

## **6\. Refleksi & Lembar Pengesahan Phase Lead**

### **A. Pertanyaan Refleksi Tim**

1. _Bagaimana tim memastikan bahwa batasan proyek yang ditetapkan realistis untuk diselesaikan dalam 16 minggu?_
   - **Jawab**: kami memastikan batasan project tetap realistis dan dapat di selesaikan dalam waktu 16 minggu, dengan mempertimbangkan hasil observasi dan wawancara yang telah dilakukan dengan mitra juga kemampuan teknis kami yang masih awam untuk pengembangannya.
2. _Apakah pemilik usaha mitra telah menyetujui batasan sistem yang diusulkan oleh kelompok?_
   - **Jawab**: Kami telah berdiskusi dengan mitra dan menyampaikan batasan project agar fitur yang dikembangkan dapat sesuai dengan kebutuhan mitra dan realistis untuk di selesaikan.

### **B. Tanda Tangan Pengesahan Phase Lead 2**

Disusun oleh Phase Lead 2 (Frame): Mutia Fatmawati — 2600016049  

Tanggal Penyusunan: 19/10/2026  

Tanda Tangan Phase Lead 2: [Tanda Tangan Digital](../assets/tanda_tangan/Tanda%20tangan%20Mutia.jpeg)  

Diverifikasi oleh Dosen Pengampu / Coach:  

Tanggal: 20/10/2026 | Status Checkpoint: [ APPROVED ]  
Catatan Dosen: Disetujui untuk lanjut ke Fase 3 (Define).  

---
