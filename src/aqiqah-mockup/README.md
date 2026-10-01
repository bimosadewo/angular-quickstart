# Mockup Habib Aqiqah

Prototipe klik-able (satu file HTML, tanpa build) untuk redesign aplikasi aqiqah.

Buka `index.html` langsung di browser, atau setelah deploy Netlify di `/aqiqah-mockup/`.

## Isi

**Pelanggan**
- Beranda: hero dengan contoh pantauan live, ketentuan sunnah (L 2 ekor / P 1 ekor), paket (Potong Saja, Siap Saji, Nasi Box), daftar harga & stok per tipe kambing, alur layanan, ulasan.
- Pesan Aqiqah: wizard 4 langkah (data anak → kambing & paket → jadwal & alamat → pembayaran) dengan ringkasan harga live, hitung hari ke-7/14/21, DP 50% atau lunas, VA/QRIS.
- Lacak Pesanan: timeline status, video penyembelihan, foto, dan sertifikat aqiqah.

**Panel Admin**
- Dashboard: KPI, grafik ekor terjual per minggu, agenda hari ini, pesanan yang perlu tindakan.
- Pesanan: pencarian, filter status, drawer detail dengan ubah status, tagih WhatsApp, invoice.
- Jadwal Potong & Kirim (mingguan), Stok Kandang (jantan/betina, dikunci vs tersedia), Keuangan (omzet, laba, komposisi, piutang DP), Pelanggan.

**Form input** (`form.html`): redesign `genz/inputh/form.php` — field Jenis Kelamin, Anak ke, Ayah, Ibu, Tkm, Jumlah Kambing, Tipe Box, Nama Box, Jumlah Box diambil dari form asli; opsi pilihan dan harga masih contoh.

Semua data di dalam mockup adalah contoh. Field database asli (tabel pesanan di phpMyAdmin) belum dipetakan karena server tidak dapat diakses dari lingkungan pembuatan mockup.
