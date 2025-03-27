# Materi 5 - Perintah Dasar Linux - Manajemen Proses

## Melihat Proses

| Perintah | Fungsi| Keterangan |
|:--:|:--:|:--:|
| ps aux | Menampilkan daftar proses yang berjalan | Menunjukkan semua proses dari semua pengguna |
| top | Menampilkan proses dan penggunaan CPU/memori secara real-time | Update berkelanjutan tentang kinerja sistem |
| htop | Versi interaktif dari top | Memerlukan instalasi tambahan, antarmuka lebih ramah pengguna |

## Menghentikan Proses

| Perintah | Fungsi| Keterangan |
|:--:|:--:|:--:|
| kill `[PID]` | Menghentikan proses berdasarkan PID | Mengirim sinyal standar untuk menutup proses |
| kill -9 `[PID]` | Memaksa menghentikan proses | Sinyal SIGKILL, digunakan jika proses tidak merespons perintah biasa |
| pkill `[nama_proses]` | Menghentikan proses berdasarkan nama | Berguna jika tidak mengetahui PID spesifik |

## Manajemen Pekerjaan Background

| Perintah | Fungsi| Keterangan |
|:--:|:--:|:--:|
| jobs | Menampilkan daftar pekerjaan di background | Menunjukkan pekerjaan yang sedang berjalan di terminal |
| bg `[job_id]` | Melanjutkan proses di background | Memindahkan proses yang dijeda ke background |
| fg `[job_id]` | Melanjutkan proses di foreground | Membawa proses background kembali ke foreground |
