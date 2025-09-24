# Executive Summary
Transjakarta merupakan salah satu moda transportasi umum utama di Jakarta yang digunakan oleh jutaan penumpang setiap harinya. 
Dengan banyaknya jumlah perjalanan dan rute yang tersedia, manajemen Transjakarta menghadapi tantangan besar dalam memastikan layanan yang efisien dan memadai.

Tanpa analisis pola perjalanan penumpang yang memadai, Transjakarta berisiko mengalami:
- Penumpukan penumpang pada jam sibuk akibat kekurangan armada.
- Rute tidak efisien, di mana ada rute yang kelebihan armada sementara rute lain kekurangan.
- Jadwal bus yang tidak optimal, yang dapat memperpanjang waktu tunggu dan menurunkan kepuasan penumpang.

Dengan melakukan analisis, Transjakarta dapat mengambil keputusan strategis untuk menambah armada di jam sibuk, mengoptimalkan jadwal, serta meningkatkan kualitas layanan dan kepuasan penumpang.

---

## Permasalahan / Research Question
- Bagaimana distribusi perjalanan penumpang berdasarkan waktu (jam sibuk)?
- Koridor dan halte mana yang paling banyak digunakan penumpang?
- Berapa lama rata-rata waktu perjalanan penumpang?
- Bagaimana distribusi penumpang berdasarkan kategori pembayaran (gratis atau berbayar)?
- Apakah ada perbedaan pola perjalanan berdasarkan jenis kelamin atau tahun lahir pelanggan?

---

## Dataset
Dataset ini berisi informasi transaksi perjalanan penumpang Transjakarta.
Terdapat **22 kolom** di dalam dataset `Transjakarta.csv`:
- `transID` : ID unik untuk setiap transaksi.
- `payCardID` : Identitas unik kartu pelanggan.
- `payCardBank` : Nama bank penerbit kartu pelanggan.
- `payCardName` : Nama pelanggan yang tertera pada kartu.
- `payCardSex` : Jenis kelamin pelanggan.
- `payCardBirthDate` : Tahun lahir pelanggan.
- `corridorID` : ID koridor/rute yang digunakan.
- `corridorName` : Nama koridor/rute.
- `tapInStops` : ID halte tap in.
- `tapInStopsName` : Nama halte tap in.
- `tapInStopsLat`, `tapInStopsLon` : Koordinat halte tap in.
- `tapStopStartSeq` : Urutan halte awal dari perjalanan.
- `tapInTime` : Waktu pelanggan melakukan tap in.
- `tapOutStopsName` : Nama halte tap out.
- `tapOutTime` : Waktu pelanggan melakukan tap out.
- `payAmount` : Jumlah pembayaran perjalanan.

---

## Teknologi yang Digunakan
- Python 3.x
- Pandas
- Matplotlib
- Seaborn
- Jupyter Notebook

---

## Visualisasi & Analisis
- **Boxplot** → Untuk mendeteksi outlier pada kolom `payAmount`.
- **Bar Chart** → Untuk menemukan 10 halte dan koridor dengan jumlah perjalanan tertinggi.
- **Distribusi Waktu** → Untuk melihat pola perjalanan berdasarkan jam.

---


