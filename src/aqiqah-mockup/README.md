# Mockup Habib Aqiqah

Redesign aplikasi aqiqah, gaya mengikuti repo `ulasanaku` (netral + aksen teal, font sistem). Satu file HTML per halaman, tanpa build.

| File | Isi |
|---|---|
| `form.html` | Redesign `genz/inputh/form.php`. **Siap pakai**: 31 field dengan `name` dan nilai pilihan yang sama persis, `action="insertdata.php"`, `method="POST"`. Di domain habibaqiqah.com form langsung terkirim; di tempat lain tampil pratinjau data. |
| `index.html` | Prototipe aplikasi: sisi pelanggan (beranda, pesan 4 langkah, lacak) dan panel admin (dashboard, pesanan, jadwal, stok, keuangan, pelanggan). |

## Memasang form baru di server

1. Backup `genz/inputh/form.php` (mis. `form.php.bak`).
2. Upload `form.html` ke `genz/inputh/`, lalu ganti nama menjadi `form.php` (atau simpan sebagai `form2.php` untuk uji coba dulu).
3. Isi satu data uji dan pastikan masuk ke database lewat `insertdata.php`.

Catatan perilaku yang berbeda dari form lama:
- Nominal rupiah diketik dengan titik ribuan, tetapi dikirim sebagai angka murni.
- Biaya bungkus, ongkir, biaya lain, dan discount yang dikosongkan dikirim sebagai `0` (form lama mewajibkan diisi).
- Draf tersimpan di browser sampai data terkirim.

## Data

- Field dan pilihan (Dapur, Courier, Agen, CS, Tkm, Jumlah Kambing, Tipe Box, Nama Box, Jumlah Box, Bank) diambil dari `form.php` asli.
- **Harga dan baris pesanan di `index.html` adalah contoh.** `aqiqahasli.php` membutuhkan login, jadi data tabel asli belum dipakai. Untuk memakai data asli: export tabel dari phpMyAdmin (database `jof43217_aqasli`) ke CSV.
