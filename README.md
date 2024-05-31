# Location Taker

Proyek ini menangkap geolokasi pengguna dan informasi perangkat kemudian mengirimkannya ke URL skrip Google Sheets yang ditentukan.

## Instruksi Penggunaan

### Persiapan URL Spreadsheet

1. Kunjungi repositori berikut untuk mendapatkan URL Spreadsheet:
   [Form to Google Sheets](https://github.com/jamiewilson/form-to-google-sheets)

2. Buat tabel seperti gambar berikut, sesuaikan dengan kodingan form yang digunakan atau sesuai permintaan Anda:
![image](https://github.com/anggeryoga/location-take/assets/139601862/b1073a15-7c8e-4fac-9f31-7795d1339cda)
| Command | Description |
| --- | --- |
| `git status` | List all *new or modified* files |
| `git diff` | Show file differences that **haven't been** staged |

### Cara Penggunaan

1. Clone repository ke komputer lokal Anda:

    ```sh
    git clone https://github.com/your-username/location-taker.git
    cd location-taker
    ```

2. Buka `index.html` di peramban web Anda.

3. Ketika halaman dimuat, pengguna akan diminta untuk mengizinkan akses lokasi. Jika pengguna memberikan izin, langkah-langkah berikut akan terjadi:
   - Geolokasi pengguna (lintang dan bujur) akan ditangkap.
   - Informasi perangkat seperti string user agent akan dikumpulkan.

4. Data yang ditangkap kemudian akan dikirim secara otomatis ke URL skrip Google Sheets yang telah ditentukan.

### Catatan Penting

- Pastikan peramban mendukung geolokasi. Sebagian besar peramban modern mendukung fitur ini, tetapi beberapa mungkin memerlukan HTTPS agar layanan geolokasi dapat berfungsi.
- Pengguna harus memberikan izin untuk mengakses lokasi mereka. Jika izin ditolak, data lokasi tidak akan ditangkap dan pesan kesalahan akan dicatat di konsol.

### Troubleshooting

- Jika lokasi tidak bisa diambil, pastikan pengaturan lokasi di perangkat pengguna sudah diaktifkan.
- Jika data tidak terkirim ke Google Sheets, cek kembali URL skrip yang digunakan dan pastikan tabel di Google Sheets sesuai dengan data yang dikirim.

---
