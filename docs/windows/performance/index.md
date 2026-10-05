# Membuat Windows 11 Lebih Lancar

Jika komputer Windows 11 terasa lambat, lakukan pemeriksaan berikut secara berurutan. Setelah kinerja sudah membaik, Anda tidak perlu meneruskan ke langkah berikutnya. Nama menu dapat sedikit berbeda tergantung versi Windows dan bahasa sistem.

<div class="image-card">
    <img src="../../assets/Knowledgebase%20IT/upload/Panduan%20Windows%2011%20Lebih%20Lancar.png" alt="Panduan meningkatkan kinerja Windows 11 dengan mengatur aplikasi startup, memeriksa proses, mengosongkan penyimpanan, memperbarui Windows dan driver, menyesuaikan efek visual, memindai keamanan, mengoptimalkan drive, dan memeriksa kebutuhan perangkat keras" width="100%">
</div>

## 1. Nonaktifkan aplikasi startup yang tidak diperlukan

Aplikasi yang berjalan otomatis saat masuk Windows dapat memperlambat proses startup dan memakai memori.

1. Tekan **Ctrl + Shift + Esc** untuk membuka **Task Manager / Pengelola Tugas**.
2. Pilih **Startup apps / Aplikasi startup**. Pada beberapa versi, namanya **Startup**.
3. Tinjau kolom **Startup impact / Dampak startup** dan nama aplikasinya.
4. Klik kanan aplikasi yang Anda kenali dan tidak perlu langsung berjalan saat komputer dinyalakan, lalu pilih **Disable / Nonaktifkan**.
5. Jangan nonaktifkan aplikasi keamanan, driver, sinkronisasi, atau aplikasi sekolah yang tidak Anda kenali. Jika ragu, biarkan aktif dan tanyakan kepada tim IT.
6. Mulai ulang komputer dan lihat apakah waktu startup membaik.

Menonaktifkan startup tidak menghapus aplikasi. Anda tetap dapat membukanya secara manual saat diperlukan.

## 2. Periksa proses yang memakai CPU dan memori

1. Tekan **Ctrl + Shift + Esc** untuk membuka **Task Manager**.
2. Pada tab **Processes / Proses**, klik judul kolom **CPU**, **Memory / Memori**, atau **Disk** untuk mengurutkan penggunaan tertinggi.
3. Tunggu beberapa saat dan periksa apakah penggunaan tinggi tetap terjadi.
4. Jika aplikasi yang Anda buka sendiri tidak merespons, pilih aplikasi itu lalu **End task / Akhiri tugas**. Simpan pekerjaan terlebih dahulu bila masih memungkinkan.
5. Jangan akhiri proses Windows, proses keamanan, atau proses yang tidak diketahui. Penggunaan tinggi sesaat saat pembaruan, pemindaian, atau membuka aplikasi besar dapat normal.
6. Buka tab **Performance / Kinerja** untuk melihat penggunaan CPU, memori, disk, dan jaringan.

Jika satu proses yang tidak dikenal terus memakai sumber daya tinggi, catat nama prosesnya dan hubungi tim IT sebelum menghapus file atau menghentikan layanan.

## 3. Kosongkan ruang penyimpanan dengan aman

1. Buka **Settings / Pengaturan > System / Sistem > Storage / Penyimpanan**.
2. Tunggu Windows menghitung penggunaan ruang.
3. Buka **Temporary files / File sementara** dan tinjau kategori yang ditawarkan.
4. Pilih hanya kategori yang dipahami dan tidak berisi file yang masih diperlukan, lalu tekan **Remove files / Hapus file**.
5. Periksa folder **Downloads / Unduhan** secara terpisah sebelum menghapus apa pun. Jangan memilih atau menghapus file pribadi yang belum dicadangkan.
6. Aktifkan **Storage Sense / Sensor Penyimpanan** hanya jika Anda memahami pengaturannya; tinjau aturan penghapusan file sementara dan Recycle Bin terlebih dahulu.
7. Hapus aplikasi yang tidak digunakan melalui **Settings > Apps > Installed apps / Aplikasi terinstal** hanya jika Anda mengenali aplikasi tersebut dan berwenang menghapusnya.

Jangan menghapus folder Windows, file sistem, atau data kerja sekolah untuk membebaskan ruang. Jika ruang hampir habis tetapi kategori file tidak jelas, minta bantuan tim IT.

## 4. Pasang pembaruan Windows dan driver yang sesuai

1. Sambungkan komputer ke daya dan jaringan yang stabil. Simpan pekerjaan yang terbuka.
2. Buka **Settings > Windows Update**, pilih **Check for updates / Periksa pembaruan**, lalu pasang pembaruan yang tersedia.
3. Mulai ulang komputer jika diminta dan biarkan pembaruan selesai. Jangan matikan paksa selama proses berlangsung.
4. Untuk masalah yang terkait perangkat tertentu, buka **Windows Update > Advanced options > Optional updates > Driver updates** jika tersedia. Pasang hanya pembaruan yang cocok dengan perangkat.
5. Jika pembaruan driver diperlukan tetapi tidak ditawarkan Windows Update, gunakan driver yang sesuai dengan model komputer dari situs resmi produsen atau minta tim IT memasangnya.
6. Uji kembali kinerja setelah komputer selesai memperbarui dan memulai ulang.

Jangan gunakan aplikasi pembaru driver pihak ketiga atau memasang driver untuk model perangkat yang berbeda. Pembaruan besar dapat berjalan di latar belakang dan sementara membuat komputer lebih lambat.

## 5. Kurangi efek visual jika komputer masih lambat

