# Cara Memasang Driver yang Hilang di Windows

Driver membantu Windows mengenali dan menggunakan perangkat seperti Wi-Fi, audio, Bluetooth, USB, dan kartu grafis. Jika perangkat tidak terdeteksi, memiliki tanda seru kuning, atau tidak berfungsi dengan benar, ikuti langkah-langkah berikut secara berurutan.

<div class="image-card">
    <img src="../assets/Knowledgebase%20IT/upload/Panduan%20Memasang%20Driver%20Hilang%20di%20Windows.png" alt="Infografik lima metode memasang driver yang hilang di Windows dan jenis driver untuk masalah umum">
</div>

!!! warning "Unduh driver dengan aman"
    Gunakan Windows Update atau situs resmi produsen perangkat. Hindari aplikasi pembaruan driver dan situs unduhan pihak ketiga yang tidak tepercaya. Driver yang salah dapat menyebabkan perangkat tidak berfungsi atau membuat Windows tidak stabil.

## Sebelum mulai

1. Simpan pekerjaan yang sedang terbuka.
2. Jika memungkinkan, sambungkan komputer ke internet. Untuk mengatasi Wi-Fi yang tidak berfungsi, gunakan kabel LAN atau tethering USB dari ponsel jika diizinkan oleh kebijakan sekolah.
3. Catat nama dan model laptop atau komputer. Pada laptop, utamakan driver dari produsen laptop karena driver dapat disesuaikan dengan perangkat tersebut.
4. Buka **Device Manager** dengan menekan **Windows + X**, lalu pilih **Device Manager** atau **Pengelola Perangkat**.
5. Cari perangkat yang bermasalah. Perangkat bisa berada di kategori yang sesuai atau muncul sebagai **Unknown device** di bagian **Other devices**. Tanda seru kuning biasanya menunjukkan ada masalah yang perlu diperiksa.

Nama menu mungkin sedikit berbeda antara Windows 10, Windows 11, dan bahasa sistem yang digunakan.

## Metode 1: Periksa dan perbarui melalui Device Manager

1. Di **Device Manager**, klik kanan perangkat yang bermasalah.
2. Pilih **Update driver** atau **Perbarui driver**.
3. Pilih **Search automatically for drivers** atau **Cari driver secara otomatis**.
4. Ikuti petunjuk Windows. Jika driver ditemukan, tunggu pemasangan selesai.
5. Mulai ulang komputer jika diminta, lalu periksa kembali perangkat tersebut.
6. Jika Windows menyatakan driver terbaik sudah terpasang tetapi perangkat masih bermasalah, lanjutkan ke Windows Update atau cari driver berdasarkan model perangkat.

Pencarian otomatis tidak selalu menemukan driver terbaru atau driver khusus dari produsen. Pesan tersebut tidak memastikan bahwa semua masalah perangkat sudah selesai.

## Metode 2: Periksa driver di Windows Update

1. Buka **Settings / Pengaturan**.
2. Pilih **Windows Update**.
3. Buka **Advanced options / Opsi lanjutan**, lalu cari **Optional updates / Pembaruan opsional**.
4. Buka bagian **Driver updates / Pembaruan driver**.
5. Pilih pembaruan yang sesuai dengan perangkat yang bermasalah, lalu pilih **Download & install / Unduh & instal**.
6. Mulai ulang komputer jika diminta dan uji kembali perangkat.

Tidak semua komputer akan menampilkan pembaruan driver opsional. Jika tidak ada pembaruan yang sesuai, lanjutkan ke metode berikutnya.

## Metode 3: Identifikasi perangkat menggunakan Hardware ID

Gunakan cara ini bila nama perangkat tidak diketahui atau ditampilkan sebagai **Unknown device**.

1. Di **Device Manager**, klik kanan perangkat tersebut, lalu pilih **Properties / Properti**.
2. Buka tab **Details / Detail**.
3. Pada daftar **Property / Properti**, pilih **Hardware Ids / ID Perangkat Keras**.
4. Klik kanan nilai teratas, lalu pilih **Copy / Salin**. Nilai teratas biasanya paling spesifik.
5. Cari model perangkat atau Hardware ID itu hanya di situs dukungan resmi produsen komputer atau komponennya.
6. Cocokkan hasil dengan model perangkat, versi Windows, dan arsitektur sistem sebelum mengunduh driver.

Jangan mengunggah Hardware ID, nomor seri, atau informasi perangkat sekolah ke forum publik. Bila hasil pencarian tidak jelas, minta bantuan tim IT daripada mencoba driver yang tampak mirip.

## Metode 4: Unduh driver dari situs resmi produsen

1. Buka halaman dukungan resmi produsen laptop atau komputer dan cari menggunakan **model perangkat**. Untuk perangkat rakitan, gunakan situs resmi produsen komponen yang tepat.
2. Pilih sistem operasi dan versi Windows yang benar. Jangan memasang driver untuk model atau versi Windows yang berbeda.
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

## Metode 5: Pindai perangkat melalui Command Prompt

Langkah ini bersifat pilihan dan hanya untuk pemeriksaan ulang perangkat. Perintah berikut tidak mengunduh atau memasang driver.

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
- **Masalah muncul setelah pembaruan:** di **Device Manager**, buka **Properties > Driver** dan periksa apakah **Roll Back Driver / Kembalikan Driver** tersedia. Gunakan hanya jika opsi tersebut tersedia dan Anda berwenang; jika ragu, hubungi tim IT.
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
