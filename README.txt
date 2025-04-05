=== RJ AUTO METADATA v1.0 ===
Aplikasi Pemrosesan Metadata Gambar Otomatis (Portable Version)

== PERSYARATAN ==
- Windows 10 atau lebih baru (64-bit)
- Koneksi internet untuk mengakses API Gemini
- Tidak diperlukan instalasi apapun - semua sudah terpaket dalam aplikasi!

== CARA MENGGUNAKAN ==
1. Jalankan RJ_Auto_Metadata.exe
2. Masukkan API key Gemini anda di bagian "API Keys" (lihat API_Keys_Setup.txt)
3. Pilih folder input (berisi gambar yang akan diproses)
4. Pilih folder output (lokasi hasil gambar setelah diproses)
5. Atur pengaturan sesuai kebutuhan:
   - Rename Files: Aktifkan untuk mengganti nama file berdasarkan metadata
   - Workers: Jumlah proses paralel (3-5 direkomendasikan)
   - Delay: Waktu jeda antar batch dalam detik
6. Klik "Mulai Proses" untuk memulai

== KETERANGAN ==
- Aplikasi ini adalah versi portable dengan semua tools yang diperlukan sudah terpaket
- ExifTool sudah diintegrasikan dalam aplikasi - tidak perlu instalasi terpisah
- Aplikasi secara otomatis mengompresi gambar berukuran besar sebelum mengirim ke API
- Metadata disimpan dalam format EXIF untuk JPG/JPEG
- Hasil CSV disimpan di folder output/metadata_csv/
- File asli akan dihapus setelah berhasil diproses dan disalin ke folder output

== TROUBLE SHOOTING ==
- Jika muncul pesan "Exiftool tidak ditemukan", mohon pastikan aplikasi tidak dijalankan dari drive terkompresi atau folder yang memerlukan akses administrator
- "API Error": Periksa kembali API key atau coba lagi nanti (kemungkinan masalah kuota/rate limit)
- Jika aplikasi tidak merespons saat pemrosesan, gunakan tombol "Hentikan" lalu mulai ulang proses

== PERINGATAN PENTING ==
- SELALU BACKUP! Pastikan Anda memiliki salinan cadangan semua file asli sebelum diproses
- Aplikasi akan MENGHAPUS file asli dari folder input setelah berhasil diproses 
- Jika terjadi error atau kerusakan data selama pemrosesan, file asli mungkin hilang
- Proses ini tidak dapat dibatalkan, jadi gunakan HANYA SALINAN file, bukan file utama Anda

== TENTANG KOMPRESI OTOMATIS ==
- Kompresi hanya digunakan untuk PENGIRIMAN ke API Gemini, bukan untuk output akhir
- File output tetap mempertahankan kualitas asli (tidak dikompresi)
- Gambar besar (>5MB) dikompresi sementara hanya untuk mendapatkan metadata
- File yang dikompresi bersifat sementara dan otomatis dihapus setelah proses selesai
- Ini adalah optimasi kecepatan dan penghematan kuota API, bukan penghematan ruang disk

== KONTAK ==
Untuk bantuan lebih lanjut, bisa hubungi di:
https://s.id/eIUOr

© Riiicil 2025