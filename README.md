# Dasar Privasi — Period Tracker

Dasar privasi yang diterbitkan untuk aplikasi Android **Period Tracker**,
dwibahasa (Bahasa Melayu dan English).

Diterbitkan di **<https://azibbe.github.io/period-tracker-privacy/>**, dan URL
itu digunakan di dua tempat:

- Play Console → App content → Privacy policy
- Google Cloud Console → OAuth consent screen → App information

## Kenapa repo berasingan

GitHub Pages tidak melayan repo private pada pelan percuma, dan repo aplikasi
itu private. Repo ini awam supaya dasar privasi mempunyai URL yang boleh dicapai
sesiapa — termasuk penyemak Play dan pengguna yang menekan pautan itu dalam
skrin kebenaran Google.

## Sumber kebenaran

`docs/dasar-privasi.md` dalam repo aplikasi, bukan fail di sini. Ia duduk
bersebelahan kod yang ia perihalkan, supaya perubahan pada cara data dikendalikan
dan perubahan pada dasar berlaku dalam commit yang sama.

Untuk menerbitkan perubahan, jalankan `docs/hantar-privasi.sh` dari repo
aplikasi. Jangan sunting `index.md` di sini secara terus — ia akan ditulis ganti.
