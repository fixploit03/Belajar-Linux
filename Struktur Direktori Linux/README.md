# Materi 3 - Struktur Direktori Linux

## Konsep Dasar Hierarki Sistem File

Linux menggunakan sistem hierarki direktori yang terstandarisasi, yang dikenal sebagai Filesystem Hierarchy Standard (FHS). Struktur ini memungkinkan organisasi yang konsisten dan terstruktur dari seluruh sistem file.

## Direktori Utama di Root (`/`)

| Direktori | Fungsi | Contoh Isi |
|:--:|:--:|:--:|
| `/` | Direktori root atau akar, titik awal dari seluruh hierarki file sistem | Root dari semua direktori |
| `/bin` | Berisi perintah-perintah dasar yang diperlukan untuk mode pengguna tunggal | `ls`, `cp`, `mv`, `rm` |
| `/boot` | File-file yang diperlukan untuk proses boot sistem | `vmlinuz` (kernel), `initrd` |
| `/dev` | File perangkat (device files) | `sda` (hardisk), `tty` (terminal) |
| `/etc` | File konfigurasi sistem | `passwd`, `fstab`, `sudoers` |
| `/home` | Direktori home untuk pengguna | Folder personal pengguna |
| `/lib` | Pustaka sistem yang diperlukan oleh perintah di `/bin` dan `/sbin` | File `.so` (shared libraries) |
| `/media` | Titik mounting untuk perangkat media yang dapat dipindah | CD-ROM, Flashdisk |
| `/mnt` | Titik mounting sementara | Mounting manual |
| `/opt` | Paket perangkat lunak opsional | Software tambahan |
| `/proc` | Sistem file virtual yang menyediakan informasi proses | Informasi sistem runtime |
| `/root` | Direktori home untuk pengguna root | File pribadi root |
| `/sbin` | Perintah sistem untuk administrator | `fdisk`, `mkfs`, `shutdown` | 
| `/tmp` | File sementara | File yang dibuat aplikasi sementara |
| `/usr` | Hierarki sekunder untuk data pengguna | Program dan data pengguna |
| `/var` | File variabel seperti log, database sementara | Log sistem, spool file |

## Penjelasan Detail Direktori Penting

## `/etc` - Konfigurasi Sistem

- Berisi file konfigurasi sistem
- Contoh file penting:
  - `passwd`: Informasi pengguna
  - `shadow`: Password terenkripsi
  - `fstab`: Konfigurasi mounting filesystem
  - `sudoers`: Pengaturan hak akses sudo
 
## `/home` - Direktori Pengguna

- Setiap pengguna memiliki subdirektori tersendiri
- Contoh: `/home/username`
- Berisi:
  - Dokumen pribadi
  - Pengaturan aplikasi
  - File multimedia
 
## `/var` - File Variabel

- Log sistem
- Spool file
- File sementara yang sering berubah
- Contoh:
  - `/var/log`: Direktori log sistem
  - `/var/cache`: File cache
  - `/var/tmp`: File sementara

## `/usr` - Program Pengguna

- Mayoritas perangkat lunak yang diinstal
- Subdirektori penting:
  - /usr/bin: Perintah non-kritis
  - /usr/sbin: Perintah administrasi
  - /usr/lib: Pustaka tambahan

## Contoh Struktur Direktori Lengkap

```
/
├── bin       # Perintah dasar
├── boot      # File boot
├── dev       # File perangkat
├── etc       # Konfigurasi
├── home      # Direktori pengguna
│   └── user1
│       ├── Documents
│       ├── Downloads
│       └── Pictures
├── lib       # Pustaka sistem
├── media     # Media yang dapat dipindah
├── mnt       # Mounting sementara
├── opt       # Perangkat lunak opsional
├── proc      # Informasi proses
├── root      # Home direktori root
├── sbin      # Perintah administrasi
├── tmp       # File sementara
├── usr       # Program pengguna
└── var       # File variabel
```

## Tips Penting

- Pahami fungsi setiap direktori
- Hindari memodifikasi direktori sistem tanpa alasan yang jelas
- Gunakan `/home` untuk menyimpan file pribadi
- Simpan file konfigurasi di `/etc`
- Gunakan `/tmp` untuk file sementara

## Catatan Keamanan

- Berhati-hati saat bekerja di direktori sistem
- Gunakan `sudo` dengan sangat hati-hati
- Selalu buat cadangan sebelum mengubah file sistem
- Hindari menghapus atau memodifikasi file di `/bin`, `/sbin`, `/lib`

## Kesimpulan

Memahami struktur direktori Linux adalah kunci untuk navigasi dan manajemen sistem dengan efektif. Setiap direktori memiliki fungsi spesifik yang penting untuk operasi sistem.
