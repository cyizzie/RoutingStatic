## Hasil Percobaan
Berdasarkan hasil tes koneksi ICMP yang dilakukan dalam percobaan routing static:
- **PC1** berhasil terhubung dengan **PC2, PC3, PC4, PC5, PC6, PC7, PC8, dan PC9**.
- **PC4** berhasil terhubung dengan **PC1, PC2, PC3, PC5, PC6, PC7, PC8, dan PC9**.
- **PC7** berhasil terhubung dengan **PC1, PC2, PC3, PC4, PC5, PC6, PC8, dan PC9**.

Semua perangkat dalam jaringan berhasil terhubung satu sama lain menggunakan protokol ICMP. Tidak ditemukan kendala dalam pengiriman paket ICMP, yang mengindikasikan bahwa konfigurasi routing statis telah diterapkan dengan baik. Setiap perangkat di jaringan dapat berkomunikasi dengan perangkat lain tanpa hambatan.

## Analisis Percobaan
Pada percobaan ini, fokus utamanya adalah mengonfigurasi routing statis untuk memungkinkan komunikasi antar jaringan yang dihubungkan oleh beberapa router. Masing-masing router telah dikonfigurasi dengan alamat IP dan disimpan ke dalam NVRAM agar konfigurasi tetap aktif meskipun perangkat di-restart. Dengan membuat tabel routing statis, setiap router mampu mengetahui jalur menuju jaringan lain yang tidak terhubung langsung. Rute ini ditambahkan secara manual untuk memastikan bahwa setiap router dapat meneruskan paket ke tujuan yang berada di luar subnetnya.

Tes koneksi dilakukan menggunakan protokol ICMP, di mana paket ping dikirim antar PC di berbagai jaringan. Tes ini bertujuan untuk memverifikasi bahwa perangkat yang berada di jaringan berbeda dapat saling berkomunikasi melalui router yang sudah dikonfigurasi. Hasil tes menunjukkan bahwa seluruh PC yang diuji berhasil merespons ping, menandakan tidak ada masalah dalam penerusan paket melalui routing statis yang diterapkan.

## Kesimpulan Percobaan
Konfigurasi routing statis yang dilakukan pada jaringan ini berjalan dengan sukses. Semua perangkat mampu saling terhubung dan berkomunikasi antar subnet tanpa mengalami masalah. Pengaturan rute yang ditambahkan secara manual memungkinkan setiap router untuk mengetahui dan meneruskan paket ke jaringan lain, menunjukkan bahwa routing statis dapat diandalkan untuk menghubungkan jaringan yang tidak terhubung secara langsung.
