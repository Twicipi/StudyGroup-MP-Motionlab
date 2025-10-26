# StudyGroup-MP-Motionlab
Untuk tugas di MotionLab

Minggu ke- 1 - Version Control (Git)
Rangkuman : Version control adalah sistem yang digunakan untuk mengelola perubahan kode atau dokumen. Fungsinya antara lain:
1. Mencatat riwayat perubahan: Bisa melihat siapa yang mengubah apa, kapan, dan kenapa.
2. Memudahkan kolaborasi: Banyak orang bisa bekerja di satu proyek tanpa saling mengganggu.
3. Mendukung workflow proyek: Bisa membuat cabang (branch) untuk fitur baru, kemudian digabungkan (merge) setelah selesai.
4. Backup otomatis: Versi sebelumnya bisa dikembalikan jika terjadi kesalahan.
Git adalah salah satu version control yang paling populer. Git bersifat distributed, artinya setiap komputer memiliki salinan penuh dari repository.

Cara Menggunakan Git
1. Instalasi
Untuk Windows: Git for Windows
Untuk macOS: brew install git
Untuk Linux (Debian/Ubuntu): sudo apt install git
Setelah instalasi, konfigurasi awal:
git config --global user.name "Nama Anda"
git config --global user.email "email@anda.com"
2. Membuat Repository
Membuat repository baru di komputer:
git init
Menghubungkan dengan repository online (misal GitHub):
git remote add origin https://github.com/username/repo.git

3. Perintah Dasar Git
Perintah	Fungsi
git status	Menampilkan status file yang berubah, belum di-commit, atau staged
git add <file>	Menambahkan file ke staging area untuk commit
git commit -m "pesan"	Menyimpan perubahan ke repository lokal
git push	Mengirim perubahan ke repository remote
git pull	Mengambil perubahan terbaru dari repository remote
git log	Melihat riwayat commit
git branch	Melihat daftar branch
git checkout <branch>	Pindah ke branch tertentu
git merge <branch>	Menggabungkan branch tertentu ke branch aktif
git clone <url>	Meng-copy repository remote ke komputer lokal

4. Workflow Dasar
  1. Clone repository dari GitHub:
  git clone https://github.com/username/repo.git
  2. Buat branch baru untuk fitur:
  git checkout -b nama-fitur
  3. Kerjakan perubahan, kemudian add dan commit:
  git add .
  git commit -m "Menambahkan fitur X"
  5. Push branch ke remote:
  git push origin nama-fitur
  6. Buat Pull Request di GitHub untuk merge ke branch utama (main/master).
