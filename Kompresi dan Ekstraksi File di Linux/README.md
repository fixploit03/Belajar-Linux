# Materi 7 - Kompresi dan Ekstraksi File di Linux

## 1. TAR

#### Kompresi

| Perintah | Fungsi | Contoh |
|:--:|:--:|:--|
| tar -cvf arsip.tar `[file/direktori]` | Membuat arsip tar biasa | tar -cvf dokumen.tar /home/user/dokumen |
| tar -czvf arsip.tar.gz `[file/direktori]` | Membuat arsip tar terkompresi (gzip) | tar -czvf arsip.tar.gz /path/ke/folder |
| tar -cjvf arsip.tar.bz2 `[file/direktori]` | Membuat arsip tar terkompresi (bzip2) | tar -cjvf arsip.tar.bz2 /path/ke/folder |

#### Ekstraksi

| Perintah | Fungsi | Contoh |
|:--:|:--:|:--|
| tar -xvf arsip.tar | Mengekstrak arsip tar | tar -xvf dokumen.tar |
| tar -xzvf arsip.tar.gz | Mengekstrak arsip tar.gz | tar -xzvf arsip.tar.gz | 
| tar -xjvf arsip.tar.bz2 | Mengekstrak arsip tar.bz2 | tar -xjvf arsip.tar.bz2 |

## 2. ZIP

| Perintah | Fungsi | Contoh |
|:--:|:--:|:--|
| zip -r arsip.zip `[file/direktori]` | Membuat arsip zip | zip -r proyek.zip /home/user/proyek |
| zip -e arsip.zip `[file/direktori]` | Membuat arsip zip terenkripsi | zip -e rahasia.zip dokumen_rahasia.txt |

#### Ekstraksi

| Perintah | Fungsi | Contoh |
|:--:|:--:|:--|
| uzip arsip.zip | Mengekstrak arsip zip | unzip proyek.zip | 
| unzip -d `[direktori]` arsip.zip | Mengekstrak ke direktori tertentu | unzip -d /tujuan proyek.zip |

## 3. RAR

#### Kompresi

| Perintah | Fungsi | Contoh |
|:--:|:--:|:--|
| rar a arsip.rar `[file/direktori]` | Membuat arsip rar | rar a proyek.rar /home/user/proyek |
| rar a -r arsip.rar `[file/direktori]` | Membuat arsip rar rekursif | rar a -r proyek.rar /home/user/proyek | 
| rar a -p arsip.rar `[file/direktori]` | Membuat arsip rar terenkripsi | rar a -p rahasia.rar dokumen_rahasia.txt |

#### Ekstraksi

| Perintah | Fungsi | Contoh |
|:--:|:--:|:--|
| unrar x arsip.rar | Mengekstrak arsip rar | unrar x proyek.rar | 
| unrar x arsip.rar `[direktori]` | Mengekstrak ke direktori tertentu | unrar x proyek.rar /tujuan |

## 4. GZIP

#### Kompresi


| Perintah | Fungsi | Contoh |
|:--:|:--:|:--|
| gzip `[file]` | Mengompres file | gzip dokumen.txt |
| gzip -9 `[file]` | Mengompres dengan kompresi maksimal | gzip -9 dokumen.txt |

#### Ekstraksi

| Perintah | Fungsi | Contoh |
|:--:|:--:|:--|
| gunzip `[file.gz]` | Mengekstrak file gzip | gunzip dokumen.txt.gz |
| gzip -d `[file.gz]` | Dekompres file gzip | gzip -d dokumen.txt.gz |

## 5. BZIP2

#### Kompresi

| Perintah | Fungsi | Contoh |
|:--:|:--:|:--|
| bzip2 `[file]` | Mengompres file | bzip2 dokumen.txt | 
| bzip2 -9 `[file] | Mengompres dengan kompresi maksimal | bzip2 -9 dokumen.txt |

#### Ekstraksi

| Perintah | Fungsi | Contoh |
|:--:|:--:|:--|
| bunzip2 `[file.bz2]` | Mengekstrak file bzip2 | bunzip2 dokumen.txt.bz2 |
| bzip2 -d `[file.bz2]` | Dekompres file bzip2 | bzip2 -d dokumen.txt.bz2 |

## 6. 7ZIP

#### Kompresi

| Perintah | Fungsi | Contoh |
|:--:|:--:|:--|
| 7z a arsip.7z `[file/direktori]` | Membuat arsip 7z | 7z a proyek.7z /home/user/proyek |
| 7z a -t7z -mx=9 arsip.7z `[file/direktori]` | Membuat arsip 7z dengan kompresi maksimal | 7z a -t7z -mx=9 proyek.7z /home/user/proyek |

#### Ekstraksi

| Perintah | Fungsi | Contoh |
|:--:|:--:|:--|
| 7z x arsip.7z | Mengekstrak arsip 7z | 7z x proyek.7z |
| 7z x arsip.7z -o`[direktori]` | Mengekstrak ke direktori tertentu | 7z x proyek.7z -o/tujuan |
