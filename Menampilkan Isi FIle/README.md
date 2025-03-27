# Materi 5 - Perintah dasar Linux-  Menampilkan Isi File

## Dasar

| Perintah | Fungsi | Contoh Penggunaan |
|:--:|:--:|:--:|
| cat `[nama_file]` | Menampilkan seluruh isi file | cat dokumen.txt |
| tac `[nama_file]` | Menampilkan isi file dari bawah ke atas | tac laporan.log |

## Dengan Navigasi

| Perintah	| Fungsi | Contoh Penggunaan |
|:--:|:--:|:--:|
| less `[nama_file]` | Menampilkan isi file dengan navigasi ke atas/bawah | less konfigurasi.conf |
| more `[nama_file]` | Menampilkan isi file dengan navigasi satu layar penuh | more README.md |

## Menampilkan Baris Tertentu Dari File

#### Baris Pertama

| Perintah	| Fungsi | Contoh Penggunaan |
|:--:|:--:|:--:|
| head `[nama_file]` | Menampilkan 10 baris pertama | head log_aktivitas.txt |
| head -n `[jumlah_baris]` `[nama_file]` | Menampilkan sejumlah baris pertama | head -n 5 script.py |

#### Baris Terakhir

| Perintah	| Fungsi | Contoh Penggunaan |
|:--:|:--:|:--:|
| tail `[nama_file]` | Menampilkan 10 baris terakhir | tail error.log |
| tail -n `[jumlah_baris]` `[nama_file]` | Menampilkan sejumlah baris terakhir | tail -n 3 catatan.txt |

## Fitur Khusus

| Perintah	| Fungsi | Keterangan |
|:--:|:--:|:--:|
| tail -f `[nama_file]` | Menampilkan isi file secara real-time | Sangat berguna untuk monitoring log |
