# Materi 2 - Manajemen File dan Direktori di Linux

## Membuat File dan Direktori

| Perintah | Fungsi |
|:--:|:--:|
| touch `[nama_file]` | Membuat file kosong baru |
| mkdir `[nama_direktori]` | Membuat direktori baru |
| mkdir -p `[path/nama_direktori]` | Membuat direktori beserta parent-nya |

## Menghapus File dan Direktori

| Perintah | Fungsi |
|:--:|:--:|
| rm `[nama_file]` | Menghapus file |
| rm -i `[nama_file]` | Menghapus file dengan konfirmasi |
| rmdir `[nama_direktori]` | Menghapus direktori kosong |
| rm -r `[nama_direktori]` | Menghapus direktori berisi file |
| rm -rf `[nama_direktori]` | Menghapus direktori tanpa konfirmasi |

## Menyalin dan Memindahkan File dan Direktori

| Perintah | Fungsi |
|:--:|:--:|
| cp `[file_sumber]` `[file_tujuan]` | Menyalin file |
| cp -r `[direktori_sumber]` `[direktori_tujuan]` | Menyalin direktori dan isinya |
| mv `[file_sumber]` `[file_tujuan]` | Memindahkan/mengganti nama file |
| mv `[direktori_sumber]` `[direktori_tujuan]` | Memindahkan direktori |

## Utilitas Path

| Perintah | Fungsi |
|:--:|:--:|
| basename `[path/file]` | Nama file dari path |
| dirname `[path/file]` | Path direktori dari file |
