PROGRAM KasirLaundry

START

REPEAT

Menampilkan menu (1-3)

INPUT Pilihan

IF Pilihan == 1 THEN

CALL Proses_Menu_1

ELSE IF pilihan == 2 THEN

CALL Proses_Menu_2

ELSE IF pilihan == 3 THEN

CALL Proses_Menu_3

END IF

UNTIL keluar

END

PROCEDURE Proses_Menu_1

Input nama

IF nama kosong? == "tidak" THEN

Print "Data belum lengkap, transaksi tidak dapat di simpan"

RETURN

END IF

// Cabang nama kosong? == "ya"

print & pilih paket

IF Pilihan valid? == "tidak" THEN

Print paket tidak valid batal

RETURN

END IF

// Cabang Pilihan valid? == "ya"

IF Ada Selimut? (y/n) THEN

jumlah kecil & besar

input jumlah selimut

END IF

input berat pakaian (kg)

hitung otomatis biaya paket, biaya berat

Print total tagihan

Input Pembayaran

IF Dibayar == total tagihan? == "ya" THEN

Status = Lunas

ELSE

Status = Belum lunas

END IF

Simpan data ke transaksi

Print nota

END PROCEDURE

PROCEDURE Proses_Menu_2

Input nama/no hp

IF Ditemukan? == "Ya" THEN

Print data transaksi

IF lunas? == "ya" THEN

keluar

ELSE

masukan nominal pembayaran

ubah status pembayaran menjadi lunas

END IF

ELSE

// Cabang Ditemukan? == "Tidak"

Print "data tidak ditemukan"

END IF

END PROCEDURE

PROCEDURE Proses_Menu_3

Pilih rekap: "1.Bulanan 2.Mingguan"

IF bulanan? == "Bulanan" THEN

Input bulan(YYYY-MM/1-12)

IF Valid? == "Ya" THEN

Tampilkan rekap bulan yang di input

ELSE

Print Tidak ada transaksi pada bulan ini

END IF

ELSE

// Cabang pilihan Mingguan

Input bulan(YYYY-MM/1-12)

Tampilkan minggu pada bulan yang di input

Input minggu yang dipilih

IF Valid? == "Ya" THEN

Tampilkan rekap minggu yang di input

ELSE

Print tidak ada transaksi pada minggu di bulan ini

END IF

END IF

END PROCEDURE