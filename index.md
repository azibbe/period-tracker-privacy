<!--
  Published at https://azibbe.github.io/period-tracker-privacy/ and pasted into
  both Play Console and the Google OAuth consent screen.

  This repo exists only because GitHub Pages will not serve a private
  repository on the free plan, and the app's own repo is private. The source of
  truth is docs/dasar-privasi.md in azibbe/period-tracker — edit it there and
  run docs/hantar-privasi.sh, so the policy cannot drift away from the code it
  describes.
-->

# Dasar Privasi — Period Tracker

Dikemas kini: 13 Ogos 2026

## Ringkasan

Period Tracker menyimpan semua rekod kitaran haid anda **di dalam peranti
anda sahaja**. Tiada akaun diperlukan. Tiada pelayan. Tiada pengiklanan, tiada
analitik, dan tiada penjejakan.

Satu-satunya masa aplikasi ini menyambung ke internet ialah apabila **anda
sendiri** menekan butang backup ke Google Drive. Kalau anda tidak pernah
menekan butang itu, aplikasi ini tidak pernah menghantar apa-apa keluar dari
telefon anda.

## Data yang disimpan dalam peranti anda

Aplikasi menyimpan perkara berikut dalam storan peribadi aplikasi, yang tidak
boleh dibaca oleh aplikasi lain:

- Tarikh mula dan tamat setiap haid yang anda rekodkan
- Log harian: aliran, simptom, mood, tahap tenaga, dan nota anda
- Tetapan kitaran (panjang kitaran, fasa luteal)
- Tetapan aplikasi: bahasa, tema, pilihan peringatan
- PIN kunci aplikasi, jika anda menetapkannya

PIN disimpan dalam storan yang dienkripsi oleh sistem Android (Android
Keystore). Rekod kitaran itu sendiri disimpan sebagai fail JSON biasa dalam
storan peribadi aplikasi — ia dilindungi oleh sandbox Android, tetapi **tidak
dienkripsi secara berasingan**. Sesiapa yang mempunyai akses penuh (root) ke
telefon anda boleh membacanya.

## Peringatan

Semua peringatan dijadualkan dan dipaparkan oleh peranti anda sendiri. Tiada
apa-apa dihantar melalui internet untuk menghasilkan peringatan.

Jika anda menghidupkan "Notifikasi diskret", teks peringatan tidak menyebut
apa-apa yang spesifik. Perlu diingat: Android tetap memaparkan nama aplikasi
("Period Tracker") pada setiap notifikasi, dan itu tidak dapat kami sembunyikan.

## Google Drive (pilihan)

Jika — dan hanya jika — anda memilih untuk menyambung Google Drive:

- Kami meminta skop `drive.appdata` sahaja. Skop ini memberi akses kepada satu
  folder tersembunyi khusus untuk aplikasi ini di dalam Drive **anda sendiri**.
  Kami tidak boleh melihat, membaca, atau mengubah mana-mana fail lain dalam
  Drive anda.
- Fail backup disimpan dalam folder tersembunyi itu. Ia tidak kelihatan dalam
  antara muka Drive dan tidak boleh dibaca oleh aplikasi lain.
- Alamat e-mel Google anda dipaparkan dalam skrin Backup supaya anda tahu akaun
  mana yang sedang bersambung. Ia tidak disimpan di mana-mana selain sesi
  aplikasi.
- Anda boleh memutuskan sambungan pada bila-bila masa. Memutuskan sambungan
  tidak memadam rekod kitaran anda — rekod itu tidak pernah terikat kepada akaun
  Google anda.

Data yang diperoleh melalui Google API digunakan semata-mata untuk fungsi backup
yang anda minta, dan tidak dipindahkan kepada mana-mana pihak ketiga.

## Perkongsian data

Kami **tidak** berkongsi, menjual, atau memindahkan data anda kepada sesiapa.
Tiada pihak ketiga menerima apa-apa daripada aplikasi ini. Tiada SDK analitik,
tiada rangkaian iklan, tiada alat pelaporan ranap.

