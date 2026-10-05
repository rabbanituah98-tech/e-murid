# e-Murid

Apps web daftar murid sekolah untuk kegunaan guru: carian pantas, butiran penuh murid dan penjaga, catatan bertarikh, tanda warna, mod siang/malam, import dan eksport Excel.

**Senarai murid di dalam `index.html` disulitkan (AES-256-GCM, kunci PBKDF2 600,000 pusingan).** Tanpa kata laluan data, isinya tidak boleh dibaca. Jangan tulis kata laluan di mana-mana dalam repo ini, dan jangan muat naik fail Excel murid ke sini. Selepas dibuka, data, catatan dan suntingan disimpan dalam peranti pengguna sahaja.

## Fail

| Fail | Fungsi |
| --- | --- |
| `index.html` | Keseluruhan apps (satu fail, tanpa CDN) |
| `apple-touch-icon.png` | Ikon skrin utama iPhone |
| `icon-192.png`, `icon-512.png` | Ikon untuk Android / pelayar |
| `manifest.webmanifest` | Tetapan apps skrin utama |
| `sw.js` | Membolehkan apps dibuka tanpa internet |

## Terbitkan di GitHub Pages

1. Cipta repo baharu (contoh: `emurid`) dan muat naik semua fail di atas ke akar repo.
2. Settings → Pages → Source: **Deploy from a branch** → Branch: `main` / `(root)` → Save.
3. Tunggu seminit, kemudian buka `https://<nama-pengguna>.github.io/emurid/`.

## Letak pada skrin utama iPhone

1. Buka pautan di atas dalam **Safari**.
2. Tekan butang **Kongsi** → **Add to Home Screen** → **Add**.
3. Buka apps daripada ikon itu, kemudian masukkan **kata laluan data** (sekali sahaja bagi setiap peranti).

Data ikon skrin utama disimpan berasingan daripada Safari, jadi masukkan kata laluan selepas apps dibuka daripada ikon. Simpan sandaran dari semasa ke semasa melalui Data dan tetapan → Simpan sandaran.
