# Cara Merestart Access Point

Restart access point dapat membantu mengatasi koneksi yang bermasalah, jaringan tidak stabil, atau perangkat yang tidak merespons. Langkah umum di bawah ini dapat digunakan untuk berbagai tipe access point, tetapi letak sakelar, nama port, indikator, dan cara catu dayanya dapat berbeda. Ikuti label pada perangkat serta panduan resmi produsennya. Restart mematikan dan menyalakan kembali perangkat, bukan menghapus konfigurasi.

<div class="image-card">
    <img src="../../assets/Knowledgebase%20IT/upload/Panduan%20Restart%20TP-Link%20TL-WR940N.png" alt="Contoh cara merestart access point TP-Link TL-WR940N dengan mencabut daya atau menggunakan tombol On/Off">
</div>

!!! note "Model pada gambar hanya contoh"
    Gambar menggunakan **TP-Link TL-WR940N (EU)** sebagai contoh. Nama port, posisi tombol, spesifikasi adaptor, indikator, dan alamat administrasi yang tampak pada gambar tidak berlaku untuk semua access point.

!!! warning "Pastikan Anda berwenang"
    Jika access point melayani jaringan kantor/sekolah atau digunakan banyak orang, beri tahu administrator/tim IT dan pastikan restart tidak mengganggu pekerjaan penting. Jangan menekan tombol **Reset** atau lubang bertanda **Reset** untuk merestart karena tindakan tersebut dapat menghapus konfigurasi. Tombol WPS juga bukan tombol restart.

## Sebelum mulai

1. Pastikan perangkat yang akan direstart adalah access point yang benar. Periksa label merek dan model pada perangkat.
2. Beri tahu pengguna lain jika restart dapat memutus koneksi mereka.
3. Cari panduan resmi untuk model perangkat jika tidak yakin bagaimana mematikan dayanya. Access point dapat menggunakan adaptor daya, kabel daya, atau **Power over Ethernet (PoE)** melalui kabel jaringan.
4. Jangan mencabut kabel LAN/WAN atau kabel jaringan PoE untuk merestart kecuali panduan perangkat atau administrator menginstruksikannya. Kabel tersebut mungkin diperlukan untuk koneksi atau catu daya.
5. Jika perangkat atau adaptor terasa sangat panas, berbau terbakar, mengeluarkan bunyi tidak normal, atau kabelnya rusak, jangan lanjutkan. Putuskan daya dengan aman dan hubungi teknisi.

## Metode 1: Restart dengan mencabut kabel daya

Gunakan cara ini jika produsen mengizinkan perangkat dimatikan dengan melepas sumber dayanya. Ini adalah cara yang ditunjukkan pada gambar untuk model contoh.

1. Identifikasi sumber daya perangkat: adaptor atau kabel daya, atau sambungan PoE melalui injektor/switch PoE.
2. Matikan atau putuskan sumber daya dengan cara yang dianjurkan produsen. Jika melepas konektor, pegang konektornya, bukan menarik kabel.
3. Tunggu **10–15 detik** agar perangkat benar-benar mati.
4. Sambungkan kembali daya atau nyalakan sumber PoE seperti sebelumnya. Jangan memaksakan konektor.
5. Pastikan indikator daya menyala kembali, jika tersedia.
6. Tunggu perangkat selesai melakukan booting. Waktunya berbeda-beda menurut model; ikuti panduan produsen dan jangan memutus daya berulang kali saat perangkat mulai menyala.

Jika sumber dayanya tidak jelas, kabel tidak mudah dilepas, konektor longgar, atau perangkat mendapat daya melalui sistem terkelola, jangan mencoba melepas kabel sembarangan. Minta bantuan administrator/teknisi.

## Metode 2: Restart dengan tombol On/Off

Gunakan cara ini hanya jika access point memiliki sakelar daya **On/Off** yang memang ditujukan untuk mematikan perangkat. Tidak semua model memilikinya.

