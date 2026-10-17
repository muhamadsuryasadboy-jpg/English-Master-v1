# English Master

Aplikasi belajar bahasa Inggris untuk pelajar Indonesia (Pre-A1 sampai C1). Satu berkas `index.html` + Capacitor 6, dibuild jadi APK debug oleh GitHub Actions.

## Cara membuat APK (dari HP lewat browser)
1. Buka github.com, buat **repo baru** (jangan pakai ulang repo aplikasi lain), misalnya `english-master`.
2. Upload semua isi folder ini ke repo: `index.html`, `package.json`, `capacitor.config.json`, `icon-*.png`, `splash*.png`, `.gitignore`, folder `data/`, dan **`.github/workflows/build-apk.yml`** (folder tersembunyi, pastikan terupload).
3. Buka tab **Actions**, pilih **Build APK**, tekan **Run workflow**. Tunggu ±5-10 menit sampai hijau.
4. Buka run yang selesai, gulir ke **Artifacts**, unduh **EnglishMaster-apk** (zip), ekstrak, lalu pasang `EnglishMaster.apk`. Izinkan "pasang dari sumber tidak dikenal" jika diminta.

Ini APK *debug* (cukup untuk pemakaian pribadi), bukan untuk Play Store.

## Isi
- 3.304 kosakata bawaan, 20 kategori (`data/kosakata.tsv` adalah salinan datanya; data yang dipakai aplikasi sudah tertanam di `index.html`). Tambah kata sendiri lewat Kosakata > Tambah kata.
- 20 materi grammar, 15 bacaan, 66 soal tes penempatan, 24 tugas menulis.
- Jalur belajar otomatis ala Duolingo (601 langkah, 42 bagian, terbuka satu per satu) di tab Belajar.
- Terjemah ketuk kata (susun kata seperti Duolingo, dua arah dengan kata pengecoh) dan Latihan kosakata.
- Jadwal ulang 1-2-4-7-14-30 hari yang adaptif, halaman Bukti Hafal, XP, streak, misi, pencapaian, mode gelap.
- AI Tutor opsional dengan kunci API milikmu sendiri (Gemini, Groq, OpenRouter, OpenAI, atau kompatibel OpenAI). Tanpa AI semua fitur lain tetap jalan.

## Batasan yang jujur
- Arti, IPA, dan panduan pelafalan ditulis dengan bantuan AI dan belum diperiksa kamus/penerjemah manusia.
- Hasil tes penempatan adalah perkiraan, bukan nilai CEFR resmi.
- Suara memakai Text-to-speech bawaan HP; pengenalan suara untuk Speaking hanya jika didukung perangkat.
- Penulisan tanpa AI hanya dicek jumlah kata dan frasa kunci.
- Data hanya tersimpan di perangkat. Buat backup dari Profil > Backup.
- APK belum diuji di perangkat Android nyata oleh pembuatnya; build dilakukan GitHub Actions di akunmu.
