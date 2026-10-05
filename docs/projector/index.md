# Troubleshooting Proyektor dari Komputer Windows

Jika proyektor tidak menampilkan gambar atau tidak terdeteksi oleh komputer/laptop, ikuti pemeriksaan berikut dari sisi komputer secara berurutan. Nama menu dapat sedikit berbeda menurut versi Windows dan bahasa sistem.

<div class="image-card">
    <img src="../assets/Knowledgebase%20IT/upload/Panduan%20Troubleshooting%20Proyektor%20Windows.png" alt="Infografik troubleshooting proyektor dari komputer Windows: mode tampilan, resolusi, display adapter, kabel VGA, dan pemeriksaan lanjutan" width="100%">
</div>

!!! note "Tipe proyektor dapat berbeda"
    Gambar menampilkan contoh proyektor dan konektor tertentu. Langkah di panduan ini berfokus pada komputer Windows, sehingga dapat digunakan sebagai pemeriksaan awal untuk berbagai merek dan tipe proyektor. Nama port, kabel, resolusi yang didukung, menu, dan indikator proyektor tidak selalu sama.

## 1. Pilih mode tampilan Windows

1. Sambungkan kabel video ke komputer.
2. Tekan **Windows + P** untuk membuka pilihan mode proyeksi.
3. Coba satu mode pada satu waktu:

   | Mode | Fungsi |
   | --- | --- |
   | **PC screen only / Hanya layar PC** | Menampilkan gambar hanya pada layar komputer. Gunakan sementara untuk memastikan layar komputer kembali terlihat. |
   | **Duplicate / Duplikat** | Menampilkan gambar yang sama di komputer dan proyektor. Biasanya pilihan awal yang paling mudah untuk presentasi. |
   | **Extend / Perluas** | Menjadikan proyektor sebagai area desktop tambahan. Jendela presentasi mungkin perlu dipindahkan ke layar tersebut. |
   | **Second screen only / Hanya layar kedua** | Menampilkan gambar hanya pada proyektor/layar kedua. Layar komputer dapat menjadi gelap. |

4. Tunggu beberapa detik setelah memilih mode.
5. Jika layar kedua belum tampil, coba **Duplicate** terlebih dahulu, lalu uji mode lain bila diperlukan.
6. Bila layar komputer menjadi gelap dan gambar proyektor tidak muncul, tekan **Windows + P**, lalu pilih **PC screen only** untuk mengembalikan tampilan komputer.

## 2. Periksa dan sesuaikan resolusi layar

Resolusi yang tidak didukung layar kedua dapat menyebabkan gambar tidak tampil atau tampak tidak semestinya.

1. Klik kanan area kosong di desktop, lalu pilih **Display settings / Pengaturan tampilan**.
2. Jika Windows menampilkan dua layar, pilih layar kedua yang mewakili proyektor. Gunakan **Identify / Identifikasi** jika tersedia untuk mengetahui nomor layarnya.
3. Pada **Display resolution / Resolusi layar**, pilih resolusi yang ditandai **Recommended / Disarankan** atau resolusi yang diketahui didukung oleh proyektor dan adaptor.
4. Jika masih tidak tampil, uji resolusi lain yang tersedia dan didukung, satu per satu. Hindari memilih resolusi atau refresh rate di luar kemampuan layar.
5. Konfirmasikan perubahan hanya jika gambar tetap terlihat dan stabil. Jika muncul hitam atau **Out of range**, tunggu Windows mengembalikan pengaturan atau tekan **Esc** jika tersedia.
6. Setelah gambar tampil, gunakan resolusi yang stabil dan sesuai kebutuhan presentasi.

Opsi resolusi dan refresh rate dapat berbeda menurut komputer, driver, kabel, adaptor, dan perangkat tampilan. Jangan menganggap satu resolusi tertentu cocok untuk semua proyektor.

## 3. Minta Windows mendeteksi layar kedua

1. Buka **Settings / Pengaturan > System / Sistem > Display / Tampilan**.
2. Pastikan kabel video sudah terhubung, lalu pilih **Detect / Deteksi** di bagian beberapa layar jika opsi tersebut tersedia.
3. Tekan **Windows + P** dan pilih **Duplicate** untuk menguji tampilan.
4. Jika layar tetap tidak terdeteksi, lanjutkan ke pemeriksaan driver dan koneksi komputer.

## 4. Periksa display adapter di Device Manager

Display adapter adalah perangkat grafis yang mengirimkan gambar dari komputer ke layar eksternal.