1. Temukan sakelar yang secara jelas berlabel **On/Off**, **Power**, atau padanannya. Pastikan itu bukan tombol **Reset** atau **WPS**.
2. Pindahkan sakelar ke posisi **OFF** sesuai label perangkat. Penandaan sakelar dapat berbeda; jangan mengandalkan posisi tombol pada gambar contoh.
3. Tunggu sampai perangkat mati dan indikator daya padam, jika tersedia.
4. Pindahkan sakelar kembali ke posisi **ON**.
5. Tunggu proses booting selesai sesuai panduan model, lalu periksa koneksi.

Jika tidak ada sakelar yang jelas, gunakan metode memutus sumber daya hanya jika dianjurkan produsen; jika ragu, tanyakan kepada administrator/teknisi.

## Kenali jenis daya dan port

Jenis daya dan tata letak port berbeda antarperangkat. Periksa label pada access point dan panduan resmi modelnya. Contoh pada gambar TL-WR940N (EU) menunjukkan:

| Bagian | Fungsi |
| --- | --- |
| **Power (DC IN)** | Masukan daya dari adaptor pada model contoh |
| **LAN 1–4** | Port jaringan lokal pada model contoh |
| **WAN (Internet)** | Port koneksi ke jaringan/internet pada model contoh |
| **WPS/Reset** | Fungsi tombol pada model contoh; bukan tombol restart biasa |

Spesifikasi adaptor pada gambar (**12 V DC, 1 A**, konektor barel **5,5 × 2,1 mm**) hanya contoh untuk perangkat yang ditampilkan. Spesifikasi daya access point lain bisa berbeda, atau menggunakan PoE. Jangan menukar adaptor berdasarkan bentuk konektor saja; cocokkan tegangan, arus, polaritas, standar PoE, dan spesifikasi resmi perangkat. Jangan memasang adaptor yang tidak sesuai.

## Setelah access point dinyalakan kembali

1. Tunggu hingga proses booting selesai; lama proses bergantung pada model.
2. Periksa indikator daya, Wi-Fi, dan jaringan jika perangkat memilikinya. Nama, warna, dan pola indikator berbeda-beda.
3. Pastikan kabel daya serta kabel jaringan yang diperlukan terpasang dengan baik.
4. Sambungkan kembali komputer atau ponsel ke jaringan Wi-Fi atau LAN.
5. Coba buka situs atau layanan yang sebelumnya bermasalah.

Lampu yang menyala tidak selalu berarti koneksi internet sudah tersedia. Periksa apakah perangkat dapat tersambung ke jaringan dan mengakses internet.

## Jika koneksi masih bermasalah

1. Pastikan access point sudah selesai booting dan sumber daya serta kabel jaringan terpasang sesuai label dan panduan modelnya.
2. Periksa indikator yang tersedia dan cocokkan artinya dengan panduan resmi perangkat.
3. Coba sambungkan kembali perangkat pengguna ke Wi-Fi.
4. Jika Anda administrator dan berwenang mengelola perangkat, gunakan alamat administrasi dan prosedur login yang ditetapkan untuk model serta jaringan tersebut. Alamat **http://192.168.0.1** hanya contoh yang ditampilkan pada gambar; alamat sebenarnya dapat berbeda atau sudah diubah.
5. Jangan mengubah konfigurasi Wi-Fi, WAN, DHCP, atau pengaturan lain tanpa mengetahui nilai yang benar. Jangan membagikan kata sandi administrator.
6. Jika jaringan tetap tidak berfungsi atau lampu indikator menunjukkan masalah, catat kondisi indikator dan hubungi administrator jaringan atau tim IT.

**Jangan melakukan factory reset** kecuali diarahkan oleh administrator/teknisi dan konfigurasi perangkat sudah dicadangkan atau tersedia untuk dipasang kembali. Factory reset berbeda dari restart dan dapat menghapus pengaturan jaringan.
