# Materi 4 - Perintah Dasar Linux - Pencarian File dan Direktori di Linux

## Pencarian Menggunakan `find`

| Perintah	| Fungsi | Contoh Penggunaan |
|:--:|:--:|:--:|
| find `[path]` -name `[nama_file]` | Mencari file berdasarkan nama | find /home -name dokumen.txt |
| find `[path]` -type d -name `[nama_direktori]` | Mencari direktori berdasarkan nama | find / -type d -name project |
| find `[path]` -type f -name "*.txt" | Mencari semua file dengan ekstensi tertentu | find /documents -type f -name "*.txt" |

## Opsi Tambahan `find`

| Opsi Tambahan | Fungsi | Contoh |
|:--:|:--:|:--:|
| -size | Mencari berdasarkan ukuran file | find / -size +100M (file > 100MB) |
| -mtime | Mencari berdasarkan waktu modifikasi | find / -mtime -7 (file dimodifikasi kurang dari 7 hari) |
| -user | Mencari file milik pengguna tertentu | find / -user username |

## Pencarian Cepat

| Perintah | Fungsi | Catatan |
|:--:|:--:|:--:|
| locate `[nama_file]` | Mencari file dengan database sistem | Gunakan `updatedb` untuk memperbarui database |

## Pencarian Perintah dan Lokasi

| Perintah | Fungsi | Contoh Keluaran |
|:--:|:--:|:--:|
| which `[perintah]` | Menampilkan path dari perintah yang dieksekusi | which ls → /bin/ls | 
| whereis `[perintah]` | Menampilkan lokasi biner, source code, dan manual dari perintah | whereis python → python: /usr/bin/python /usr/share/python /usr/share/man/man1/python.1.gz |

## Pencarian Teks dalam File

| Perintah | Fungsi | Contoh Penggunaan |
|:--:|:--:|:--:|
| grep "teks" `[nama_file]` | Mencari teks dalam file | grep "error" log.txt |

## Opsi Tambahan `grep`

| Opsi | Fungsi | Contoh |
|:--:|:--:|:--:|
| -i | Pencarian case-insensitive | grep -i "error" log.txt |
| -r | Pencarian rekursif dalam direktori | grep -r "error" /var/log/ |
| -n | Menampilkan nomor baris | grep -n "error" log.txt |
