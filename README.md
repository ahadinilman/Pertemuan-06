# Pertemuan 06 Nested Loop Python

Nama: Ahadin Ilman  
NIM: 2225250220  
Kelas: 3A 

## Tujuan
Menggunakan nested loop, pola, akumulasi, dan pencacahan.

## Cara Menjalankan
python3 tugas/tabel_perkalian_dan_statistik.py

## Algoritma Tugas 3
1. Membaca input n dan melakukan validasi menggunakan loop while sampai n > 0.
2. Inisialisasi variabel akumulator total_semua = 0 dan counter count_genap = 0.
3. Jalankan loop luar (i) dari 1 hingga n untuk merepresentasikan baris.
4. Di dalam loop luar, set total_baris = 0.
5. Jalankan loop dalam (j) dari 1 hingga n untuk merepresentasikan kolom.
6. Hitung hasil = i * j dan tampilkan nilainya.
7. Tambahkan hasil ke total_baris dan total_semua.
8. Cek apakah hasil modulo 2 sama dengan 0. Jika ya, tambahkan count_genap sebanyak 1.
9. Setelah loop dalam selesai, cetak total_baris.
10. Setelah loop luar selesai, cetak total_semua dan count_genap.

## Hasil Pengujian
| Input n | Hasil Diharapkan (Jumlah Pasangan, Total Semua, Genap) | Keluaran Aktual | Status |
| :---: | :---: | :---: | :---: |
| 1 | Pasangan: 1, Total: 1, Genap: 0 | Pasangan: 1, Total: 1, Genap: 0 | Sesuai |
| 2 | Pasangan: 4, Total: 9, Genap: 3 | Pasangan: 4, Total: 9, Genap: 3 | Sesuai |
| 3 | Pasangan: 9, Total: 36, Genap: 5 | Pasangan: 9, Total: 36, Genap: 5 | Sesuai |

## Analisis Efisiensi
Badan loop dalam dieksekusi sebanyak n x n (n^2) kali untuk input n. Hal ini terjadi karena untuk setiap 1 kali iterasi pada loop luar, loop dalam akan beriterasi sebanyak n kali.

## Refleksi
Kesalahan nested loop yang umum ditemukan adalah lupa mereset variabel akumulator baris di dalam loop luar. Jika total_baris diinisialisasi di luar kedua loop, nilainya akan terus terakumulasi dari baris-baris sebelumnya dan menghasilkan nilai total baris yang salah. Solusinya adalah meletakkan total_baris = 0 tepat di dalam loop luar sebelum loop dalam dimulai.