NAMA  : Andi Daniella Mezauri <BR/>
NIM   : 09011282328083 <BR/>
KELAS : SK3B <BR/>
MK    : Sistem Operasi<BR/>
Tugas : 10 soal dari modul Praktikum 3<BR/>

# Laporan Praktikum Modul 3 (File System)
## BAB I PENDAHULUAN

### 1.1 LATAR BELAKANG
<p> Pada sistem operasi berbasis Unix/Linux, pengelolaan file dan direktori sangat penting untuk menjaga keamanan dan aksesibilitas data, terutama dalam lingkungan multi-user. Sistem ini memungkinkan administrator untuk mengatur hak akses file dan direktori, memastikan hanya pengguna tertentu yang dapat membaca, menulis, atau mengeksekusi file. Selain itu, konsep umask dan link juga menjadi kunci dalam mengatur izin default saat file baru dibuat dan menghubungkan file ke referensi lain, sehingga pengelolaan file menjadi lebih efisien dan aman. </p>

### 1.2 TUJUAN LAPRAK
-  Mengenal organisasi File di Linux <br/>
-  Menciptakan dan manipulasi direktori<br/>
-  Mempelajari ijin akses (permission) dari file dan direktori<br/>
-  Mengenal konsep Owner dan Group<br/>
-  Mengerti konsep Link dan symbolic link<br/>

### 1.3 ALAT DAN BAHAN
- Laptop
- Sistem operasi Linux (misalnya, Ubuntu)
- Command Line/Terminal

### 1.4 DASAR TEORI
- Pada sistem operasi Unix/Linux, terdapat banyak perintah dasar yang digunakan untuk mengelola file dan direktori. Berikut beberapa konsep penting yang dipelajari dalam praktikum ini:
- Peralatan I/O (Input/Output) adalah perangkat keras yang berinteraksi dengan komputer, misalnya keyboard, mouse, printer, dll. Character device merupakan salah satu tipe perangkat I/O yang mentransfer data satu karakter dalam satu waktu.
- Izin Akses File memungkinkan kita untuk mengontrol siapa yang dapat membaca, menulis, dan mengeksekusi file atau direktori. Izin akses ditetapkan untuk tiga kategori: owner (pemilik), group (kelompok), dan others (lainnya).
- Umask adalah nilai default yang digunakan sistem untuk menetapkan izin pada file baru. Umask menentukan hak akses apa yang dihapus ketika file atau direktori baru dibuat.
- Link merupakan cara untuk membuat referensi dari satu file ke file lain. Ada dua jenis link: hard link dan symbolic link. Hard link membuat referensi langsung ke data file, sementara symbolic link adalah rujukan ke nama file.

## BAB II LANGKAH KERJA
- [ Tugas dan Percobaan ]
### 2.1 Lihat peralatan I/O, character device, yang ada pada system komputer.
<img src="https://github.com/user-attachments/assets/942cb9fd-e95d-4284-8fd9-40a8bedfe3db" width=500/>
<img src="https://github.com/user-attachments/assets/fc9fda86-605a-4a94-9def-14ead9760a5b" width=500/>

### 2.2 Buatlah sub direktori januari, februari dan maret sekaligus pada direktori latihan5.
<img src="https://github.com/user-attachments/assets/11304422-bd84-488c-9767-f01367b4f557" width=500/>
<img src="https://github.com/user-attachments/assets/03b9981e-6dec-4189-aa19-03b3b08fc37e" width=500/>
<img src="https://github.com/user-attachments/assets/5ea3d192-8563-4d17-8d7a-473117d874e8" width=500/>

