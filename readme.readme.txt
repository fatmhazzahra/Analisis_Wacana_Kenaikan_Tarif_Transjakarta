Optimalisasi Transjakarta :
Analisis Skema Wacana Kenaikan Tarif Transjakarta

Latar Belakang

Transjakarta diresmikan pada 15 Januari 2004 pada era Gubernur Sutiyoso. Transjakarta tercatat sebagai sistem Bus Rapid Transit (BRT) pertama di Asia Tenggara dan Selatan. Dalam dua dekade perjalanannya, Transjakarta telah berkembang pesat menjadi sistem BRT dengan lintasan terpanjang di dunia, melayani jutaan penumpang setiap harinya melalui ekosistem yang terintegrasi, mulai dari bus besar di koridor utama hingga angkutan mikro (Mikrotrans/JakLingko) yang menjangkau pemukiman padat.

Sejak awal beroperasi hingga saat ini, tarif dasar Transjakarta dipatok sebesar Rp3.500, sebuah angka yang tetap bertahan meskipun terjadi fluktuasi harga bahan bakar, inflasi ekonomi, dan peningkatan Upah Minimum Provinsi (UMP) selama 20 tahun terakhir. Stabilitas tarif ini menjadikan Transjakarta sebagai jaring pengaman sosial yang krusial bagi mobilitas warga, namun di sisi lain menciptakan kesenjangan (gap) yang semakin lebar antara pendapatan tiket dan biaya operasional riil. Hal ini menjadikan beban subsidi semakin memberatkan Anggaran Pendapatan dan Belanja Daerah (APBD), Pemerintah Provinsi DKI Jakarta, sehingga pada akhir tahun 2025 mulai diadakan wacana penyesuaian tarif yang signifikan menjadi Rp5.000.

Meskipun kenaikan ini dinilai logis secara ekonomi, penerapannya menghadapi tantangan sosial yang besar. Masyarakat menuntut agar kenaikan harga dibarengi dengan peningkatan kualitas layanan, ketepatan waktu, dan kenyamanan armada. Oleh karena itu, diperlukan analisis berbasis data untuk merumuskan strategi yang meminimalkan gejolak resistensi publik.

Fokus Analisis
Bagaimana merancang skema penyesuaian tarif Transjakarta yang mampu menyeimbangkan target peningkatan pendapatan perusahaan dengan daya beli masyarakat, serta skema manakah (Flat, Peak Hour, atau Demografis) yang memberikan dampak paling efisien?

Tujuan Analisis
Analisis ini bertujuan untuk mengevaluasi tiga skenario kebijakan tarif menggunakan [data Transjakarta](https://drive.google.com/drive/folders/1S04hk5uHfHYe6J1S6fVqDunuja1Lk1Lo), dengan rincian sebagai berikut:
1. Kenaikan tarif flat / secara keseluruhan,
2. Kenaikan tarif berbasis Rush Hour,
3. Kenaikan tarif berbasis profil demografis.
Serta memberi rekomendasi kebijakan strategis berdasarkan ketiga skenario diatas.


Data yang digunakan dalam analisis ini adalah

Dataset Transjakarta yang memiliki 22 kolom informasi dan 37900 baris, dengan rincian sebagai berikut:

| Nama Kolom        | Deskripsi                                                       |
|-------------------|------------------------------------------------------------------|
| `TransID`           | ID transaksi unik untuk setiap transaksi                        |
| `PayCardID`         | ID kartu pelanggan dari kartu yang digunakan pelanggan sebagai tiket untuk masuk dan keluar |
| `PayCardBank`       | Nama bank penerbit kartu pelanggan                               |
| `PayCardName`       | Nama pelanggan yang tertera pada kartu                           |
| `PayCardSex`        | Jenis kelamin pelanggan yang tertera pada kartu                  |
| `PayCardBirthDate`  | Tahun kelahiran pelanggan                                        |
| `CorridorID`        | ID koridor dari perjalanan yang ditempuh pelanggan |
| `CorridorName`      | Nama koridor yang mencakup titik awal dan akhir dari setiap rute |
| `Direction`         | Arah rute perjalanan. 0 untuk Pergi, 1 untuk Kembali                       |
| `TapInStops`        | ID halte tap-in (masuk) untuk mengidentifikasi nama halte       |
| `TapInStopsName`    | Nama halte tap-in (masuk) tempat pelanggan melakukan tap-in      |
| `TapInStopsLat`     | Lintang dari halte tap-in (masuk)                               |
| `TapInStopsLon`     | Bujur dari halte tap-in (masuk)                                 |
| `StopStartSeq`      | Urutan halte, halte pertama, kedua, dan seterusnya. Terkait dengan arah |
| `TapInTime`         | Waktu saat tap-in (masuk). Tanggal dan waktu                             |
| `TapOutStops`       | ID halte tap-out (keluar) untuk mengidentifikasi nama halte     |
| `TapOutStopsName`   | Nama halte tap-out (keluar) tempat pelanggan melakukan tap-out  |
| `TapOutStopsLat`    | Lintang dari halte tap-out (keluar)                              |
| `TapOutStopsLon`    | Bujur dari halte tap-out (keluar)                                |
| `StopEndSeq`        | Urutan halte, halte pertama, kedua, dan seterusnya. Terkait dengan arah |
| `TapOutTime`        | Waktu saat tap-out (keluar). Tanggal dan waktu                            |
| `PayAmount`         | Jumlah yang dibayar pelanggan. Beberapa gratis, beberapa tidak  |


