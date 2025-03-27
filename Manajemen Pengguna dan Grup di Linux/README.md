# Materi 9 - Manajemen Pengguna dan Grup di Linux

## Identifikasi Pengguna

| Perintah | Fungsi | Keterangan |
| :--:|:--:|:--|
| whoami | Menampilkan user yang sedang login | Menunjukkan nama pengguna aktif saat ini |
| id | Menampilkan UID dan GID user saat ini | Menampilkan ID pengguna dan grup | 
| who | Menampilkan daftar user yang login | Menunjukkan pengguna yang terhubung ke sistem |

## Manajemen Pengguna

| Perintah | Fungsi | Keterangan |
| :--:|:--:|:--|
| adduser `[nama_user]` | Menambahkan user baru | adduser john - Membuat pengguna baru |
| deluser `[nama_user]` | Menghapus user | deluser john - Menghapus pengguna |
| passwd `[nama_user]` | Mengubah password user | passwd john - Mengubah password untuk pengguna john |

## Manajemen Grup

| Perintah | Fungsi | Keterangan |
| :--:|:--:|:--|
| groupadd `[nama_grup]` | Menambahkan grup baru | groupadd developers - Membuat grup baru |
| usermod -aG `[nama_grup]` `[nama_user]` | Menambahkan user ke grup | usermod -aG developers john - Menambahkan john ke grup developers |