### 2.3 Buatlah file dataku yang berisi nama, nim dan alamat anda pada sub direktori januari dan copy-kan file tersebut ke sub direktori februari dan maret.
<img src="https://github.com/user-attachments/assets/a8bdafa0-45d3-4ce2-a6cc-a80e64e89dac" width=500/>
<img src="https://github.com/user-attachments/assets/7c196107-c710-418b-9c46-16a5125c3b9e" width=500/>
<img src="https://github.com/user-attachments/assets/1fc57214-c5af-486c-bac7-301b8e7abffc" width=500/>
<img src="https://github.com/user-attachments/assets/9116f3c8-53ba-4ce2-a84e-2e6e2446f7bf" width=500/>
<img src="https://github.com/user-attachments/assets/412e9401-ecd3-4280-bce6-fbd4c366e47a" width=500/>

### 2.4 Ubahlah ijin akses file dataku pada sub direktori januari sehingga group dan others dapat melakukan write.
<img src="https://github.com/user-attachments/assets/fed1ff85-c1c3-43f6-9782-3499e9d36055" width=500/>
<img src="https://github.com/user-attachments/assets/e1031e77-54ca-492f-aa6d-7f3381c35f6a" width=500/>

### 2.5 Ubahlah ijin akses file dataku pada sub direktori februari sehingga user dapat melakukan baik write, read maupun execute, tetapi group dan others hanya bisa read dan execute.
<img src="https://github.com/user-attachments/assets/8b96f29a-951d-4e7d-9491-620a3e492289" width=500/>
<img src="https://github.com/user-attachments/assets/24c9db2d-117b-4f77-a809-439bfa5f75cd" width=500/>

### 2.6 Ubahlah ijin akses file dataku pada sub direktori maret sehingga semua dapat melakukan write, read dan execute.
<img src="https://github.com/user-attachments/assets/53b23401-7793-4261-8383-3354fee1f8f4" width=500/>

### 2.7 Hapuslah direktori maret.
<img src="https://github.com/user-attachments/assets/9e302b45-a635-402e-8725-879c7fe9693c" width=500/>
<img src="https://github.com/user-attachments/assets/f9d2b906-5019-4272-8541-3e07d8308663" width=500/>

### 2.8 Ubahkan kepemilikan sub direktori februari sehingga user dan group hanya dapat melakukan read, dan cobalah untuk membuat direktori baru haha pada sub direktori februari.
<img src="https://github.com/user-attachments/assets/61081ce4-e14c-469a-995e-266a187683f6" width=500/>
<img src="https://github.com/user-attachments/assets/35511623-4544-4a52-9df2-ed6a4afc7b8b" width=500/>
<img src="https://github.com/user-attachments/assets/92bc849a-99c4-4ae4-8008-5fd502153532" width=500/>
<img src="https://github.com/user-attachments/assets/5994c09b-06b2-4ff3-84dd-34f68346f647" width=500/>
<img src="https://github.com/user-attachments/assets/b26545d3-cf38-4196-9d7f-239bef8ee43d" width=500/>

### 2.9 Modifikasi umask dari file dataku pada sub direktori januari menjadi 027 dan berapakan nilai default-nya. 
<img src="https://github.com/user-attachments/assets/52d10d4e-d586-434d-968d-1bc215131781" width=500/>

### 2.10 Buatlah link dari file dataku ke file dataku.ini dan file dataku.juga dan dengan perintah list perhatikan berapa link yang terjadi ?
<img src="https://github.com/user-attachments/assets/7f08724d-ed6f-420e-9c29-8419e735eab2" width=500/>
<img src="https://github.com/user-attachments/assets/de92e60c-4aff-4372-b1fc-8c3c784d64c6" width=500/>
<img src="https://github.com/user-attachments/assets/cac8a27c-712e-450d-a1e6-ab2b9e8ff8c1" width=500/>

## BAB III PENUTUP
### 3.1 KESIMPULAN
1. Izin akses file sangat penting dalam mengelola hak akses user, group, dan others di sistem Unix/Linux.
2. Umask mengontrol izin default saat file baru dibuat.
3. Hard link memungkinkan file yang sama untuk diakses melalui nama file yang berbeda.
4. Perintah chmod, umask, dan ln sangat berguna dalam mengelola izin akses dan link di sistem Unix/Linux.


