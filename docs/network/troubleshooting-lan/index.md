# Troubleshooting Internet Tidak Muncul di Komputer (Kabel LAN)

Jika komputer tidak terhubung ke internet melalui kabel LAN, lakukan pemeriksaan pada komputer terlebih dahulu sebelum memeriksa perangkat jaringan lainnya. Ikuti langkah secara berurutan dan uji koneksi setelah setiap perubahan. Berhenti jika koneksi sudah pulih.

<div class="image-card">
    <img src="../../assets/Knowledgebase%20IT/upload/Panduan%20Troubleshooting%20Internet%20Kabel%20LAN.png" alt="Infografik sembilan langkah troubleshooting internet kabel LAN pada komputer">
</div>

!!! warning "Jangan ubah pengaturan jaringan sekolah tanpa izin"
    IP statis, DNS, firewall, antivirus, VPN, router, dan switch dapat diatur khusus oleh sekolah. Jangan mengubahnya atau menonaktifkan perlindungan keamanan jika komputer dikelola sekolah. Jika diminta hak administrator atau Anda tidak mengetahui konfigurasi yang seharusnya, hentikan dan hubungi tim IT.

## 1. Periksa status koneksi jaringan

1. Lihat ikon jaringan di area notifikasi Windows.
2. Pastikan komputer menunjukkan koneksi Ethernet. Ikon globe, tanda silang, atau pesan **No Internet / Tidak ada internet** dapat menunjukkan masalah pada sambungan atau akses internet.
3. Jika ikon menunjukkan koneksi normal, tetapi hanya satu situs atau aplikasi yang tidak berfungsi, uji situs atau aplikasi lain sebelum mengubah pengaturan jaringan.
4. Jika Ethernet tidak tersambung, lanjutkan ke pemeriksaan adaptor dan kabel di bawah.

Ikon status hanya petunjuk awal: komputer bisa tersambung ke jaringan lokal tetapi belum memiliki akses internet.

## 2. Periksa driver LAN

1. Tekan **Windows + X**, lalu pilih **Device Manager / Pengelola Perangkat**.
2. Buka **Network adapters / Adaptor jaringan**.
3. Cari adaptor Ethernet atau LAN.
4. Pastikan adaptor muncul dan tidak memiliki tanda seru atau tanda peringatan.
5. Jika ada tanda peringatan, gunakan Windows Update atau panduan [Memasang Driver yang Hilang](../../drivers/index.md) untuk mencari driver yang sesuai dengan model perangkat.

Jika adaptor tidak terlihat sama sekali, driver tidak tersedia, atau Windows meminta izin administrator, minta bantuan tim IT.

## 3. Matikan dan aktifkan kembali adaptor

Langkah ini menyegarkan sambungan adaptor tanpa menghapus driver.

1. Di **Device Manager > Network adapters**, klik kanan adaptor Ethernet yang benar.
2. Pilih **Disable device / Nonaktifkan perangkat** dan tunggu beberapa detik.
3. Klik kanan adaptor yang sama dan pilih **Enable device / Aktifkan perangkat**.
4. Tunggu hingga Windows menyambungkan kembali Ethernet, lalu uji internet.

Jangan menonaktifkan adaptor yang tidak dikenali atau adaptor yang sedang dipakai untuk akses jarak jauh. Jika koneksi tetap tidak pulih, lanjutkan ke pemeriksaan kabel.

## 4. Lepas dan pasang kembali kabel LAN

1. Pastikan tidak ada proses penting yang sedang menggunakan koneksi kabel.
2. Lepas kabel LAN dari komputer dengan memegang konektornya, bukan menarik kabel.
3. Periksa konektor apakah retak, bengkok, longgar, atau kotor. Jangan memasukkan benda ke port.
4. Pasang kembali hingga konektor terkunci dan terdengar atau terasa klik.
5. Tunggu beberapa saat dan periksa apakah indikator koneksi pada komputer atau port jaringan menyala.

Jangan menarik kabel yang terikat atau terpasang permanen. Minta bantuan teknisi jika konektor atau instalasi kabel rusak.

## 5. Periksa kondisi kabel LAN

