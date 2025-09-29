# Pratikum-3
Latihan Halaman Profil Instagram dengan Bootstrap 5
Proyek ini adalah implementasi halaman profil Instagram yang sepenuhnya responsif, dibuat menggunakan HTML, CSS, dan framework Bootstrap 5. Tujuannya adalah untuk mempraktikkan dan mendemonstrasikan pemahaman tentang sistem grid responsif, komponen, dan utilitas Bootstrap.

Struktur File
Struktur direktori proyek ini sederhana dan terorganisir sebagai berikut:

.
index.html              # File HTML utama untuk struktur halaman
README.md               # File penjelasan ini
assets/
css/
style.css       # File untuk styling kustom tambahan
img/
profile-pic.jpg # Contoh foto profil
post1.jpg       # Contoh gambar postingan

Cara Menjalankan (Build/Run)
Tidak ada proses build atau kompilasi yang diperlukan. Proyek ini murni berbasis file statis.

Cara menjalankan: Cukup buka file index.html di browser web modern pilihan Anda (seperti Google Chrome, Mozilla Firefox, atau Safari).

Dependensi
Proyek ini menggunakan beberapa library eksternal yang dimuat melalui CDN (Content Delivery Network), sehingga tidak perlu di-download secara manual.

Bootstrap 5.3.3 CSS & JS: Digunakan sebagai framework utama untuk layout, komponen, dan responsivitas.

Bootstrap Icons 1.11.3: Digunakan untuk ikon-ikon pada antarmuka, seperti ikon grid dan reels.

Pertanyaan & Penjelasan
1. Kenapa konfigurasi kolomnya dibuat beda-beda untuk setiap ukuran layar?
Singkatnya, biar tampilannya pas dan enak dilihat di perangkat apa pun, entah itu HP, tablet, atau komputer.

Di HP (1 kolom): Saya buat satu kolom penuh supaya tiap gambar postingan kelihatan besar dan jelas. Jadi, pengguna tidak perlu repot-repot zoom dan bisa lebih fokus ke satu konten.

Di Tablet (2 kolom): Layar tablet lebih lega, jadi sayang kalau hanya satu kolom. Dengan dua kolom, lebih banyak postingan yang bisa dilihat tanpa membuat gambarnya jadi terlalu kecil.

Di Komputer (4 kolom): Kalau di layar komputer yang lebar, menampilkan empat kolom sekaligus itu paling efisien. Pengguna bisa melihat banyak gambar dalam sekejap, pas untuk sekadar scrolling cepat.

2. Gimana caranya tombol "Edit Profile" tetap gampang dijangkau di HP?
Saya akali dengan "menyembunyikan" dan "memunculkan" tombol sesuai ukuran layar. Sebenarnya ada dua set tombol yang sama di dalam kode.

Satu set untuk Komputer: Tombol ini letaknya di samping nama pengguna. Tombol ini sengaja saya sembunyikan di tampilan HP dan baru akan muncul saat dibuka di layar yang lebih lebar (tablet/komputer).

Satu set lagi untuk HP: Tombol ini saya letakkan persis di bawah bio. Posisinya strategis, dan saya buat ukurannya memanjang selebar layar. Jadi, setelah orang selesai baca bio, tombolnya langsung kelihatan jelas dan gampang banget dipencet pakai jempol.

Dengan trik ini, posisi tombol bisa beradaptasi, memastikan fungsinya tetap maksimal di mana saja.

3. Kalau postingannya ada 50, apa masalahnya dan gimana solusinya?
Grid Bootstrap-nya sendiri sih tidak akan rusak, ia akan terus membuat baris baru ke bawah. Masalah utamanya ada di dua hal lain: loading yang super lemot dan pengalaman pengguna yang buruk.

Bayangkan harus memuat 50 gambar sekaligus, pasti berat sekali. Selain itu, pengguna harus scroll jauh sekali ke bawah hanya untuk melihat footer.

Solusinya adalah jangan memuat semua 50 gambar itu secara serentak. Ada dua cara populer untuk mengatasinya:

Dibagi per halaman (Paginasi): Ini cara klasik. Kita hanya tampilkan 12 postingan di halaman pertama. Kalau mau lihat sisanya, pengguna tinggal klik nomor halaman (2, 3, 4, dst.) di bagian bawah. Jelas dan simpel.

Digulir terus (Infinite Scroll): Ini cara yang dipakai Instagram asli. Awalnya, kita tetap muat 12 gambar. Nanti, saat pengguna scroll hampir ke bawah, kode akan otomatis memuat 12 gambar berikutnya. Jadi terasa lebih mulus dan modern, seolah-olah postingannya tidak ada habisnya.
