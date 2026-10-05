# Memperbaiki Windows yang Terjebak Boot Loop

Jika komputer terus memulai ulang atau berhenti di logo Windows, ikuti langkah pemulihan berikut secara berurutan. Setelah Windows berhasil masuk ke desktop dan dapat digunakan normal, hentikan langkah berikutnya.

<div class="image-card">
    <img src="../../assets/Knowledgebase%20IT/upload/Panduan%20Memperbaiki%20Windows%20Boot%20Loop.png" alt="Panduan memperbaiki Windows boot loop melalui Windows Recovery Environment, Startup Repair, pemeriksaan driver, penghapusan update, System Restore, dan Reset Windows" width="100%">
</div>

## 1. Buka Windows Recovery Environment

1. Jika komputer sedang menyelesaikan pembaruan Windows atau pembaruan firmware/BIOS, jangan matikan paksa. Tunggu proses tersebut selesai.
2. Jika komputer benar-benar berhenti di logo atau terus memulai ulang, tahan tombol daya sampai komputer mati.
3. Nyalakan kembali komputer. Jika masalah tetap terjadi, ulangi proses mati dan nyala hingga total 2–3 kali. Jangan terus mengulanginya setelah itu.
4. Tunggu hingga layar **Preparing Automatic Repair** atau **Automatic Repair** muncul, lalu pilih **Advanced options / Opsi lanjutan**.
5. Pilih **Troubleshoot / Pemecahan masalah > Advanced options / Opsi lanjutan**.

Jika Windows Recovery Environment (WinRE) tidak terbuka, mulai komputer menggunakan media instalasi Windows, lalu pilih **Repair your computer / Perbaiki komputer Anda**—bukan **Install now / Instal sekarang**. Gunakan media instalasi Windows yang sesuai atau minta bantuan teknisi.

## 2. Jalankan Startup Repair

1. Dari **Troubleshoot > Advanced options**, pilih **Startup Repair / Perbaikan Startup**.
2. Pilih instalasi Windows jika diminta, lalu masukkan kata sandi akun jika diminta.
3. Tunggu pemeriksaan dan perbaikan selesai. Komputer dapat memulai ulang selama proses ini.
4. Jika Windows berhasil masuk ke desktop, masalah selesai. Jika tidak, buka kembali **Advanced options** dan lanjutkan ke langkah berikutnya.

## 3. Periksa file sistem dengan Command Prompt

1. Dari **Troubleshoot > Advanced options**, pilih **Command Prompt / Prompt Perintah**. Masuk ke akun jika diminta.
2. Temukan huruf drive tempat Windows terpasang. Huruf drive di WinRE dapat berbeda dari huruf yang biasa terlihat di Windows. Periksa satu per satu, misalnya:

   ```bat
   dir C:\Windows
   dir D:\Windows
   dir E:\Windows
   ```

   Gunakan drive yang menampilkan isi folder Windows. Contoh di bawah memakai `D:`; ganti dengan huruf drive yang ditemukan.

3. Jalankan pemeriksaan file sistem Windows secara luring:

   ```bat
   sfc /scannow /offbootdir=D:\ /offwindir=D:\Windows
   ```

4. Tunggu sampai pemindaian selesai, lalu catat pesan hasilnya.
5. Ketik `exit` untuk menutup Command Prompt, mulai ulang komputer, dan periksa apakah Windows dapat masuk.

Jika SFC menyatakan tidak dapat melakukan operasi yang diminta, pastikan huruf drive dan lokasi folder Windows sudah benar. Jangan menjalankan perintah dengan huruf drive contoh jika instalasi Windows berada di drive lain.

## 4. Periksa driver melalui Safe Mode

Lakukan langkah ini jika boot loop mulai terjadi setelah driver diperbarui atau jika langkah pemulihan sebelumnya belum menyelesaikannya.

1. Dari **Troubleshoot > Advanced options**, pilih **Startup Settings / Pengaturan Startup**, lalu pilih **Restart / Mulai ulang**.
2. Setelah daftar pilihan muncul, tekan **4** atau **F4** untuk masuk ke **Safe Mode / Mode Aman**. Jika membutuhkan jaringan untuk mendapatkan driver, tekan **5** atau **F5**.
3. Setelah Windows masuk, tekan **Windows + X**, lalu buka **Device Manager / Pengelola Perangkat**.
4. Buka **Display adapters / Display adapter**, klik kanan adaptor grafis, lalu pilih **Update driver / Perbarui driver**. Gunakan Windows Update atau driver yang sesuai dengan model komputer dari situs resmi produsennya.
5. Jika masalah dimulai tepat setelah pembaruan driver dan tersedia, buka **Properties / Properti > Driver > Roll Back Driver / Kembalikan Driver** untuk mengembalikan versi sebelumnya.
6. Mulai ulang komputer secara normal. Jika tidak dapat masuk ke Safe Mode, lanjutkan ke langkah berikutnya.

Jangan menghapus atau menonaktifkan adaptor grafis sebagai percobaan. Jika menu meminta hak administrator pada komputer yang dikelola sekolah, hentikan langkah ini dan minta tim IT melakukannya.

## 5. Hapus pembaruan terbaru atau gunakan System Restore

Jika boot loop dimulai setelah pembaruan Windows, hapus pembaruan terbaru dari WinRE:

1. Buka **Troubleshoot > Advanced options > Uninstall Updates / Hapus Pembaruan**.
2. Pilih **Uninstall latest quality update / Hapus pembaruan kualitas terbaru** terlebih dahulu.
3. Ikuti instruksi di layar, mulai ulang komputer, dan periksa apakah Windows dapat masuk.
4. Jika masalah tetap terjadi dan baru dimulai setelah pembaruan versi Windows, buka kembali menu tersebut dan pilih **Uninstall latest feature update / Hapus pembaruan fitur terbaru**, jika tersedia.

Jika pembaruan bukan penyebabnya atau penghapusannya tidak menyelesaikan masalah, gunakan titik pemulihan yang tersedia:

1. Buka **Troubleshoot > Advanced options > System Restore / Pemulihan Sistem**.
2. Pilih akun dan titik pemulihan bertanggal sebelum boot loop dimulai.
3. Tinjau perubahan yang akan dilakukan, lalu konfirmasikan pemulihan.
4. Setelah proses selesai, mulai ulang komputer.

System Restore dapat menghapus aplikasi, driver, atau pembaruan yang dipasang setelah tanggal titik pemulihan. Jika tidak ada titik pemulihan yang tersedia, lanjutkan ke langkah terakhir.

## 6. Reset Windows sebagai langkah terakhir

Reset dapat menghapus aplikasi dan pengaturan. **Remove everything / Hapus semuanya** menghapus file pribadi dari komputer. Pastikan file penting sudah dicadangkan sebelum melanjutkan jika masih memungkinkan.

1. Dari WinRE, pilih **Troubleshoot > Reset this PC / Reset PC ini**.
2. Pilih **Keep my files / Simpan file saya** untuk mencoba mempertahankan file pribadi. Aplikasi dan pengaturan tetap akan dihapus, dan pilihan ini bukan pengganti cadangan.
3. Pilih **Remove everything / Hapus semuanya** hanya jika memang ingin menghapus file pribadi serta aplikasi dan pengaturan.
4. Ikuti instruksi di layar sampai reset selesai. Jangan matikan komputer selama proses berlangsung.

Jika diminta kunci pemulihan BitLocker, masukkan kunci yang sesuai. Jika kunci tidak tersedia, data perlu diselamatkan, atau opsi reset gagal, hentikan proses dan hubungi tim IT/teknisi sebelum menginstal ulang Windows.
