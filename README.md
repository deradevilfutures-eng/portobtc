# PortoBTC

Portofolio Bitcoin sederhana dan responsif untuk desktop, tablet, dan ponsel.

## Fitur
- Harga BTC/USDT dan perubahan 24 jam dari Binance.
- Grafik candlestick dengan interval 1m, 5m, 15m, 1h, 4h, dan 1d.
- WebSocket publik untuk pembaruan ticker dan candle; otomatis mencoba menyambung ulang.
- Catatan transaksi beli/jual, kalkulasi posisi, estimasi untung/rugi, dan ekspor CSV.
- Penyimpanan transaksi di localStorage browser; tidak memerlukan login atau API key.
- Pilihan tampilan USD/IDR. Konversi IDR bersifat perkiraan berdasarkan feed kurs publik.

## Deploy dengan GitHub Pages
1. Buka **Settings → Pages** pada repository.
2. Pada **Build and deployment**, pilih **Deploy from a branch**.
3. Pilih branch utama (misalnya `main`) dan folder **/(root)**, lalu tekan **Save**.
4. Tunggu proses deploy dan buka URL Pages yang ditampilkan GitHub.

## Catatan data dan keamanan
- Data pasar publik tidak dijamin memiliki latensi nol. Kecepatan pembaruan bergantung pada jaringan, browser, dan layanan bursa.
- Aplikasi ini hanya memantau pasar dan mencatat transaksi secara manual. Aplikasi tidak mengeksekusi order, tidak terhubung ke akun exchange, dan tidak meminta API key.
- Catatan transaksi hanya tersimpan di browser/perangkat saat ini. Bersihkan data situs/browser dapat menghapusnya. Gunakan Export CSV untuk membuat cadangan.
- Harga yang ditampilkan adalah BTC/USDT; tampilan IDR mengonversi estimasi nilai USD ke rupiah.
- CDN grafik dan endpoint harga memerlukan koneksi internet. Jika layanan publik membatasi akses atau sedang gangguan, data dapat terlambat atau tidak tersedia.

## Teknologi
HTML, CSS, JavaScript, Lightweight Charts, Binance public REST API + WebSocket.

Bukan saran investasi.
