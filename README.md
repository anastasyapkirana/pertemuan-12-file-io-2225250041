# Pertemuan 12 — File Input-Output dan Penanganan Error

## Identitas Mahasiswa

- **Nama:** Anastasya Putri Kirana
- **NIM:** 2225250041
- **Kelas:** 3A
- **Mata Kuliah:** Algoritma dan Pemrograman

## Tujuan

Mempelajari cara membaca dan menulis file menggunakan Python serta memahami penanganan error menggunakan `try-except`. Praktikum menggabungkan file I/O dengan pengolahan data numerik.

## Struktur Project

```text
pertemuan-12-file-io-2225250041/
├── README.md
├── .gitignore
├── data/
│   ├── catatan.txt
│   ├── nilai.txt
│   └── hasil_rekap.txt
├── latihan/
│   ├── 01_tulis_file.py
│   ├── 02_baca_file.py
│   ├── 03_append_file.py
│   ├── 04_proses_baris.py
│   ├── 05_file_not_found.py
│   └── 06_value_error.py
└── tugas/
    └── rekap_nilai_file.py
```

## Deskripsi Latihan

1. Menulis file menggunakan mode `w`.
2. Membaca file menggunakan mode `r`.
3. Menambahkan isi file menggunakan mode `a`.
4. Membaca dan memproses data per baris.
5. Menangani error `FileNotFoundError`.
6. Menangani error `ValueError` saat konversi input.

## Tugas — Rekap Nilai dari File

Program membaca data nilai mahasiswa dari `data/nilai.txt`, melewati baris kosong dan nilai yang tidak valid, kemudian menghitung statistik nilai.

Hasil rekap disimpan ke `data/hasil_rekap.txt`.

Fungsi utama:
- `baca_data(nama_file)`: membaca dan memvalidasi data.
- `tulis_rekap(nama_file, data)`: menghitung dan menyimpan hasil rekap.

## Cara Menjalankan

Gunakan terminal dari folder utama project:

```bash
py latihan/01_tulis_file.py
py latihan/02_baca_file.py
py latihan/03_append_file.py
py latihan/04_proses_baris.py
py latihan/05_file_not_found.py
py latihan/06_value_error.py
py tugas/rekap_nilai_file.py
```

## Hasil Pengujian

| Pengujian | Hasil |
|---|---|
| Data normal | Data valid berhasil diproses |
| File tidak ditemukan | Pesan FileNotFoundError ditampilkan |
| Nilai tidak valid | Baris A004,abc dilewati |
| Baris kosong | Baris kosong dilewati |
| Batas kelulusan 60 | Nilai 60 dihitung lulus |

Hasil rekap dengan data asli:

- Jumlah data valid: 5
- Rata-rata: 83.40
- Minimum: 74.00
- Maksimum: 92.00
- Jumlah lulus: 5

Pengujian tambahan dengan nilai A007 sebesar 60 menghasilkan 6 data valid, rata-rata 81.17, dan 6 mahasiswa lulus.

## Refleksi

Melalui praktikum ini, saya mempelajari penggunaan file untuk menyimpan dan membaca data secara permanen. Saya juga memahami perbedaan mode `r`, `w`, dan `a`, serta pentingnya penanganan error agar program tetap berjalan ketika menemukan file yang tidak tersedia atau data yang tidak valid.

## Referensi

- Bahan Ajar Algoritma dan Pemrograman — Pertemuan 12.
- Video tutorial pembelajaran
