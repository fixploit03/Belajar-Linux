# Materi 4 - Perintah dasar Linux

## Menampilkan Informasi Direktori

| Perintah	| Fungsi |
|:--:|:--:|
| pwd	| Menampilkan jalur (path) direktori kerja saat ini |
| ls	| Menampilkan daftar isi direktori |
| ls -l	| Menampilkan isi direktori dalam format daftar detail |
| ls -a	| Menampilkan semua file, termasuk file tersembunyi |
| ls -lh | Menampilkan ukuran file dalam format yang mudah dibaca |

## Struktur Direktori Linux

```
/home/linux/documents
 └┬┘   └┬┘   └┬┘
  |     |     |
  |     |     Current Directory
  |     Parrent Directory
  Base Directory
```

#### Penjelasan Komponen:

1. **Base Directory** (`/home`)
   - Direktori dasar atau awal dari path
   - Titik awal hierarki direktori
   - Dalam contoh ini, /home adalah base directory

2. **Parent Directory** (`/home/linux`)
   - Direktori yang berisi direktori saat ini
   - Satu level di atas direktori saat ini
   - Dapat diakses menggunakan `..`

3. **Current Directory** (`/home/linux/documents`)
   - Direktori tempat Anda saat ini berada
   - Lokasi aktif dalam sistem file
   - Dapat dirujuk dengan `.`
     
## Berpindah Direktori

| Perintah	| Fungsi |
|:--:|:--:|
| cd `[nama_direktori]`	| Berpindah ke direktori tertentu | 
| cd ..	| Kembali ke direktori induk (parent directory) |
| cd ~	| Berpindah ke direktori home |
| cd /	| Berpindah ke direktori root |
| cd -	| Kembali ke direktori sebelumnya |
