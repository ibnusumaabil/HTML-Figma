UD KARYA ABADI — REVISI INTERAKSI WEBSITE

CARA MEMBUKA
1. Ekstrak seluruh ZIP (jangan membuka HTML dari dalam ZIP).
2. Buka index.html di folder hasil ekstrak menggunakan Chrome, Edge, atau Firefox.
3. Seluruh file HTML, style.css, script.js, dan folder assets harus tetap bersama.
Tidak perlu plugin Figma, npm, atau server untuk navigasi lokal.

TAMPILAN
Enam SVG asli pengguna dipertahankan byte-for-byte (SHA-256 sama dengan convert.zip). Tampilan awal tidak diganti; HTML/CSS menempatkan link, tombol, dan kolom input di atas SVG. Ukuran layar kecil mengikuti skala proporsional desain desktop. Revisi ini bukan rekonstruksi seluruh teks menjadi HTML editable.

INTERAKSI
- Menu utama dan logo, tombol Lihat produk, Detail Produk, Selengkapnya, Lihat detail material, dan footer terhubung.
- Pencarian, filter, urutkan harga/nama, grid/daftar, dan pagination memberi respons.
- Kartu Meja Kayu terhubung ke Detail Produk asli. Produk lain menampilkan nama/harga yang tersedia pada desain dan opsi konsultasi.
- Foto galeri, pilihan foto, pilihan warna, tab detail, dan berbagi produk memberi respons.
- FAQ pertama dapat ditutup/dibuka. Pertanyaan lain tidak memiliki jawaban di sumber; dialog memberikan opsi bertanya melalui WhatsApp, tidak mengarang jawaban.
- Form nama dan pesan dapat diisi, divalidasi dan menghasilkan link WhatsApp berisi pesan. Pengguna sendiri menekan tombol untuk membuka WhatsApp.
- Nomor di header/footer memakai +62 812 3456 7890; form halaman Kontak memakai +62 812 3458 7690. Ini dua nomor berbeda dalam desain; pemilik perlu memverifikasi nomor yang benar sebelum publikasi.
- Halaman 2–3 tidak memiliki data asli, sehingga tampil pemberitahuan dan kontrol kembali. URL akun Facebook/Instagram/TikTok tidak tersedia; tombol menampilkan informasi dan link kontak. Tidak ada katalog atau akun yang diada-adakan.

BATASAN FIDELITAS
25 navigasi Figma dengan tujuan valid dipertahankan. Aksi untuk tombol tanpa tujuan ditambahkan berdasarkan label dan konteks. Popup/filter/sort/tab yang ditambahkan bukan state visual Figma yang terverifikasi. Smart Animate diadaptasi menjadi efek CSS 200 ms, bukan reproduksi identik. Tidak ada varian foto tiap warna; pemilih warna menandai pilihan saja. Tidak ada backend, pengiriman pesan otomatis, atau validasi akun sosial/nomor WhatsApp.

PENGUJIAN
- 192 area kontrol awal lolos uji hit-test pusat elemen di Chromium, ukuran viewport 1440. Ukuran stage juga diuji pada lebar 390.
- Pengujian alur JavaScript dilakukan lewat pemuatan HTML/CSS/JS ke dokumen browser: pencarian, kartu, galeri, filter, sort, list, pagination, reset, foto/warna, tab, input, link pesan, dan FAQ. Tidak ada error JavaScript saat pengujian.
- SVG Kontak dimuat asli saat pengujian browser. Lima halaman lain memakai SVG uji berukuran sama untuk hit-test. Semua SVG asli diverifikasi identik dengan unggahan pengguna.
- Semua href lokal yang ditulis mengarah ke file yang tersedia. Kebijakan browser lingkungan pengujian memblokir navigasi file:// dan jaringan; navigasi antarfile aktual dan pembukaan WhatsApp di perangkat pengguna belum diuji end-to-end.
- Lihat kontrol.json dan uji-interaksi.json untuk rincian.