1. Tekan **Windows + R**, ketik `sysdm.cpl`, lalu tekan **Enter**.
2. Buka tab **Advanced / Tingkat Lanjut**.
3. Pada bagian **Performance / Kinerja**, pilih **Settings / Pengaturan**.
4. Di tab **Visual Effects / Efek Visual**, pilih **Adjust for best performance / Sesuaikan untuk kinerja terbaik**.
5. Pilih **Apply / Terapkan**, lalu **OK**.
6. Jika tampilan menjadi terlalu sederhana, pilih **Let Windows choose what's best for my computer / Biarkan Windows memilih pengaturan terbaik** untuk mengembalikan pengaturan otomatis.

Pilihan kinerja terbaik dapat mengurangi animasi dan efek tampilan. Pengaturan ini tidak menambah kemampuan perangkat keras; kembalikan pengaturan sebelumnya jika mengganggu penggunaan.

## 6. Jalankan pemindaian keamanan

1. Buka **Start / Mulai**, cari **Windows Security / Keamanan Windows**, lalu buka.
2. Pilih **Virus & threat protection / Perlindungan virus & ancaman**.
3. Pilih **Quick scan / Pemindaian cepat** untuk pemeriksaan awal.
4. Jika ada indikasi malware atau pemindaian cepat tidak menyelesaikan masalah, pilih **Scan options / Opsi pemindaian > Full scan / Pemindaian penuh > Scan now / Pindai sekarang**.
5. Biarkan pemindaian selesai dan ikuti tindakan yang direkomendasikan Windows Security.

Pemindaian penuh dapat memerlukan waktu dan sementara memakai sumber daya komputer. Jangan menonaktifkan antivirus untuk mempercepat komputer. Jika perangkat memakai antivirus yang dikelola sekolah, ikuti kebijakan IT.

## 7. Optimalkan drive

1. Buka Start dan cari **Defragment and Optimize Drives / Defragmentasi dan Optimalkan Drive**.
2. Pilih drive yang ingin diperiksa, lalu tekan **Analyze / Analisis** jika tersedia.
3. Pilih **Optimize / Optimalkan**. Windows akan menjalankan tindakan yang sesuai dengan jenis drive; SSD tidak perlu didefragmentasi secara manual dengan aplikasi pihak ketiga.
4. Tunggu proses selesai. Jangan matikan komputer selama optimasi berjalan.
5. Biarkan optimasi terjadwal Windows aktif kecuali tim IT memberi arahan lain.

Jika drive menunjukkan kesalahan, mengeluarkan bunyi tidak biasa, atau file menghilang, hentikan optimasi dan hubungi tim IT agar data diperiksa terlebih dahulu.

## 8. Pertimbangkan peningkatan perangkat keras

Jika komputer tetap lambat setelah langkah di atas, kebutuhan perangkat keras mungkin tidak lagi sesuai dengan beban kerja.

- **RAM:** penambahan memori dapat membantu jika penggunaan memori sering mendekati kapasitas penuh. Pastikan jenis dan kapasitas RAM kompatibel dengan model komputer.
- **HDD ke SSD:** SSD dapat mengurangi waktu boot dan membuka aplikasi dibandingkan HDD, tetapi harus kompatibel dan pemasangannya mungkin memerlukan pemindahan atau instalasi ulang sistem.
- **Ruang kosong:** usahakan tetap tersedia ruang kosong yang memadai agar Windows dan aplikasi dapat bekerja normal.

Kompatibilitas, garansi, lisensi, enkripsi, dan pencadangan harus diperiksa sebelum mengganti komponen. Jangan membuka perangkat atau membeli komponen untuk komputer sekolah tanpa persetujuan tim IT.

## Jalankan perbaikan file sistem jika Windows masih bermasalah

Gunakan perintah berikut jika Windows mengalami kesalahan sistem atau kerusakan file, bukan sebagai langkah rutin untuk setiap komputer yang terasa lambat. Simpan pekerjaan sebelum mulai.

1. Klik kanan **Start / Mulai**, lalu pilih **Terminal (Admin)** atau **Command Prompt (Admin)**.
2. Setujui permintaan **User Account Control / Kontrol Akun Pengguna** jika Anda berwenang. Jika meminta kredensial administrator yang tidak Anda miliki, berhenti dan hubungi tim IT.
3. Jalankan perintah DISM berikut dan tunggu sampai selesai:

   ```bat
   DISM /Online /Cleanup-Image /RestoreHealth
   ```

4. Setelah DISM selesai, jalankan pemeriksaan file sistem:

   ```bat
   sfc /scannow
   ```

5. Tunggu hingga verifikasi selesai. Jangan tutup jendela atau matikan komputer saat proses berjalan.
6. Mulai ulang Windows jika diminta, lalu periksa kembali apakah masalah teratasi.

DISM dapat memerlukan koneksi Windows Update dan kedua perintah ini bisa berjalan cukup lama. Jika muncul pesan kegagalan, catat pesan tersebut dan minta bantuan tim IT; jangan mengulang perbaikan berkali-kali tanpa pemeriksaan.

## Jika kinerja belum membaik

Mulai ulang komputer setelah pekerjaan tersimpan, lalu catat kondisi yang masih lambat—misalnya waktu startup, aplikasi tertentu, atau penggunaan CPU/memori/disk di Task Manager. Sampaikan hasil langkah yang sudah dilakukan kepada tim IT. Jika komputer sering mati sendiri, drive berbunyi tidak normal, atau muncul pesan kesalahan, hentikan penggunaan yang tidak penting dan minta pemeriksaan teknisi.
