# Final-Project-Sistem-Operasi-Proyek-6-Kelompok-HDP-1
**PROYEK 6 | Implementasi Kontainerisasi Menggunakan Docker: Pembuatan Dockerfile, Manajemen Multikontainer dan Pembatasan Resource | Kelompok HDP1**
**Disusun Oleh Kelompok HDP 1**
1. Akbar Rizki Lingga [2401020003]
2. Al Adlhu Sodri Niwra [2401020015]
3. Muhammad Al-Fikry Akbar [2401020031]
4. Dzaky Ribal Faiz [2401020035]

**LATAR BELAKANG**
    Perkembangan teknologi komputasi modern menuntut aplikasi yang dapat
dijalankan secara konsisten pada berbagai lingkungan tanpa perlu konfigurasi ulang.
Perbedaan sistem operasi, versi library, dan dependency sering menyebabkan aplikasi
gagal berjalan atau menghasilkan perilaku berbeda antara satu mesin dengan mesin
lainnya (environment drift).
    Untuk mengatasi hal tersebut, digunakan konsep containerization, yaitu teknik
virtualisasi ringan yang memungkinkan aplikasi berjalan dalam lingkungan terisolasi
(isolated execution environment) tanpa memerlukan sistem operasi lengkap sebagaimana
pada virtual machine. Salah satu platform containerization paling banyak digunakan
adalah Docker.
    Docker menyediakan mekanisme untuk membangun image, yaitu paket berisi
aplikasi beserta dependensinya, dan menjalankannya sebagai container, yaitu instance
yang terisolasi dan ringan. Dalam konteks Sistem Operasi, Docker memanfaatkan fitur
kernel Linux seperti namespaces dan cgroups untuk menciptakan isolasi proses, file
system, networking, serta pembatasan penggunaan CPU dan memori.
    Proyek ini dirancang sebagai bentuk penerapan langsung konsep-konsep tersebut
melalui pembuatan Dockerfile, pembangunan image, menjalankan dua container, serta
menerapkan pembatasan resource menggunakan cgroups melalui Docker. Dengan
demikian, mahasiswa tidak hanya memahami teori, tetapi juga melakukan implementasi
nyata dari virtualisasi tingkat sistem operasi.

**METODOLOGI PROYEK
Gambaran Umum Proyek**

Proyek ini berfokus pada pembuatan lingkungan terisolasi berbasis container.
Mahasiswa akan membuat Dockerfile, membangun image, menjalankan dua container, serta
menerapkan batas resource CPU dan memori. Seluruh proses dilakukan berdasarkan konsep
virtualisasi tingkat sistem operasi.

**Arsitektur Sistem**
Arsitektur yang direncanakan mencakup komponen berikut:
1. Host Machine — perangkat fisik yang menjalankan Docker Engine.
2. Docker Engine — sistem utama yang mengelola image dan container.
3. Docker Image — blueprint aplikasi Python.
4. Container 1 — dibatasi CPU 0.5 core & memori 128 MB.
5. Container 2 — dibatasi CPU 1 core & memori 256 MB.
Arsitektur ini bersifat konseptual dan digunakan sebagai acuan implementasi pada laporan
akhir.

**Analisis Kebutuhan**
_Kebutuhan Perangkat Keras_
• CPU minimal dual-core
• RAM minimal 4 GB
• Ruang penyimpanan minimal 2 GB

_Kebutuhan Perangkat Lunak_
• Docker Desktop / Docker Engine
• Python 3
• Terminal / Command Prompt
• Text Editor (misalnya VS Code)

_Kebutuhan Fungsional_
• Sistem dapat membangun image dari Dockerfile.
• Sistem dapat menjalankan dua container secara bersamaan.
• Sistem dapat membatasi penggunaan CPU/memori container.
