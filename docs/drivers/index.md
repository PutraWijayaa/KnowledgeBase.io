# Mengatasi Masalah dan Memperbarui Driver Windows

Driver membantu Windows mengenali dan menggunakan perangkat seperti kartu grafis, Wi-Fi/LAN, chipset, audio, Bluetooth, dan penyimpanan. Jika perangkat tidak terdeteksi, kinerjanya menurun, muncul pesan kesalahan, atau berhenti berfungsi setelah pembaruan, ikuti pemeriksaan berikut.

<div class="image-card">
    <img src="../assets/Knowledgebase%20IT/upload/Masalah%20dan%20Pembaruan%20Driver.png" alt="Infografik masalah driver dan langkah memperbarui driver Windows melalui Device Manager">
</div>

!!! warning "Unduh driver dengan aman"
    Gunakan Windows Update atau situs resmi produsen komputer/perangkat. Hindari aplikasi pembaru driver dan situs unduhan pihak ketiga yang tidak tepercaya. Driver yang salah atau tidak kompatibel dapat membuat perangkat tidak berfungsi atau Windows tidak stabil.

## Gejala masalah driver

- Perangkat tidak muncul atau tampil sebagai **Unknown device / Perangkat tidak dikenal** di Device Manager.
- Ada tanda seru kuning atau kode kesalahan pada perangkat.
- Wi-Fi, suara, Bluetooth, grafis, atau penyimpanan tidak bekerja seperti biasanya.
- Masalah muncul setelah pembaruan Windows, pemasangan perangkat, atau pembaruan driver.

Driver yang umumnya diperiksa sesuai gejalanya:

| Gejala | Driver yang perlu diperiksa |
| --- | --- |
| Tampilan, grafis, atau resolusi bermasalah | Graphics / Display adapter |
| Wi-Fi atau LAN tidak terhubung | Network / Wi-Fi / LAN |
| USB atau perangkat motherboard tidak dikenali | Chipset atau USB |
| Tidak ada suara | Audio |
| Bluetooth tidak tersedia | Bluetooth |
| Drive penyimpanan tidak dikenali Windows | Storage / SATA / NVMe |

## 1. Perbarui driver melalui Device Manager

1. Simpan pekerjaan yang terbuka dan sambungkan komputer ke internet jika diperlukan.
2. Tekan **Windows + X**, lalu pilih **Device Manager / Pengelola Perangkat**.
3. Buka kategori perangkat yang bermasalah. Cari perangkat bertanda seru atau **Unknown device / Perangkat tidak dikenal**.
4. Klik kanan perangkat tersebut, lalu pilih **Update driver / Perbarui driver**.
5. Pilih **Search automatically for drivers / Cari driver secara otomatis**.
6. Jika Windows menemukan driver, ikuti instruksi hingga instalasi selesai.
7. Mulai ulang komputer jika diminta, lalu uji kembali perangkat.

Pencarian otomatis hanya memeriksa sumber yang tersedia bagi Windows dan tidak selalu menemukan driver terbaru atau khusus dari produsen. Jika Windows menyatakan driver terbaik sudah terpasang tetapi masalah berlanjut, lanjutkan ke Windows Update atau situs resmi produsen.

## Sebelum mulai

1. Simpan pekerjaan yang sedang terbuka.
2. Jika memungkinkan, sambungkan komputer ke internet. Untuk mengatasi Wi-Fi yang tidak berfungsi, gunakan kabel LAN atau tethering USB dari ponsel jika diizinkan oleh kebijakan sekolah.
3. Catat nama dan model laptop atau komputer. Pada laptop, utamakan driver dari produsen laptop karena driver dapat disesuaikan dengan perangkat tersebut.
4. Jika komputer meminta hak administrator, jangan mencoba melewati pembatasan. Minta tim IT memasang driver.

Nama menu mungkin sedikit berbeda antara Windows 10, Windows 11, dan bahasa sistem yang digunakan.

## 2. Periksa driver di Windows Update

1. Buka **Settings / Pengaturan**.
2. Pilih **Windows Update**.
3. Buka **Advanced options / Opsi lanjutan**, lalu cari **Optional updates / Pembaruan opsional**.
4. Buka bagian **Driver updates / Pembaruan driver**.
5. Pilih pembaruan yang sesuai dengan perangkat yang bermasalah, lalu pilih **Download & install / Unduh & instal**.
6. Mulai ulang komputer jika diminta dan uji kembali perangkat.

Tidak semua komputer akan menampilkan pembaruan driver opsional. Jika tidak ada pembaruan yang sesuai, lanjutkan ke metode berikutnya.

## 3. Identifikasi perangkat menggunakan Hardware ID

Gunakan cara ini bila nama perangkat tidak diketahui atau ditampilkan sebagai **Unknown device**.

1. Di **Device Manager**, klik kanan perangkat tersebut, lalu pilih **Properties / Properti**.
2. Buka tab **Details / Detail**.
3. Pada daftar **Property / Properti**, pilih **Hardware Ids / ID Perangkat Keras**.
4. Klik kanan nilai teratas, lalu pilih **Copy / Salin**. Nilai teratas biasanya paling spesifik.
5. Cari model perangkat atau Hardware ID itu hanya di situs dukungan resmi produsen komputer atau komponennya.
6. Cocokkan hasil dengan model perangkat, versi Windows, dan arsitektur sistem sebelum mengunduh driver.

