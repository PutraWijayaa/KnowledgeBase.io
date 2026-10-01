# Mengatasi Internet LAN yang Tidak Muncul di Komputer

Ikuti langkah berikut secara berurutan jika komputer tidak mendapat koneksi internet melalui kabel LAN. Setelah setiap langkah, coba buka situs yang biasa digunakan. Jika koneksi sudah pulih, Anda tidak perlu melanjutkan ke langkah berikutnya.

<div class="image-card">
    <img src="../../assets/Knowledgebase%20IT/upload/Panduan%20Mengatasi%20Internet%20LAN%20Mati.png" alt="Infografik delapan langkah memeriksa koneksi internet LAN di Windows">
</div>

!!! warning "Jaringan sekolah mungkin dikelola oleh tim IT"
    Jangan mengubah konfigurasi router/switch, VLAN, proxy, DNS, firewall, antivirus, atau alamat IP statis jaringan sekolah tanpa izin. Bila perangkat meminta akun administrator atau pengaturan berbeda dari panduan ini, hentikan dan hubungi tim IT.

## 1. Periksa kabel LAN dan perangkat jaringan

1. Pastikan kabel Ethernet terpasang rapat pada komputer dan port LAN router, switch, atau stopkontak jaringan.
2. Periksa apakah lampu indikator pada port komputer dan router/switch menyala atau berkedip. Lampu mati bisa menunjukkan port, kabel, atau perangkat jaringan tidak tersambung.
3. Jika tersedia, coba kabel LAN lain yang diketahui berfungsi dan port jaringan lain yang disetujui.
4. Pastikan router atau switch menyala. Jangan mencabut kabel uplink, kabel daya, atau kabel jaringan lain yang digunakan bersama.

Jika kabel atau port tampak rusak, atau masalah terjadi di banyak komputer, sampaikan kepada tim IT. Jangan mencoba memperbaiki instalasi kabel sendiri.

## 2. Pastikan alamat IP didapatkan secara otomatis

Pada jaringan rumah biasa, komputer umumnya menerima alamat IP dan DNS secara otomatis melalui DHCP. Jaringan sekolah dapat menggunakan konfigurasi khusus; jangan mengganti konfigurasi yang diberikan tim IT.

1. Buka **Control Panel / Panel Kontrol**.
2. Pilih **Network and Internet > Network and Sharing Center**.
3. Pilih **Change adapter settings / Ubah pengaturan adaptor**.
4. Klik kanan **Ethernet**, lalu pilih **Properties / Properti**.
5. Pilih **Internet Protocol Version 4 (TCP/IPv4)**, lalu tekan **Properties / Properti**.
6. Jika jaringan Anda memang menggunakan DHCP, pilih **Obtain an IP address automatically** dan **Obtain DNS server address automatically**, lalu pilih **OK**.
7. Tutup jendela pengaturan dan uji koneksi kembali.

Jika pilihan ini sebelumnya diatur oleh sekolah atau teknisi, atau perangkat memerlukan IP statis, jangan mengubahnya. Hubungi tim IT untuk mendapatkan nilai yang benar.

## 3. Reset komponen jaringan Windows

Reset ini dapat membantu saat konfigurasi jaringan Windows bermasalah. Simpan pekerjaan terlebih dahulu. VPN, IP statis, atau konfigurasi jaringan khusus mungkin perlu disiapkan kembali.

1. Cari **Command Prompt**, klik kanan, lalu pilih **Run as administrator / Jalankan sebagai administrator** jika Anda berwenang.
2. Jalankan perintah berikut satu per satu. Tekan **Enter** setelah setiap perintah:

   ```bat
   netsh winsock reset
   netsh int ip reset
   ipconfig /flushdns
   ```

3. Baca hasil setiap perintah. Jika muncul pesan gagal atau akses ditolak, jangan mengulanginya dengan cara lain; hubungi tim IT.
4. Mulai ulang komputer, lalu sambungkan kembali kabel LAN dan uji koneksi.

## 4. Periksa driver Network Adapter

1. Tekan **Windows + X**, lalu pilih **Device Manager / Pengelola Perangkat**.
2. Buka kategori **Network adapters / Adaptor jaringan**.
3. Cari adaptor Ethernet (misalnya nama yang memuat **Ethernet**, **LAN**, atau produsen adaptor).
4. Jika ada tanda seru atau perangkat dinonaktifkan, klik kanan adaptor dan pilih **Update driver / Perbarui driver**. Ikuti petunjuk Windows atau panduan [Memasang Driver yang Hilang](../../drivers/index.md).
5. Jika adaptor dinonaktifkan, pilih **Enable device / Aktifkan perangkat**.
6. Jika masalah dimulai setelah pembaruan driver, periksa **Properties > Driver > Roll Back Driver** bila opsi itu tersedia.
7. Hindari **Uninstall device / Hapus instalan perangkat** jika Anda tidak memiliki hak administrator atau tidak yakin driver dapat dipasang kembali. Jika tim IT meminta melakukannya, jangan memilih opsi untuk menghapus driver dari komputer, lalu mulai ulang agar Windows mencoba mendeteksi perangkat kembali.

