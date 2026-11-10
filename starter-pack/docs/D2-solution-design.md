# D2 — System & Solution Design

**Project**: Digital Problem Framing Mini Project — [Rezza Laundry]
**Tim**: [Deva Nayla Maisya, Mutia Fatmawati, Farizhki, M. Faris Ilham, M. Zacky Alfattah] | **Tanggal**: [10/11/2026] | **Versi**: [v1.0]
**Template**: TPL-02

> **Petunjuk**: Hapus teks dalam `[...]` setelah diisi.
> Worksheet terkait: WS05, WS06, WS07

---

## 1. Daftar Kebutuhan (User Story)

| # | User Story | Prioritas |
|---|---|---|
| 1 | Sebagai [Pemilik Laundry], saya ingin [Saya ingin mencatat transaksi pelanggan dan menghitung secara secara otomatis.] sehingga [Sehingga pencatatan transaksi lebih terstruktur dan memudahkan dalam pencarian data.] | [Tinggi] |
| 2 | Sebagai [Pemilik Laundry], saya ingin [Mencari data transaksi pelanggan untuk memeriksa status pembayaran tanpa melihat buku besar secara manual.] sehingga [Sehingga saya dapat melihat status pembayaran pelanggan dengan lebih mudah dan cepat.] | [Sedang] |
| 3 | Sebagai [Pemilik Laundry], saya ingin [Saya ingin melihat rekapitulasi transaksi dalam bentuk spreadsheet] sehingga [Tidak perlu menghitung nota fisik dan catatan di buku besar secara manual.] | [Sedang] |

## 2. Kriteria Penerimaan

| # | Kriteria Penerimaan (terukur & dapat diuji) |
|---|---|
| 1 | [Sistem berhasil menyimpan data pesanan baru ke dalam basis data (database/file) dan menampilkannya di riwayat transaksi.] |
| 2 | [Sistem menampilkan total harga dengan tingkat akurasi 100% (Berat cucian x Harga layanan per kg) dalam waktu kurang dari 2 detik.] |
| 3 | [Sistem dapat menghasilkan atau menampilkan struk rincian pesanan yang memuat ID Pesanan, Nama, dan Total Bayar setelah transaksi disimpan.] |

## 3. Success Metrics

| Metrik | Baseline (Sekarang) | Target | Cara Mengukur |
|---|---|---|---|
| [waktu pencatatan] | [120 detik (2 menit)] | [<70 detik] | [Stopwatch sampel 10 transaksi input pesanan] |
| [Durasi pencarian data transaksi & status pelanggan] | [30–60 detik / pencarian manual di buku besar] | [< 10 detik / pencarian] | [Uji coba pencarian data berdasarkan nama atau nomor telepon] |
| [Frekuensi kesalahan hitung nota & selisih tagihan] | [1–2 kali / bulan (kesalahan hitung manual)] | [0 kali / bulan (Akurasi 100%)] | [Audit verifikasi kesesuaian tarif dan kalkulasi otomatis sistem] |

## 4. Desain Solusi

### 4.1 Konsep Solusi (ringkasan)

_[Satu paragraf bagaimana prototipe menjawab masalah dari D1]_

### 4.2 Peta Komponen (IPO)

```
Input  ──▶  Proses  ──▶  Output
  │                           │
  └───── Data/Penyimpanan ────┘
```

- **Input**: [Nama Pelanggan, Nomor HP, Berat Cucian (Kg), Jenis Layanan (Cuci Komplit/Cuci Kering/Setrika).]
- **Proses**: [Sistem menerima input, mengalikan berat cucian dengan tarif layanan, menghasilkan ID Pesanan unik, dan memproses penyimpanan.]
- **Output**: [Struk detail/nota pesanan di layar dan rekapitulasi transaksi.]
- **Data/Penyimpanan**: [Data transaksi dan pelanggan disimpan ke dalam spreadsheet/JSON]

### 4.3 Flowchart & Pseudocode

_[Tempel flowchart di `assets/` dan tulis pseudocode di bawah]_

```
[PSEUDOCODE]
```

## 5. Hasil Validasi Pemilik Usaha

- **Tanggal validasi**: [DD/MM/YYYY]
- **Feedback pemilik**: [...]
- **Perubahan setelah validasi**: [...]

---

**Status**: ⬜ Draf → ⬜ Review Tim → ⬜ Validasi Pemilik → ⬜ Final (GATE 1)
