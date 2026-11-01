# D1 — Problem Brief

**Project**: Digital Problem Framing Mini Project — [Nama Unit Usaha]
**Tim**: [Nama anggota] | **Tanggal**: [DD/MM/YYYY] | **Versi**: [v1.0]
**Template**: TPL-01

> **Petunjuk**: Hapus teks dalam `[...]` dan huruf miring setelah diisi.
> Worksheet terkait: WS03, WS04

---

## 1. Profil Organisasi / Unit Usaha

- **Nama unit usaha**: [Rizky Laundry]
- **Jenis usaha / layanan**: [Laundry]
- **Lokasi**: [Jl. Tegal Mulyo No.RT05 RW06, Tamanan, Kec. Banguntapan, Kab. Bantul, Daerah Istimewa Yogyakarta 55191]
- **Deskripsi singkat operasional**: [Laundry yang beroperasi setiap hari mulai pukul 07.00-21.00 WIB. Dengan kegiatan operasianal yang dilakukan oleh pemilik laundry, mulai dari penerimaan pesanan, pencatatan transaksi, proses pencucian, dan pengelolaan pembayaran.]
- **Narahubung / pemilik**: [Rezza Rahayu (pemilik), 082317480455]

## 2. Deskripsi Masalah Utama

- **Masalah utama**: [Pencatatan transaksi masih dilakukan secara manual menggunakan buku dan kertas nota. Dengan pencatatan stock yang masih belum terstruktur untuk memantau persediaan, sehingga pembelian barang dilakukan ketika pemilik melihat persediaan menipis atau sudah habis. Sistem pencarian data pelanggan masih dilakukan secara manual, yaitu dengan menelusuri buku catatan untuk memastikan status pembayaran pelanggan saat mengambil pesanan. Di sisi lain, pemilik juga hanya melakukan rekapitulasi pengeluaran rutin setiap minggu tanpa melakukan rekapitulasi transaksi secara rutin. Karena masih terdapat pelanggan yang belum melunasi pembayaran.]

- **Pihak yang terdampak**: [Pemilik laundry, karena ia harus melakukan proses transaksi secara manual dan menelusuri buku catatan untuk memastikan status pembayaran pelanggan yang mengambil laundry.]
- **Frekuensi / keparahan**: [Terjadi secara berkala, frekuensi kesalahan pencatatan atau koreksi (seperti lupa mencatat item tambahan seperti selimut/sprei atau kesalahan hitung manual) terjadi sekitar 1–2 kali dalam sebulan. Hal ini membuat pemilik memerlukan waktu untuk melakukan konfirmasi ulang dengan pelanggan.]

## 3. Batasan Sistem (Scope)

- **Diselesaikan dalam proyek ini**: [Pencatatan transaksi pelanggan, pencatatan status pembayaran, pencarian data transaksi, dan ringkasan rekapitulasi mingguan.]
- **Tidak diselesaikan (dan alasan)**: [Integrasi gateway pembayaran e-wallet / QRIS otomatis, rekapitulasi pengeluaran, pemesanan stok otomatis. karena, keterbatasan waktu 1 semester & kompleksitas API luar di PBL Level 1, rekapitulasi pengeluaran tidak dilakukan karena focus utama pada pencatatan transaksi, juga karena rekapitulasi pengeluaran membutuhkan data yang berbeda dari pencatatan transaksi, dan pembelian stock  masih dilakukan ketika diketahui menipis atau habis, juga karena belum ada pencatatan stock yang terstruktur.]

- **Asumsi yang dipakai**: [Sistem pencatatan dan pencarian transaksi akan digunakan oleh pemilik Rizky Laundry untuk membantu mencatat data pelanggan, memeriksa status pembayaran, dan membuat rekap transaksi. Data transaksi dimasukkan secara manual oleh pemilik.]


## 4. Data Kuantitatif Pendukung

| Indikator | Nilai/Baseline | Sumber Data | Tanggal |
|---|---|---|---|
| [waktu layanan rata-rata] | [2 menit/pelanggan] | [pemilik laundry (wawancara 1)] | [07/10/2026] |
| [jumlah transaksi per hari] | [4-7 orang] | [pemilik laundry (wawancara 1)] | [07/10/2026] |
| [frekuensi kesalahan pencatatn/selisih] |[1-2 kali/bulan] |[pemilik laundry (wawancara 1)] | [07/10/2026] |

## 5. Pernyataan Kebutuhan Awal (ringkasan ke D2)

- Kebutuhan inti yang akan dijawab prototipe:
 [1. Pencatatan Transaksi: Input data terstruktur yang mencakup nama, nomor telepon, paket, berat, dan status pembayaran, dilengkapi kalkulator otomatis untuk menghitung total harga.
2. Pencarian dan Pembaruan Status: Mencari data pesanan berdasarkan nama atau nomor telepon untuk melihat sekaligus memperbarui status pembayaran.
3. Rekapitulasi Periode: Menampilkan rekapitulasi total transaksi atau pendapatan dalam rentang waktu tertentu sesuai kebutuhan pemilik.]
  

## 6. Daftar Rujukan / Bukti

- [Observasi lapangan tanggal: 07/10/2026]
- [Wawancara pemilik tanggal: 07/10/2026]
- [Dokumen pendukung lainnya: ]

---

**Status**: ⬜ Draf → ⬜ Review Tim → ⬜ Validasi Pemilik → ⬜ Final (Gate 1)
