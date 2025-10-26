# StudyGroup-MP-Motionlab

Untuk tugas di MotionLab

## Minggu ke-1 - Version Control (Git)

### Rangkuman

Version control adalah sistem yang digunakan untuk mengelola perubahan kode atau dokumen. Fungsinya antara lain:

1. **Mencatat riwayat perubahan**: Bisa melihat siapa yang mengubah apa, kapan, dan kenapa.
2. **Memudahkan kolaborasi**: Banyak orang bisa bekerja di satu proyek tanpa saling mengganggu.
3. **Mendukung workflow proyek**: Bisa membuat cabang (branch) untuk fitur baru, kemudian digabungkan (merge) setelah selesai.
4. **Backup otomatis**: Versi sebelumnya bisa dikembalikan jika terjadi kesalahan.

Git adalah salah satu version control yang paling populer. Git bersifat distributed, artinya setiap komputer memiliki salinan penuh dari repository.

---

## Cara Menggunakan Git

### 1. Instalasi

- **Windows**: [Git for Windows](https://git-scm.com/download/win)
- **macOS**: `brew install git`
- **Linux (Debian/Ubuntu)**: `sudo apt install git`

Setelah instalasi, lakukan konfigurasi awal:
```bash
git config --global user.name "Nama Anda"
git config --global user.email "email@anda.com"
```

### 2. Membuat Repository

Membuat repository baru di komputer:
```bash
git init
```

Menghubungkan dengan repository online (misal GitHub):
```bash
git remote add origin https://github.com/username/repo.git
```

### 3. Perintah Dasar Git

| Perintah | Fungsi |
|----------|--------|
| `git status` | Menampilkan status file yang berubah, belum di-commit, atau staged |
| `git add <file>` | Menambahkan file ke staging area untuk commit |
| `git commit -m "pesan"` | Menyimpan perubahan ke repository lokal |
| `git push` | Mengirim perubahan ke repository remote |
| `git pull` | Mengambil perubahan terbaru dari repository remote |
| `git log` | Melihat riwayat commit |
| `git branch` | Melihat daftar branch |
| `git checkout <branch>` | Pindah ke branch tertentu |
| `git merge <branch>` | Menggabungkan branch tertentu ke branch aktif |
| `git clone <url>` | Meng-copy repository remote ke komputer lokal |

### 4. Workflow Dasar

1. Clone repository dari GitHub:
```bash
   git clone https://github.com/username/repo.git
```

2. Buat branch baru untuk fitur:
```bash
   git checkout -b nama-fitur
```

3. Kerjakan perubahan, kemudian add dan commit:
```bash
   git add .
   git commit -m "Menambahkan fitur X"
```

4. Push branch ke remote:
```bash
   git push origin nama-fitur
```

5. Buat Pull Request di GitHub untuk merge ke branch utama (main/master).
