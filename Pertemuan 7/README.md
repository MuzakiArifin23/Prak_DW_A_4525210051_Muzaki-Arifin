# Praktikum Desain Web - HTML Form Dasar: Input & Pengiriman Data

**Nama:** Muhamad Rasha Zein
**NPM:** 4525210042

## Struktur Folder

```
latihan/
├── individu/desain-web/pertemuan-07/
│   ├── index.html
│   ├── css/style.css
│   ├── images/
│   └── dokumentasi/   (desktop.png, mobile.png)
└── studi-kasus/desain-web/pertemuan-07/
    ├── index.html
    ├── css/style.css
    ├── images/
    └── dokumentasi/   (desktop.png, mobile.png)
```

## Hasil Tampilan

### Individu - Form Pencarian Data Mahasiswa

| Desktop | Mobile |
|---|---|
| ![Desktop](latihan/individu/desain-web/pertemuan-07/dokumentasi/desktop.png) | <img src="latihan/individu/desain-web/pertemuan-07/dokumentasi/mobile.png" width="260" alt="Mobile"> |

### Studi Kasus - Form Pendaftaran Mahasiswa

| Desktop | Mobile |
|---|---|
| ![Desktop](latihan/studi-kasus/desain-web/pertemuan-07/dokumentasi/desktop.png) | <img src="latihan/studi-kasus/desain-web/pertemuan-07/dokumentasi/mobile.png" width="260" alt="Mobile"> |

## Ringkasan

Pada praktikum ini saya membuat dua form HTML: form pencarian data mahasiswa (individu) dan form pendaftaran mahasiswa (studi kasus). Setiap field saya susun dalam div form-group yang berisi label dan kontrol input, lalu label dihubungkan dengan input melalui atribut for yang sama dengan id. Setiap kontrol juga saya beri atribut name supaya datanya punya key saat dikirim ke backend. Form individu memakai input text, number, dan date, serta tiga jenis button: submit, reset, dan button biasa. Form studi kasus memuat input text, email, password, number, dan date, ditambah select program studi dan textarea alamat, dengan tiga jenis button yang sama.

Masalah yang saya temui adalah memilih method yang tepat dan menjaga agar id dan for tidak salah ketik, karena kalau berbeda maka label tidak terhubung dengan input. Solusinya, saya memakai method get untuk form pencarian karena datanya dikirim lewat URL dan berupa kata kunci pencarian, sedangkan form pendaftaran memakai post karena memuat password dan data pribadi yang dikirim lewat body request. Saya mengecek ulang setiap pasangan for dan id satu per satu. Saya juga menambahkan atribut required, min, dan max agar validasi dasar berjalan di browser. Saya sadar method post tidak otomatis membuat data aman, sehingga HTTPS dan validasi server tetap diperlukan. Tombol reset saya sertakan sesuai tugas, tetapi pada proyek nyata perlu hati-hati karena bisa menghapus isian pengguna secara tidak sengaja.