Jangan mengunggah Hardware ID, nomor seri, atau informasi perangkat sekolah ke forum publik. Bila hasil pencarian tidak jelas, minta bantuan tim IT daripada mencoba driver yang tampak mirip.

## 4. Unduh driver dari situs resmi produsen

1. Buka halaman dukungan resmi produsen laptop atau komputer dan cari menggunakan **model perangkat**. Untuk perangkat rakitan, gunakan situs resmi produsen komponen yang tepat.
2. Periksa versi Windows dan tipe sistem di **Settings > System > About / Pengaturan > Sistem > Tentang**. Pilih sistem operasi dan arsitektur yang sesuai (misalnya 64-bit); jangan memasang driver untuk model atau versi Windows yang berbeda.
3. Unduh hanya driver yang diperlukan. Beberapa contoh:

   | Gejala | Driver yang mungkin diperlukan |
   | --- | --- |
   | Wi-Fi atau jaringan tidak berfungsi | Wi-Fi atau LAN |
   | Tidak ada suara | Audio |
   | Tampilan, resolusi, atau grafis bermasalah | Grafis |
   | USB atau chipset tidak terdeteksi | Chipset atau USB |
   | Bluetooth tidak tersedia | Bluetooth |

4. Buka file yang diunduh dan ikuti petunjuk pemasangan dari produsen. Jika situs menyediakan petunjuk khusus, ikuti petunjuk tersebut.
5. Mulai ulang komputer jika diminta.
6. Buka kembali **Device Manager** dan pastikan perangkat dapat digunakan tanpa tanda peringatan.

Jangan menonaktifkan antivirus, menjalankan file dari situs yang tidak dikenal, atau memasang beberapa driver yang tidak berkaitan sekaligus. Jika komputer dikelola sekolah dan meminta izin administrator, hubungi tim IT.

## 5. Periksa kembali perangkat setelah pembaruan

1. Mulai ulang komputer jika belum dilakukan.
2. Buka kembali **Device Manager** dan pastikan perangkat muncul tanpa tanda peringatan.
3. Uji fungsi yang bermasalah, seperti suara, koneksi Wi-Fi, Bluetooth, atau tampilan eksternal.
4. Jika masalah baru muncul setelah pembaruan driver, di **Device Manager** klik kanan perangkat, pilih **Properties / Properti > Driver > Roll Back Driver / Kembalikan Driver** jika tersedia.
5. Ikuti instruksi, mulai ulang komputer, lalu uji kembali. Jika opsi tidak tersedia atau memerlukan izin administrator, hubungi tim IT.

Jangan menghapus atau menonaktifkan perangkat sebagai percobaan. Jika Windows tidak dapat dijalankan normal setelah pembaruan, minta bantuan tim IT untuk pemulihan.

## Pemeriksaan ulang perangkat melalui Command Prompt

Langkah pilihan ini meminta Windows memindai ulang perangkat dan menampilkan paket driver yang telah terpasang; langkah ini tidak mengunduh atau memasang driver.

1. Cari **Command Prompt** dari menu Start.
2. Pilih **Run as administrator / Jalankan sebagai administrator** jika tersedia dan diizinkan.
3. Jalankan perintah berikut satu per satu:

   ```bat
   pnputil /scan-devices
   pnputil /enum-drivers
   ```

`pnputil /scan-devices` meminta Windows memindai ulang perangkat. `pnputil /enum-drivers` menampilkan paket driver pihak ketiga yang sudah ada di Windows. Daftar tersebut bukan rekomendasi driver untuk diunduh. Tutup Command Prompt setelah selesai, lalu periksa kembali **Device Manager**. Jika perintah tidak dikenal atau akses ditolak, lewati langkah ini dan gunakan metode lain atau hubungi tim IT.

## Jika driver belum berhasil dipasang

- **Perangkat masih bertanda seru atau tidak dikenal:** pastikan model komputer dan Hardware ID sudah cocok, lalu periksa kembali halaman dukungan resmi produsen.
- **Windows tidak menemukan driver:** coba **Pembaruan opsional**. Jika tidak tersedia, unduh driver yang tepat dari situs resmi produsen.
- **Pemasangan gagal:** mulai ulang komputer satu kali, pastikan file sesuai dengan model dan versi Windows, lalu ikuti kembali petunjuk resmi produsen. Jangan memaksa pemasangan driver yang tidak cocok.
- **Masalah muncul setelah pembaruan:** gunakan **Roll Back Driver / Kembalikan Driver** jika tersedia dan Anda berwenang.
- **Tidak ada koneksi internet:** gunakan koneksi kabel atau tethering yang diizinkan, atau minta tim IT membantu mengunduh driver dari komputer lain melalui sumber resmi.
- **Komputer meminta kata sandi administrator atau menolak pemasangan:** jangan mencoba melewati pembatasan. Minta bantuan tim IT.

## Kapan harus menghubungi tim IT?

Hubungi tim IT jika perangkat tetap tidak berfungsi setelah langkah di atas, driver untuk model perangkat tidak ditemukan, pemasangan ditolak, atau masalah terjadi pada banyak perangkat sekaligus. Sertakan:

- nama dan model komputer;
- versi Windows, jika diketahui;
- nama perangkat atau foto pesan kesalahan;
- langkah yang sudah dicoba dan hasilnya;
- waktu mulai terjadinya masalah.

Jangan menghapus driver yang masih berfungsi atau membongkar perangkat. Jika masalahnya tampak seperti kerusakan fisik, hentikan percobaan dan minta pemeriksaan.
