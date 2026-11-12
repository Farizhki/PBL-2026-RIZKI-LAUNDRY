# D1 — Problem Brief

**Project**: Digital Problem Framing Mini Project — Rizky Laundry
**Tim**: Kelompok Tulip (Deva Nayla Maisya, Mutia Fatmawati, Farizhki, M. Faris Ilham, M. Zacky Alfattah) | **Tanggal**: 19/10/2026 | **Versi**: v1.0
**Template**: TPL-01

> Worksheet terkait: WS03, WS04

---

## 1. Profil Organisasi / Unit Usaha

- **Nama unit usaha**: Rizky Laundry
- **Jenis usaha / layanan**: Laundry
- **Lokasi**: Jl. Tegal Mulyo No.RT05 RW06, Tamanan, Kec. Banguntapan, Kab. Bantul, Daerah Istimewa Yogyakarta 55191 (~300m selatan kampus)
- **Deskripsi singkat operasional**: Laundry yang beroperasi setiap hari mulai pukul 07.00–21.00 WIB. Seluruh kegiatan operasional dilakukan langsung oleh pemilik laundry, mulai dari penerimaan pesanan pakaian, penimbangan, pencatatan transaksi di buku dan nota, proses pencucian, hingga penyerahan dan penerimaan pembayaran.
- **Narahubung / pemilik**: Rezza Rahayu (pemilik), 082317480455

## 2. Deskripsi Masalah Utama

- **Masalah utama**: Pencatatan transaksi masih dilakukan secara manual menggunakan buku catatan dan kertas nota. Sistem pencarian data pelanggan masih manual dengan menelusuri buku catatan lembar demi lembar untuk memastikan status pembayaran pelanggan saat pengambilan cucian. Di samping itu, pemilik jarang melakukan rekapitulasi transaksi harian/mingguan secara rutin karena masih terdapat transaksi pelanggan yang belum lunas. Pencatatan persediaan bahan baku (stok) juga belum terstruktur sehingga pembelian barang hanya dilakukan saat pemilik melihat persediaan menipis atau habis.
- **Pihak yang terdampak**: Pemilik laundry, karena harus melayani transaksi secara manual, menghitung biaya tanpa sistem otomatis, dan menelusuri buku catatan satu per satu saat pelanggan mengambil laundry.
- **Frekuensi / keparahan**: Terjadi secara berkala; frekuensi kesalahan pencatatan atau koreksi (seperti lupa mencatat item tambahan sprei/selimut atau kesalahan hitung manual total biaya) terjadi sekitar 1–2 kali dalam sebulan, yang membuat pemilik memerlukan waktu tambahan untuk melakukan konfirmasi ulang dengan pelanggan.

## 3. Batasan Sistem (Scope)

- **Diselesaikan dalam proyek ini**: 
  1. Pencatatan data transaksi pesanan pelanggan secara terstruktur (nama, nomor telepon, pilihan paket layanan, berat/satuan, dan kalkulator hitung otomatis total harga).
  2. Pencatatan dan pembaruan status pembayaran (lunas, belum lunas, DP).
  3. Pencarian data transaksi pelanggan berdasarkan nama atau nomor telepon.
- **Tidak diselesaikan (dan alasan)**: 
  1. Integrasi gateway pembayaran online / QRIS otomatis.
  2. Rekapitulasi pengeluaran operasional (fokus utama proyek adalah pencatatan transaksi masuk dan status pembayaran pelanggan, serta memerlukan struktur data yang berbeda).
  3. Pemesanan dan manajemen stok otomatis (pencatatan stok belum terstruktur dan pembelian bahan masih dilakukan manual saat habis).
- **Asumsi yang dipakai**: Sistem pencatatan dan pencarian transaksi akan digunakan langsung oleh pemilik Rizky Laundry berbasis Spreadsheet. Data transaksi dimasukkan secara manual oleh pemilik.

## 4. Data Kuantitatif Pendukung

| Indikator | Nilai/Baseline | Sumber Data | Tanggal |
|---|---|---|---|
| Waktu layanan transaksi rata-rata | 2 menit/pelanggan | Pemilik laundry (Wawancara 1 & Observasi) | 07/10/2026 |
| Jumlah pelanggan pada jam sibuk | 4–7 orang/hari | Pemilik laundry (Wawancara 1) | 07/10/2026 |
| Frekuensi kesalahan pencatatan/selisih hitung | 1–2 kali/bulan | Pemilik laundry (Wawancara 1 & 2) | 07/10/2026 |

## 5. Pernyataan Kebutuhan Awal (ringkasan ke D2)

- Kebutuhan inti yang akan dijawab prototipe:
  1. **Pencatatan Transaksi**: Input data terstruktur yang mencakup nama pelanggan, nomor telepon, pilihan paket (express, komplit, cuci saja, setrika saja, atau satuan sprei/selimut), berat pakaian, serta status pembayaran dengan kalkulasi otomatis total harga.
  2. **Pencarian dan Pembaruan Status**: Mencari data pesanan berdasarkan nama atau nomor telepon untuk melihat sekaligus memperbarui status pembayaran.
  3. **Rekapitulasi Periode**: Menampilkan rekapitulasi total transaksi atau pendapatan dalam rentang waktu mingguan/per-hari sesuai kebutuhan pemilik.

## 6. Daftar Rujukan / Bukti

- Observasi lapangan tanggal: 07/10/2026
- Wawancara pemilik (Wawancara 1 & 2) tanggal: 07/10/2026
- Bukti pendukung pada folder `starter-pack/assets/`: [[Bukti]](https://github.com/Farizhki/PBL-2026-RIZKI-LAUNDRY/tree/c2a3af791fb2bbf21b75751effdd85849910a724/starter-pack/assets)
  - Transkrip Wawancara 1 & 2 (`assets/transkrip/`) [[Bukti]](https://github.com/Farizhki/PBL-2026-RIZKI-LAUNDRY/tree/c2a3af791fb2bbf21b75751effdd85849910a724/starter-pack/assets)
  - Audio Rekaman Wawancara 1 & 2 (`assets/rekaman_suara/`) [[Bukti]](https://github.com/Farizhki/PBL-2026-RIZKI-LAUNDRY/tree/c2a3af791fb2bbf21b75751effdd85849910a724/starter-pack/assets)
  - Foto Dokumentasi Lapangan (`assets/foto/Dokumentasi wawancara 1.jpg`) [[Bukti]](https://github.com/Farizhki/PBL-2026-RIZKI-LAUNDRY/tree/c2a3af791fb2bbf21b75751effdd85849910a724/starter-pack/assets)
  - Lembar Komitmen dan Tanda Tangan Anggota Tim (`assets/tanda_tangan/`) [[Bukti]](https://github.com/Farizhki/PBL-2026-RIZKI-LAUNDRY/tree/c2a3af791fb2bbf21b75751effdd85849910a724/starter-pack/assets)

---

**Status**: ☑ Draf → ⬜ Review Tim → ⬜ Validasi Pemilik → ⬜ Final (Gate 1)
