Website Portofolio – PPW 2

Ini adalah tugas akhir JUDUL 2 Praktikum Pemrograman Web.

---

Cara Pembuatan

```bash
# Inisialisasi Git
git init

# Ubah nama branch utama menjadi 'main'
git branch -M main

# Commit awal (index.html, style.css, gambar, dan file pendukung)
git add .
git commit -m "menambahkan semua file"

# Commit penambahan animasi hover
git add .
git commit -m "tambahkan animasi hover pada tombol"

# Buat branch baru untuk eksperimen styling
git checkout -b styling-experiment

# Lakukan perubahan warna tema pada style.css
git add style.css
git commit -m "ubah tema dari coklat ke coklat muda"

# Kembali ke branch utama
git checkout main

# Gabungkan (merge) hasil eksperimen styling ke branch utama
git merge styling-experiment

# Tambahkan dokumen README
git add README.md
git commit -m "Dokumen readme"

# Hubungkan repository lokal dengan repository GitHub
git remote add origin https://github.com/nabilaputri04/ppw_2.git

# Push ke GitHub
git push -u origin main

# Push branch eksperimen styling
git push origin styling-experiment
```

---

Cara Penggunaan

1. Clone repository ini:

   ```bash
   git clone https://github.com/nabilaputri04/ppw_2.git
   ```

2. **Masuk ke direktori proyek:**

   ```bash
   cd ppw_2
   ```

3. Buka file `index.html`:
   Klik dua kali file `index.html` di folder untuk membukanya di browser.

---

Struktur Commit

Proses pengembangan website ini dilakukan secara bertahap agar setiap perubahan dapat dilacak dengan jelas melalui commit berikut:

```bash
$ git log --graph --oneline
* dfdf621 (HEAD -> main, origin/main, origin/styling-experiment, styling-experiment) ubah tema dari coklat ke coklat muda
* 323f74d tambahkan animasi hover pada tombol
* 0fc3d78 menambahkan semua file
* c1ac82a Initial commit
```

---

Branching dan Merging

Pengembangan fitur baru dilakukan melalui **branch eksperimental** agar tidak mengganggu versi utama.

- main → Berisi versi stabil dari website.
- styling-experiment → Digunakan untuk eksperimen perubahan tampilan (tema warna, animasi, dll).

Setelah proses pengujian dan revisi selesai, branch `styling-experiment` di-merge kembali ke `main` agar hasil akhirnya menjadi bagian dari versi utama proyek.