1. Periksa seluruh kabel. Hindari kabel yang tertekuk tajam, terjepit, terkelupas, atau konektornya rusak.
2. Jika ada kabel LAN lain yang diketahui berfungsi dan Anda diizinkan menggunakannya, coba kabel tersebut.
3. Jika koneksi pulih dengan kabel pengganti, hentikan penggunaan kabel yang diduga rusak dan laporkan untuk diganti.

Jangan memperbaiki konektor atau instalasi kabel sendiri jika tidak memiliki perlengkapan dan izin.

## 6. Periksa port LAN pada komputer

1. Periksa port Ethernet di komputer dan port jaringan di sisi lainnya.
2. Pastikan port tidak tampak retak, longgar, atau terhalang debu.
3. Jika kabel dan port lain tersedia serta diizinkan, uji dengan port LAN lain yang diketahui aktif.
4. Catat apakah lampu link pada port menyala atau berkedip.

Jangan membersihkan port dengan benda logam atau cairan. Jika port rusak atau tetap tidak menunjukkan link dengan kabel yang baik, hubungi teknisi atau tim IT.

## 7. Periksa pengaturan alamat IP

Untuk jaringan rumah biasa, alamat IP dan DNS biasanya diperoleh otomatis melalui DHCP. Jaringan sekolah dapat menggunakan konfigurasi khusus.

1. Buka **Control Panel / Panel Kontrol > Network and Internet > Network and Sharing Center**.
2. Pilih **Change adapter settings / Ubah pengaturan adaptor**.
3. Klik kanan **Ethernet > Properties / Properti**.
4. Pilih **Internet Protocol Version 4 (TCP/IPv4) > Properties**.
5. Jika jaringan memang menggunakan DHCP, pilih **Obtain an IP address automatically** dan **Obtain DNS server address automatically**.
6. Pilih **OK** dan uji koneksi kembali.

Jika alamat IP, subnet mask, gateway, atau DNS diatur oleh sekolah maupun teknisi, jangan menggantinya dengan otomatis. Mintalah nilai konfigurasi yang benar kepada tim IT.

## 8. Mulai ulang perangkat

1. Simpan pekerjaan dan mulai ulang komputer dari menu **Start > Power > Restart**.
2. Jika Anda mengelola router rumah, mulai ulang router mengikuti petunjuk produsennya, lalu tunggu sampai lampu koneksi stabil.
3. Jangan memulai ulang router atau switch jaringan sekolah tanpa izin karena dapat memutus koneksi pengguna lain.
4. Setelah perangkat siap, pastikan kabel terpasang dan coba kembali koneksi.

## 9. Jika masih bermasalah

1. Pastikan tidak ada gangguan dari penyedia layanan internet. Untuk koneksi rumah, periksa status layanan atau hubungi ISP. Untuk jaringan sekolah, tanyakan kepada tim IT.
2. Jika diizinkan, uji kabel atau port yang sama dengan perangkat lain. Ini membantu membedakan masalah komputer dari masalah kabel atau jaringan.
3. Jika hanya aplikasi tertentu yang terdampak, jangan mematikan firewall atau antivirus untuk pengujian. Periksa izin aplikasi melalui pengaturan resmi atau minta tim IT meninjau aturan keamanan.
4. Pada komputer sekolah, jangan membuat pengecualian firewall/antivirus atau mengubah VPN/proxy tanpa persetujuan administrator.
5. Jika Anda sempat mematikan perlindungan keamanan, aktifkan kembali segera.

Hubungi administrator jaringan, tim IT, atau ISP sesuai lokasi masalah. Sertakan nama komputer, lokasi, hasil pemeriksaan kabel/port, status lampu link, pesan kesalahan, waktu mulai masalah, dan langkah yang sudah dicoba.

## Perbedaan dari panduan LAN lainnya

Panduan ini menelusuri masalah mulai dari komputer, adaptor dan kabel hingga jaringan. Untuk langkah tambahan seperti reset komponen jaringan Windows, pemeriksaan firewall yang lebih rinci, dan DNS, lihat [Mengatasi Internet LAN yang Tidak Muncul](../lan-internet/index.md). Pada jaringan sekolah, ikuti kebijakan tim IT sebelum menjalankan reset atau mengganti DNS.