## Menghapuskan data anda

- Nyahpasang aplikasi, atau
- Tetapan Android → Aplikasi → Period Tracker → Storan → Kosongkan data

Kedua-duanya memadam semua rekod dalam peranti secara kekal. Jika anda pernah
membuat backup ke Google Drive, padamkannya melalui
[Drive → Tetapan → Urus Apl](https://drive.google.com/drive/settings).

## Ramalan bukan nasihat perubatan

Ramalan dalam aplikasi ini adalah anggaran statistik daripada sejarah yang anda
rekodkan sendiri. Ia **bukan kaedah perancang keluarga** dan **bukan nasihat
perubatan**. Rujuk profesional kesihatan untuk sebarang kebimbangan.

## Kanak-kanak

Aplikasi ini tidak ditujukan kepada kanak-kanak di bawah 13 tahun dan kami tidak
mengumpul apa-apa data daripada mereka secara sedar.

## Perubahan

Sebarang perubahan kepada dasar ini akan dikemas kini di halaman ini, berserta
tarikh baharu di atas.

## Hubungi

syarumie@gmail.com

---

# Privacy Policy — Period Tracker (English)

Last updated: 13 August 2026

## Summary

Period Tracker keeps every cycle record **on your device only**. No account is
required. There is no server, no advertising, no analytics, and no tracking.

The only time this app connects to the internet is when **you** press the button
to back up to Google Drive. If you never press it, nothing ever leaves your
phone.

## Data stored on your device

The app stores the following in its private app storage, which other apps
cannot read:

- The start and end date of every period you record
- Daily logs: flow, symptoms, mood, energy level, and your notes
- Cycle settings (cycle length, luteal phase)
- App settings: language, theme, reminder preferences
- The app-lock PIN, if you set one

The PIN is held in storage encrypted by Android's own Keystore. The cycle
records themselves are stored as a plain JSON file in the app's private storage
— protected by the Android sandbox, but **not separately encrypted**. Anyone
with full (root) access to your phone can read it.

## Reminders

All reminders are scheduled and shown by your own device. Nothing is sent over
the internet to produce a reminder.

If you turn on "Discreet notifications", the reminder text says nothing
specific. Note that Android always displays the app's name ("Period Tracker") on
every notification, and that is not something we can hide.

## Google Drive (optional)

If — and only if — you choose to connect Google Drive:

- We request the `drive.appdata` scope and nothing wider. It grants access to a
  single hidden folder belonging to this app inside **your own** Drive. We
  cannot see, read, or change any other file in your Drive.
- The backup file is stored in that hidden folder. It does not appear in the
  Drive interface and cannot be read by other apps.
- Your Google email address is shown on the Backup screen so you know which
  account is connected. It is not stored anywhere beyond the app session.
- You can disconnect at any time. Disconnecting does not delete your cycle
  records — they were never tied to your Google account.

Data obtained through Google APIs is used solely for the backup function you
asked for, and is not transferred to any third party.

## Data sharing

We do **not** share, sell, or transfer your data to anyone. No third party
receives anything from this app. There is no analytics SDK, no ad network, and
no crash-reporting tool.

## Deleting your data

- Uninstall the app, or
- Android Settings → Apps → Period Tracker → Storage → Clear data

Either removes every on-device record permanently. If you ever backed up to
Google Drive, delete it via
[Drive → Settings → Manage Apps](https://drive.google.com/drive/settings).

## Predictions are not medical advice

The forecasts in this app are a statistical estimate from the history you record
yourself. They are **not a method of contraception** and **not medical advice**.
Consult a health professional with any concerns.

## Children

This app is not directed at children under 13 and we do not knowingly collect
any data from them.

## Changes

Any change to this policy will be published on this page, with a new date at the
top.

## Contact

syarumie@gmail.com
