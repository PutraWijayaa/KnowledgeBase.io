# Mengatasi BIOS Tidak Mendeteksi Hard Drive

Jika BIOS/UEFI tidak menampilkan HDD atau SSD, Windows tidak dapat menggunakan drive tersebut sebagai perangkat penyimpanan atau boot. Ikuti pemeriksaan berikut secara berurutan. Jika drive berisi data penting yang belum dicadangkan, batasi percobaan menyalakan komputer dan hubungi teknisi.

<div class="image-card">
    <img src="../../assets/Knowledgebase%20IT/upload/Panduan%20Mengatasi%20BIOS%20Tidak%20Mendeteksi%20Hard%20Drive.png" alt="Langkah mengatasi BIOS tidak mendeteksi hard drive dengan memeriksa kabel SATA dan daya, kondisi drive, port motherboard, pengaturan BIOS, dan versi BIOS" width="100%">
</div>

## 1. Pastikan drive memang tidak terdeteksi BIOS

1. Nyalakan komputer dan masuk ke BIOS/UEFI dengan menekan tombol yang ditampilkan saat mulai menyala. Tombol yang umum digunakan adalah **F2**, **Delete**, atau **F10**, bergantung pada perangkat.
2. Buka halaman **Storage**, **SATA Information**, **SATA Configuration**, atau menu sejenis.
3. Periksa apakah nama/model HDD atau SSD muncul pada daftar perangkat.
4. Jika drive muncul di BIOS tetapi tidak terlihat di File Explorer, jangan lakukan langkah bongkar kabel atau reset BIOS dari panduan ini. Masalahnya berbeda; hubungi tim IT untuk memeriksa Windows, partisi, atau status drive tanpa memformatnya.
5. Jika drive tidak muncul di BIOS, lanjutkan ke pemeriksaan koneksi.

Nama menu dan tampilan BIOS berbeda menurut merek dan model komputer.

## 2. Periksa kabel SATA dan kabel daya

Langkah ini hanya untuk **komputer desktop** yang boleh dibuka dan jika Anda berwenang. Untuk laptop, komputer sekolah yang masih bergaransi, atau perangkat yang tidak boleh dibongkar, minta teknisi melakukan pemeriksaan internal.

1. Matikan komputer sepenuhnya.
2. Cabut kabel listrik dari stopkontak. Pada desktop, pastikan daya benar-benar terputus sebelum menyentuh komponen di dalam casing.
3. Buka casing hanya jika Anda memiliki izin dan dapat melakukannya dengan aman. Jangan membuka power supply.
4. Periksa kabel data SATA dan kabel daya yang tersambung ke HDD/SSD. Pastikan konektornya terpasang rapat dan tidak terlihat rusak.
5. Jika konektor tampak baik, lepaskan lalu pasang kembali dengan hati-hati. Jangan menarik kabelnya, menekuk konektor, atau memaksa pemasangan.
6. Tutup casing, sambungkan kembali daya, lalu nyalakan komputer dan periksa daftar drive di BIOS.
7. Jika kabel terkelupas, konektor longgar, atau drive masih tidak terdeteksi, matikan komputer dan lanjutkan hanya jika tersedia kabel pengganti yang sesuai; jika tidak, hubungi teknisi.

## 3. Uji drive dan kabel satu per satu

Pengujian dengan komponen lain dapat membantu membedakan kerusakan drive, kabel, atau komputer. Lakukan hanya dengan perangkat yang kompatibel dan atas izin teknisi.

1. Coba kabel SATA data lain yang diketahui berfungsi, lalu periksa lagi BIOS.
2. Jika tidak berhasil, uji drive pada komputer lain atau sambungan kompatibel yang diketahui berfungsi.
3. Jika drive dikenali pada kabel/komputer lain, kemungkinan masalah berada pada kabel, port SATA, atau konfigurasi komputer awal.
4. Jika drive tidak dikenali di beberapa sambungan yang berfungsi, kemungkinan drive rusak. Hentikan percobaan berulang, terutama jika ada data penting, dan minta pemeriksaan profesional.

Jangan melakukan inisialisasi, format, atau proses pemulihan yang menulis ke drive jika data di dalamnya perlu diselamatkan.

## 4. Periksa port SATA motherboard

1. Matikan komputer dan cabut daya sebelum memindahkan konektor internal.
2. Jika Anda berwenang dan komponen desktop mudah dijangkau, pindahkan kabel data ke port SATA lain yang tersedia pada motherboard.
3. Nyalakan komputer dan periksa kembali BIOS.
4. Jika drive terdeteksi pada port lain, port sebelumnya atau konfigurasi port tersebut mungkin bermasalah.
5. Jika drive tetap tidak terdeteksi, kembalikan koneksi sesuai konfigurasi yang diketahui atau serahkan pemeriksaan kepada teknisi.

Jangan menyentuh pin, mengikis konektor, atau menggunakan port yang terlihat bengkok, kotor, atau rusak.

## 5. Periksa konfigurasi BIOS/UEFI

1. Di BIOS/UEFI, buka **SATA Configuration**, **Storage Configuration**, atau menu sejenis.
2. Pastikan port SATA tempat drive terhubung dalam keadaan **Enabled / Aktif** dan deteksi perangkat tidak dinonaktifkan.
3. Periksa mode SATA yang sedang digunakan, misalnya **AHCI**, **RAID**, atau konfigurasi lain. Catat pengaturan saat ini.
4. **Jangan mengubah mode AHCI/RAID/IDE sebagai percobaan.** Perubahan mode dapat membuat Windows gagal boot atau membuat drive tidak dapat diakses. Jika pengaturan tampak salah atau baru berubah, minta tim IT mengonfirmasi konfigurasi yang benar untuk perangkat tersebut.
5. Simpan hanya perubahan yang sudah dipastikan benar. Jika tidak yakin, keluar tanpa menyimpan perubahan.

## 6. Perbarui BIOS/UEFI hanya jika diperlukan

Pembaruan BIOS bukan langkah rutin untuk masalah deteksi drive dan pembaruan yang gagal dapat membuat komputer tidak dapat digunakan.

1. Catat model lengkap komputer atau motherboard serta versi BIOS/UEFI saat ini.
2. Periksa catatan rilis pada halaman dukungan **resmi** produsen untuk memastikan pembaruan memang menangani masalah kompatibilitas atau deteksi penyimpanan.
3. Jika komputer dikelola sekolah, minta tim IT melakukan pembaruan. Jangan menggunakan file BIOS untuk model yang berbeda.
4. Pembaruan harus mengikuti instruksi produsen dan dilakukan dengan daya yang stabil. Jangan matikan atau cabut daya selama proses berlangsung.
5. Setelah pembaruan selesai, periksa kembali apakah drive muncul di BIOS.

## Jika BIOS tetap tidak mendeteksi drive

Hentikan percobaan dan hubungi tim IT/teknisi jika drive tidak muncul setelah koneksi dan port diperiksa, terdengar bunyi klik atau gesekan, konektor terlihat rusak, atau ada data penting yang belum dicadangkan. Jangan format drive, menginisialisasi disk, membuka casing HDD/SSD, atau berulang kali menyalakan drive yang diduga rusak.

Saat meminta bantuan, sampaikan model komputer, model drive jika diketahui, apakah drive terlihat di BIOS, pemeriksaan kabel/port yang sudah dilakukan, perubahan BIOS terakhir, dan apakah data pada drive perlu diselamatkan.