1. Tekan **Windows + X**, lalu pilih **Device Manager / Pengelola Perangkat**.
2. Buka bagian **Display adapters / Adaptor tampilan**.
3. Pastikan adaptor grafis muncul dan tidak memiliki tanda peringatan. Nama bisa berupa Intel, AMD, NVIDIA, atau nama lain sesuai komputer.
4. Jika ada tanda panah ke bawah pada adaptor, berarti perangkat mungkin dinonaktifkan. Klik kanan adaptor tersebut dan pilih **Enable device / Aktifkan perangkat** jika Anda berwenang.
5. Jika terdapat tanda seru atau pesan kesalahan, catat nama adaptor dan pesan tersebut. Minta tim IT memeriksa driver yang tepat untuk model komputer.
6. Jika komputer dikelola organisasi, jangan memilih **Uninstall device / Hapus instalan perangkat**, menghapus driver, atau mengubah driver tanpa arahan teknisi.

Menonaktifkan display adapter saat layar sedang digunakan dapat membuat tampilan komputer atau layar eksternal menjadi gelap. Karena itu, jangan menonaktifkannya sebagai langkah coba-coba. Jika perubahan membuat layar tidak terlihat, tunggu pemulihan otomatis atau minta bantuan teknisi.

## 5. Periksa kabel dan port dari sisi komputer

1. Pastikan konektor video terpasang penuh pada port komputer yang benar.
2. Untuk VGA seperti yang tampak pada gambar, periksa konektor di sisi komputer. Pastikan pin tidak bengkok atau patah dan sekrup pengunci terpasang secukupnya tanpa dikencangkan paksa.
3. Untuk HDMI, USB-C, atau jenis lain, pastikan konektor dan adaptor sesuai dengan port komputer serta tidak longgar.
4. Jika tersedia dan diizinkan, coba port komputer lain yang mendukung keluaran video atau gunakan kabel/adaptor pengganti yang diketahui berfungsi.
5. Jika memakai USB-C, pastikan port tersebut mendukung output display; tidak semua port USB-C mendukung video.
6. Jangan memasukkan benda ke port, menekuk pin, atau memaksa konektor. Jika port komputer tampak rusak, hentikan penggunaan dan laporkan ke tim IT.

Pemeriksaan utama panduan ini dilakukan dari komputer. Jika kabel di sisi proyektor atau kondisi proyektor perlu diperiksa, minta operator atau teknisi melakukannya.

## 6. Uji untuk menemukan sumber masalah

Jika masih belum berhasil, lakukan pengujian terkontrol apabila perangkat tersedia dan penggunaannya diizinkan:

1. Sambungkan komputer ke layar eksternal lain yang diketahui berfungsi menggunakan kabel/adaptor yang sesuai.
2. Sambungkan komputer lain yang diketahui berfungsi ke kabel dan proyektor yang sama, dengan bantuan operator.
3. Catat hasilnya:

   - Jika komputer tidak menampilkan gambar ke beberapa layar eksternal, masalah mungkin ada pada pengaturan, port, adaptor, atau driver komputer.
   - Jika komputer dapat menampilkan gambar ke layar lain tetapi tidak ke proyektor tertentu, minta operator/teknisi memeriksa kabel, input, kompatibilitas, dan proyektor.
   - Jika komputer lain berhasil pada sambungan yang sama, minta tim IT memeriksa pengaturan atau driver komputer awal.

Jangan menyimpulkan proyektor rusak hanya dari satu kali pengujian. Koneksi, adaptor, mode tampilan, atau kompatibilitas dapat menjadi penyebab.

## Jika tetap belum berhasil

- Pilih **Duplicate** melalui **Windows + P** dan pastikan komputer kembali ke mode tampilan yang diinginkan.
- Periksa kembali kabel/adaptor serta port komputer, tanpa memaksa konektor.
- Catat apakah layar kedua terdeteksi di **Display settings** dan apakah display adapter menunjukkan peringatan.
- Mulai ulang komputer jika pekerjaan sudah disimpan dan kebijakan perangkat mengizinkan.
- Hubungi tim IT jika driver memerlukan pembaruan, port tampak rusak, layar tidak terdeteksi di beberapa perangkat, atau diperlukan izin administrator.

Saat meminta bantuan, sertakan model komputer, versi Windows jika diketahui, jenis kabel/adaptor, mode **Windows + P** yang dicoba, hasil **Detect**, pesan kesalahan, dan hasil pengujian dengan layar/kabel lain.
