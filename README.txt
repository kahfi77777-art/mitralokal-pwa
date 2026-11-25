MITRALOKAL PWA - CARA MENJALANKAN

Isi folder:
- index.html: website MitraLokal
- manifest.webmanifest: identitas aplikasi PWA
- sw.js: service worker untuk cache/offline app shell
- icons/: ikon aplikasi 192px dan 512px

PENTING:
PWA memerlukan HTTPS atau localhost. Membuka index.html langsung melalui file:// tidak akan mengaktifkan instalasi PWA maupun service worker.

CARA UJI DI KOMPUTER:
1. Ekstrak ZIP.
2. Jalankan server lokal dari folder mitralokal-pwa, misalnya dengan Python:
   python -m http.server 8000
3. Buka http://localhost:8000 di Chrome.
4. Gunakan menu Chrome "Install app" atau tombol "Pasang aplikasi" jika tersedia.

CARA PASANG DI HP ANDROID:
1. Upload folder ini ke hosting HTTPS (contoh GitHub Pages, Netlify, atau Vercel).
2. Buka URL website yang sudah HTTPS melalui Chrome Android.
3. Pilih menu titik tiga > Tambahkan ke layar utama / Install app.

BATASAN VERSI INI:
- Warung, menu, dan harga masih data contoh.
- Service worker menyimpan app shell untuk membuka tampilan website offline; peta, WhatsApp, dan konten online tetap memerlukan internet.
- Formulir masih demo, belum tersambung ke database/backend.
