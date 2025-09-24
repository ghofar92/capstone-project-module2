### Latar Belakang
Transjakarta merupakan salah satu moda transportasi umum utama di Jakarta yang digunakan oleh jutaan penumpang setiap harinya. Dengan banyaknya jumlah perjalanan dan rute yang tersedia, manajemen Transjakarta menghadapi tantangan besar dalam memastikan layanan yang efisien dan memadai.

Tanpa analisis pola perjalanan penumpang yang memadai, Transjakarta berisiko mengalami:

- Penumpukan penumpang pada jam sibuk akibat kekurangan armada.
- Rute tidak efisien, di mana ada rute yang kelebihan armada sementara rute lain kekurangan.
- Jadwal bus yang tidak optimal, yang dapat memperpanjang waktu tunggu dan menurunkan kepuasan penumpang.

Dataset transaksi perjalanan penumpang yang tersedia, mencakup waktu naik (tap in), turun (tap out), rute, dan pembayaran, memungkinkan identifikasi jam sibuk, halte dengan jumlah penumpang terbanyak, serta rata-rata lama perjalanan. Dengan analisis ini, Transjakarta dapat mengambil keputusan strategis untuk menambah armada di jam tertentu, mengoptimalkan jadwal, serta meningkatkan kualitas layanan di koridor dengan tingkat penggunaan tertinggi.

### Permasalahan
Permasalahan yang akan dianalisis dalam proyek ini adalah:
- Bagaimana distribusi perjalanan penumpang berdasarkan waktu (jam sibuk)?
- Koridor dan halte mana yang paling banyak digunakan penumpang?
- Berapa lama rata-rata waktu perjalanan penumpang?
- Bagaimana distribusi penumpang berdasarkan kategori pembayaran (gratis atau berbayar)?
- Apakah ada perbedaan pola perjalanan berdasarkan jenis kelamin atau tahun lahir penumpang?

Dengan menjawab pertanyaan-pertanyaan tersebut, diharapkan diperoleh insight yang dapat membantu manajemen Transjakarta dalam mengoptimalkan operasi bus dan meningkatkan pengalaman penumpang.

Dataset ini berisi informasi terkait transaksi perjalanan penumpang Transjakarta.  
Data mencakup identitas kartu, rute perjalanan, lokasi dan waktu tap in/out, serta jumlah pembayaran.  
Ada 22 kolom di dalam dataset `Transjakarta.csv`, yaitu:

- **transID** : ID unik untuk setiap transaksi.
- **payCardID** : Identitas utama pelanggan. Kartu ini digunakan untuk tap in dan tap out.
- **payCardBank** : Nama bank penerbit kartu pelanggan.
- **payCardName** : Nama pelanggan yang tertera pada kartu.
- **payCardSex** : Jenis kelamin pelanggan (sesuai data pada kartu).
- **payCardBirthDate** : Tahun lahir pelanggan.
- **corridorID** : ID koridor/rute yang digunakan (berguna untuk pengelompokan rute).
- **corridorName** : Nama koridor/rute yang berisi titik awal dan akhir perjalanan.
- **direction** : Arah perjalanan (0 = Pergi, 1 = Pulang).
- **tapInStops** : ID halte tempat pelanggan melakukan tap in.
- **tapInStopsName** : Nama halte tempat pelanggan tap in.
- **tapInStopsLat** : Latitude (garis lintang) halte tap in.
- **tapInStopsLon** : Longitude (garis bujur) halte tap in.
- **stopStartSeq** : Urutan halte dari awal perjalanan (halte ke-1, ke-2, dst).
- **tapInTime** : Waktu pelanggan melakukan tap in (tanggal & jam).
- **tapOutStops** : ID halte tempat pelanggan melakukan tap out.
- **tapOutStopsName** : Nama halte tempat pelanggan tap out.
- **tapOutStopsLat** : Latitude (garis lintang) halte tap out.
- **tapOutStopsLon** : Longitude (garis bujur) halte tap out.
- **stopEndSeq** : Urutan halte sampai akhir perjalanan (halte ke-1, ke-2, dst).
- **tapOutTime** : Waktu pelanggan melakukan tap out (tanggal & jam).
- **payAmount** : Jumlah yang dibayar pelanggan. Ada yang gratis, ada yang berbayar.

