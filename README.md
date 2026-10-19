# Bot Automasi Data Jaringan FTTH/FTTX

Bot Telegram berbasis Python yang dikembangkan dalam konteks kegiatan magang di PT Telkom Akses/Telkom untuk membantu proses pencarian dan validasi informasi jaringan FTTH/FTTX. Proyek ini mengeksplorasi pemanfaatan bot percakapan dan integrasi API agar akses data operasional dapat dilakukan melalui alur yang lebih praktis.

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Telegram Bot API](https://img.shields.io/badge/Telegram_Bot_API-26A5E4?style=for-the-badge&logo=telegram&logoColor=white)
![Google API](https://img.shields.io/badge/Google_API-4285F4?style=for-the-badge&logo=google&logoColor=white)

## Daftar Isi
- [Latar Belakang](#latar-belakang)
- [Tujuan Proyek](#tujuan-proyek)
- [Solusi yang Dikembangkan](#solusi-yang-dikembangkan)
- [Fitur dan Alur Kerja](#fitur-dan-alur-kerja)
- [Teknologi](#teknologi)
- [Gambaran Arsitektur](#gambaran-arsitektur)
- [Manfaat](#manfaat)
- [Batasan dan Catatan](#batasan-dan-catatan)
- [Pengembangan Selanjutnya](#pengembangan-selanjutnya)
- [Peran dan Konteks Proyek](#peran-dan-konteks-proyek)

## Latar Belakang
Pengecekan informasi jaringan dan pencatatan data operasional dapat melibatkan pencarian manual pada sumber data yang berbeda. Proyek ini dirancang untuk menyederhanakan akses informasi tertentu melalui Telegram, dengan memanfaatkan Python dan layanan Google API.

## Tujuan Proyek
- Mempermudah pencarian informasi jaringan yang diperlukan dalam proses operasional.
- Mengurangi langkah manual saat mengambil atau memvalidasi data.
- Menghubungkan antarmuka Telegram dengan sumber data berbasis layanan Google.
- Mengeksplorasi otomasi sederhana untuk mendukung pekerjaan teknis dan administrasi jaringan.

## Solusi yang Dikembangkan
Bot bertindak sebagai antarmuka percakapan. Pengguna mengirim permintaan melalui Telegram, logika Python memproses permintaan tersebut, lalu integrasi API digunakan untuk mengakses sumber data yang telah dikonfigurasi.

## Fitur dan Alur Kerja
Berdasarkan dokumentasi proyek, cakupan fungsi yang dituju meliputi:
- **Pencarian informasi jaringan:** membantu pencarian data terkait infrastruktur FTTH/FTTX, seperti ODP, STO, dan informasi ketersediaan port apabila tersedia pada sumber data yang terhubung.
- **Integrasi sumber data:** menggunakan Google Sheets API dan Google Drive API sesuai kebutuhan alur kerja.
- **Pemrosesan melalui bot:** menerima permintaan melalui Telegram dan memprosesnya menggunakan Python.
- **Pencatatan aktivitas:** mendukung pencatatan atau sinkronisasi informasi sesuai implementasi yang dikonfigurasi.

## Teknologi
| Teknologi | Peran |
|---|---|
| Python 3 | Logika dan pemrosesan aplikasi |
| Telegram Bot API | Antarmuka interaksi pengguna |
| Google Sheets API | Akses data spreadsheet |
| Google Drive API | Integrasi dengan sumber daya Google Drive |
| `python-telegram-bot` | Membantu pengembangan bot Telegram |
| `gspread` | Interaksi dengan Google Sheets |
| `oauth2client` | Dukungan autentikasi Google API pada konfigurasi yang digunakan |
| `pandas` | Pengolahan data tabular bila diperlukan |

## Gambaran Arsitektur
1. Pengguna mengirim permintaan melalui Telegram.
2. Bot menerima pesan dan meneruskannya ke logika Python.
3. Aplikasi memproses permintaan dan mengakses sumber data melalui API yang dikonfigurasi.
4. Hasil pemrosesan dikirim kembali melalui Telegram.

```text
Pengguna
   |
   v
Telegram
   |
   v
Bot Telegram (Python)
   |
   +------> Google Sheets API
   |
   +------> Google Drive API
   |
   v
Hasil pemrosesan dikirim kembali ke pengguna
```

## Manfaat
- Membantu memusatkan akses ke informasi yang dibutuhkan melalui satu antarmuka.
- Berpotensi mengurangi langkah pencarian manual dan risiko kesalahan saat menyalin data.
- Memberikan pengalaman akses data yang lebih praktis bagi pengguna operasional.

Efisiensi numerik tertentu belum dicantumkan sebagai hasil terverifikasi dalam dokumentasi ini. Klaim seperti persentase penghematan waktu sebaiknya ditambahkan hanya jika tersedia catatan pengukuran atau pembandingan yang dapat dijelaskan.

## Batasan dan Catatan
- Hasil bot bergantung pada ketersediaan, struktur, dan izin akses sumber data.
- Kredensial API dan token bot tidak boleh disimpan di repository publik.
- Informasi jaringan internal atau data operasional sensitif tidak boleh ditampilkan dalam screenshot atau contoh penggunaan.
- Repository ini saat ini berisi dokumentasi ringkasan proyek. Source code yang telah disanitasi, contoh konfigurasi, serta bukti demonstrasi dapat ditambahkan untuk membantu pembaca memahami implementasi secara lebih menyeluruh.

## Pengembangan Selanjutnya
- Menambahkan source code yang sudah disanitasi dari token, kredensial, dan informasi internal.
- Menyediakan file contoh konfigurasi seperti `.env.example` tanpa nilai rahasia.
- Menambahkan diagram arsitektur dan screenshot demonstrasi dengan data dummy.
- Mendokumentasikan perintah bot, penanganan kesalahan, serta langkah instalasi setelah implementasi diverifikasi.
- Menambahkan evaluasi efisiensi berdasarkan pengukuran yang dapat dipertanggungjawabkan.


## Pengembang: Sela Putri Ismalia  

