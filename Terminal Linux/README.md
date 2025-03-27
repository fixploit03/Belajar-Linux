# Materi 4 - Terminal Linux

## Apa itu Terminal Linux?

Terminal Linux adalah antarmuka baris perintah (Command Line Interface/CLI) yang memungkinkan pengguna berinteraksi langsung dengan sistem operasi menggunakan teks perintah. Ini adalah alat powerful untuk mengelola sistem, mengotomatisasi tugas, dan mengontrol komputer dengan lebih mendalam.

## Komponen Utama Terminal

1. **Shell**

- Definisi: Program yang menerjemahkan perintah pengguna
- Jenis Shell Umum:
  - Bash (Bourne Again Shell) - Default di mayoritas distro Linux
  - Zsh (Z Shell) - Shell dengan fitur canggih
  - Fish - Shell dengan fitur autosugest modern
  - Sh (Bourne Shell) - Shell paling dasar

2. **Prompt Terminal**
   
Struktur prompt biasanya:

```
[username@hostname ~]$
```

- `username`: Nama pengguna saat ini
- `hostname`: Nama komputer
- `~`: Direktori home pengguna
- `$`: Indikator akses pengguna biasa
- `#`: Indikator akses root/administrator

## Shortcut Keyboard Penting

#### Navigasi Teks

- `Ctrl + A`: Pindah ke awal baris
- `Ctrl + E`: Pindah ke akhir baris
- `Ctrl + U`: Hapus dari kursor ke awal baris
- `Ctrl + K`: Hapus dari kursor ke akhir baris
- `Ctrl + W`: Hapus satu kata sebelumnya

#### Riwayat Perintah

- `Panah Atas/Bawah`: Navigasi perintah sebelumnya
- `Ctrl + R`: Pencarian riwayat perintah
- `!!`: Jalankan perintah terakhir
- `!n`: Jalankan perintah ke-n di riwayat

#### Manajemen Proses

- `&`: Jalankan proses di background
- `Ctrl + Z`: Jeda proses
- `jobs`: Daftar proses background
- `fg`: Kembalikan proses ke foreground
- `Ctrl + C`: Hentikan proses saat ini

## Tips Produktivitas

1. Gunakan tab completion
2. Pelajari perintah `man` untuk dokumentasi
3. Gunakan `alias` untuk perintah yang sering dipakai
4. Simpan konfigurasi shell di `.bashrc` atau `.zshrc`

## Catatan Keamanan

- Selalu berhati-hati dengan perintah yang membutuhkan `sudo`
- Pahami konsekuensi setiap perintah
- Gunakan `--help` atau `man` untuk memahami perintah
