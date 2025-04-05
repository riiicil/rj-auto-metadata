# RJ Auto Metadata v1.0

Aplikasi Pemrosesan Metadata Gambar Otomatis (Portable Version). Aplikasi ini menggunakan AI untuk menghasilkan metadata berkualitas tinggi untuk gambar Anda dengan mengintegrasikan Gemini API dan ExifTool.

## Persyaratan
- Windows 10 atau lebih baru (64-bit)
- Koneksi internet untuk mengakses Gemini API
- Aplikasi portable; tidak diperlukan instalasi

## Cara Menggunakan
1. Jalankan `RJ_Auto_Metadata.exe`
2. Masukkan API key Gemini pada bagian **API Keys**  
   Lihat [API_Keys_setup.txt] untuk petunjuk detail.
3. Pilih folder input (berisi gambar yang akan diproses)
4. Pilih folder output (lokasi hasil gambar dan metadata)
5. Atur pengaturan sesuai kebutuhan:
   - **Rename Files:** Aktifkan untuk mengganti nama file berdasarkan metadata
   - **Workers:** Jumlah proses paralel (3-5 direkomendasikan)
   - **Delay:** Jeda antar batch (dalam detik)
6. Klik "Mulai Proses" untuk memulai

## Fitur Utama
- Pemrosesan metadata otomatis dengan Gemini API
- Penulisan metadata ke file EXIF (untuk JPG/JPEG)
- Ekspor metadata ke file CSV (folder output/metadata_csv/)
- Kompresi otomatis untuk gambar besar (hanya untuk pengiriman ke API)
- Multi-threading untuk pemrosesan batch yang cepat
- Penamaan file berbasis AI

## Setup ExifTool
Pastikan `exiftool.exe` berada dalam tools folder yang sama dengan `RJ_Auto_Metadata.exe` atau sesuai dengan petunjuk di [exiftools_setup.txt].

## Troubleshooting
Lihat [TROUBLESHOOTING.txt] untuk solusi masalah umum, misalnya:
- Aplikasi tidak dapat dijalankan
- ExifTool tidak ditemukan
- API error atau "Maximum retries exceeded"
- Masalah saat menulis EXIF atau output rusak

## Catatan Penting
- **Backup File:** Selalu gunakan salinan gambar, bukan file asli, karena aplikasi menghapus file input setelah pemrosesan berhasil.
- **Kompresi:** Gambar besar dikompresi hanya sementara untuk pengiriman ke API; file output tetap mempertahankan kualitas asli.
- **Keamanan Data:** Jangan gunakan folder dengan file penting sebagai folder input.

## Kontak
Untuk bantuan lebih lanjut, bisa kunjungi: [https://s.id/eIUOr](https://s.id/eIUOr)

© Riiicil 2025