# Use Case dan User Story, Pertemuan 10

Presentasi web 58 slide untuk mata kuliah **Analisis dan Desain Sistem Informasi
Perpustakaan**, Jurusan Ilmu Perpustakaan, Fakultas Adab dan Humaniora,
UIN Alauddin Makassar.

Pengampu: Bayu Rizki, M.Kom. Bobot tugas 5 persen. CPMK-2, Sub-CPMK 4.

## Menjalankan

Buka `index.html` di peramban. Tanpa pemasangan, tanpa internet. Fon tertanam
di dalam berkas dan seluruh gambar ada di folder `img/`.

## Tombol

| Tombol | Fungsi |
|---|---|
| `→` `←` `Spasi` | Pindah slide |
| `Home` `End` | Slide pertama atau terakhir |
| `G` | Menu lompat bagian, 18 bagian dari Sampul sampai Bagian P |
| `O` | Ikhtisar 58 slide, dikelompokkan per bagian |
| `F` | Layar penuh |
| `Esc` | Menutup pembesar gambar, menu bagian, atau ikhtisar |
| Usap kiri dan kanan | Pindah slide di ponsel atau tablet |

Tautan ke slide tertentu: tambahkan `#s42` di akhir alamat.
Kendali menghilang sendiri setelah 3 detik diam.

## Bagian yang bisa diklik saat mengajar

| Slide | Yang bisa dilakukan |
|---|---|
| Semua slide gambar | Klik pelat gambarnya untuk memperbesar satu layar penuh. Berguna untuk diagram padat seperti Gambar 9 dan Gambar 10. Tekan Esc untuk menutup. |
| 1, Sampul | Arahkan tetikus ke salah satu aktor. Use case dan garis asosiasi miliknya menyala, sisanya meredup. |
| 42, Pola kalimat | Klik bagian bergaris untuk menukar contoh. Peran, tujuan, alasan, dan kriteria penerimaan berganti bersama-sama. Empat contoh, semuanya dari materi modul. |
| 52, Delapan kesalahan | Klik satu baris untuk menandainya sudah ditemukan. Dipakai saat Langkah 5 praktikum ketika mengaudit Gambar 13. |
| 55, Jadwal praktikum | Klik angka menit untuk menjalankan penghitung mundur langkah itu. Klik lagi untuk menyetel ulang. |

Tidak ada teks yang disembunyikan menunggu diklik. Seluruh isi slide sudah
terbaca saat halaman terbuka. Yang berubah hanya penandaan dan contohnya.

## Menyembunyikan slide

Tiap slide diberi komentar penanda di `index.html`:

```html
<!-- ===== SLIDE 48 | Lampiran Perbedaan | Perbedaannya, dilihat dari letaknya ===== -->
<section class="slide">
```

Cari penandanya dengan Ctrl+F, lalu tambahkan `hide` pada kelasnya:

```html
<section class="slide hide">
```

Nomor halaman ikut menyesuaikan sendiri, tidak ada nomor yang lompat.
Boleh juga dengan `data-hide`. Hapus kembali untuk memunculkannya.

Lima slide Lampiran ada di nomor 46 sampai 50. Kalau waktu kelas tidak cukup,
kelimanya dapat disembunyikan tanpa memutus alur pertemuan.

## Menyalakan GitHub Pages

Settings, lalu Pages, lalu Source: Deploy from a branch, branch `main`,
folder `/ (root)`, lalu Save. Tunggu alur kerja *pages build and deployment*
di tab Actions sampai hijau, lalu muat ulang dengan `Ctrl+Shift+R`.

## Catatan desain

Latar hijau kehitaman. Diagram asli dari modul tampil sebagai pelat putih
bercahaya, seperti lembar gambar di bawah lampu meja.

- **Archivo 800** untuk judul, **IBM Plex Sans** untuk isi, **IBM Plex Mono** untuk label
- Hijau `#248252` dan emas `#E1A835` dari logo UIN Alauddin. Hijau menandai yang
  benar dan sudah pasti. Emas menandai pertanyaan, dugaan, dan yang perlu diperiksa
- Kurung siku di sudut tiap pelat gambar mengutip **batas sistem**, gagasan inti
  diagram use case
- Kode bagian ditampilkan sebagai chip hijau, bukan dipisah tanda baca
- Rel di tepi kiri: penanda emas bergeser turun mengikuti posisi slide, dan garis
  putih menandai awal tiap bagian
- Kedelapan belas gambar use case dipakai apa adanya dari modul, tidak ada yang
  digambar ulang

## Lisensi materi

Materi kuliah milik penulis. Gambar dibuat untuk modul praktikum P10.