Jika adaptor Ethernet tidak muncul di Device Manager, hubungi tim IT untuk pemeriksaan perangkat keras atau driver yang tepat.

## 5. Periksa port router atau switch

Jika Anda berwenang mengelola router rumah:

1. Pastikan router/switch menyala dan port LAN yang digunakan menunjukkan indikator link.
2. Coba port LAN lain yang memang tersedia untuk perangkat Anda.
3. Jangan gunakan port **WAN/Internet** sebagai pengganti port **LAN** untuk menyambungkan komputer.

Pada jaringan sekolah, jangan masuk ke halaman admin router/switch, mengubah VLAN, memindahkan kabel uplink, atau mengubah pemfilteran MAC. Catat nomor port dan indikator lampunya, lalu laporkan ke tim IT.

## 6. Periksa firewall dan antivirus tanpa menurunkan keamanan

Firewall dan antivirus membantu melindungi komputer. **Jangan mematikan perlindungan secara permanen atau menonaktifkannya untuk menguji koneksi**, terutama pada komputer sekolah.

1. Jika hanya aplikasi tertentu yang tidak dapat tersambung, periksa apakah aplikasi tersebut diizinkan pada profil jaringan yang benar melalui pengaturan keamanan Windows atau aplikasi resmi sekolah.
2. Jangan membuat pengecualian untuk aplikasi atau alamat yang tidak dikenal. Minta tim IT meninjau aturan firewall jika perlu.
3. Jika Anda sudah mematikan firewall atau antivirus untuk pengujian, aktifkan kembali segera. Pada perangkat terkelola, hubungi tim IT untuk memastikan perlindungan kembali aktif.

Jika ikon jaringan menunjukkan koneksi tetapi internet tetap tidak berfungsi, lanjutkan ke pemeriksaan DNS dan uji perangkat lain. Firewall bukan satu-satunya penyebab masalah.

## 7. Periksa DNS

1. Buka **Control Panel > Network and Sharing Center > Change adapter settings**.
2. Klik kanan **Ethernet**, pilih **Properties**, lalu pilih **Internet Protocol Version 4 (TCP/IPv4) > Properties**.
3. Untuk jaringan yang menggunakan pengaturan otomatis, pilih **Obtain DNS server address automatically**.
4. Jangan memasukkan DNS publik seperti `8.8.8.8` atau `1.1.1.1` pada jaringan sekolah kecuali tim IT menginstruksikannya. DNS sekolah mungkin diperlukan untuk mengakses layanan internal, kebijakan penyaringan, atau sistem masuk.
5. Jika tim IT memberi alamat DNS tertentu, masukkan hanya nilai tersebut. Jika tidak, kembalikan ke pengaturan otomatis hanya bila jaringan menggunakan DHCP dan tidak ada konfigurasi khusus.
6. Pilih **OK**, tutup jendela, lalu uji kembali koneksi.

## 8. Mulai ulang komputer dan perangkat jaringan

1. Simpan pekerjaan, lalu mulai ulang komputer melalui menu **Start > Power > Restart**.
2. Setelah komputer menyala kembali, pastikan kabel LAN terpasang dan adaptor Ethernet aktif.
3. Jika Anda mengelola router rumah, Anda dapat memulai ulang router dengan tombol atau prosedur dari produsennya. Tunggu sampai koneksi kembali sebelum menguji.
4. Jangan mematikan atau memulai ulang router/switch sekolah tanpa izin; tindakan itu dapat memutus koneksi banyak orang.

## Jika internet masih tidak berfungsi

- Uji koneksi dengan perangkat lain pada kabel atau port yang sama, jika diizinkan. Ini membantu membedakan masalah komputer dari kabel, port, atau jaringan.
- Jika semua perangkat pada jaringan yang sama gagal, masalah mungkin berada pada router, switch, atau layanan internet. Pada koneksi rumah, hubungi penyedia layanan internet bila perangkat jaringan menunjukkan gangguan; pada jaringan sekolah, laporkan ke tim IT.
- Jika hanya satu komputer yang gagal, sampaikan nama komputer, lokasi dan nomor port (jika diketahui), lampu indikator port, pesan kesalahan, serta langkah yang sudah dicoba.
- Jangan mengubah alamat IP, VLAN, proxy, atau pengaturan keamanan lebih lanjut untuk mencoba memperbaiki koneksi tanpa arahan tim IT.
