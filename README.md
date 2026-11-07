# Dokumentasi Workshop Day 1: From AI to GitHub

Repositori ini memuat catatan, dokumentasi, dan refleksi pembelajaran kegiatan **Workshop Day 1: "From AI to GitHub"**. Seluruh berkas disusun untuk memenuhi tugas dokumentasi harian peserta workshop.

---

## 📌 Identitas Peserta
- **Nama Lengkap:** Dimas Sakti Satarsyah
- **Kelompok:** 8-Persona
- **Kegiatan:** Workshop Day 1 – Proyek Workshop
- **Topik Workshop:** From AI to GitHub

---

## 📖 Deskripsi & Tujuan Repositori

### Deskripsi Singkat
Repositori ini berfungsi sebagai wadah dokumentasi komprehensif atas materi yang dipelajari dan dipraktikkan pada Day 1 Workshop. Berisi rangkuman materi mulai dari dasar *Prompt Engineering* yang efektif, pemahaman fundamental perbedaan Git dan GitHub, konfigurasi lingkungan kerja lokal, hingga pembuatan aplikasi web nyata dengan bantuan AI.

### Tujuan dan Kegunaan
1. **Penyimpanan Dokumentasi Terpusat:** Menyimpan ringkasan materi, catatan teknis, dan alur kerja (*workflow*) yang dipelajari selama workshop secara rapi dan terstruktur.
2. **Portofolio & Rekam Jejak Belajar:** Menjadi bukti autentik pemahaman konsep dasar *version control* dan pemanfaatan AI dalam pengembangan perangkat lunak.
3. **Referensi Teknis Mandiri:** Menjadi rujukan cepat untuk konfigurasi Git, SSH, maupun teknik pemberian instruksi (*prompting*) pada proyek-proyek mendatang.

---

## 📚 Rangkuman Materi Workshop

Materi Workshop Day 1 difokuskan pada pengenalan pemanfaatan AI secara terarah serta pengenalan dasar *version control system* (VCS) untuk pemula:

### 1. Seni Merancang Prompt (*Prompt Engineering*)
Kualitas hasil dari AI sangat ditentukan oleh bagaimana instruksi dirumuskan. Prompt yang singkat atau ambigu (misalnya sekadar *"Create student task planner"*) hanya akan menghasilkan aplikasi yang umum dan kurang relevan. Prompt yang efektif dibangun dari kerangka **4 Unsur Kunci**:
- **Role (Peran):** Mendefinisikan persona AI (misal: *Senior Front-End Developer*).
- **Task (Tujuan/Tugas):** Menyatakan secara spesifik apa yang harus dibangun atau diselesaikan.
- **Context (Konteks):** Memberikan batasan teknis, kebutuhan pengguna, atau aturan khusus.
- **Format (Bentuk Output):** Menentukan format respons (misal: kode terpisah HTML, CSS, dan JS).

> **Prinsip Penting:** Menyertakan instruksi penutup agar AI **tidak mengklaim aplikasi telah berfungsi** sebelum perilakunya diverifikasi. Pengembang harus tetap memvalidasi dan menguji hasil yang diberikan oleh AI.

---

### 2. Fundamental Git vs GitHub
Sering kali pemula menyamakan Git dan GitHub, padahal keduanya memiliki peran berbeda:
- **Git:** Alat pengendali versi (*Version Control System*) yang terinstal di komputer lokal. Git bertugas melacak riwayat perubahan berkas, siapa yang mengubah, kapan diubah, serta memungkinkan pengelolaan *branching*.
- **GitHub:** Platform berbasis *cloud* (daring) untuk menyimpan repositori Git jarak jauh (*remote repository*), mempermudah kolaborasi antartim, manajemen isu (*issue tracking*), dan peninjauan kode (*code review*).

---

### 3. Alur Kerja Dasar Git (*Git Core Workflow*)
Perubahan berkas dikelola melalui tiga area utama sebelum diunggah ke internet:
1. **Working Directory:** Area kerja lokal tempat menulis dan memodifikasi berkas kode.
2. **Staging Area (`git add`):** Titik pemilihan berkas mana saja yang siap disimpan ke dalam riwayat perubahan.
3. **Local Repository (`git commit`):** Perekaman snapshot riwayat perubahan secara permanen di komputer lokal disertai pesan *commit* yang jelas.
4. **Remote Repository (`git push`):** Proses pengiriman commit dari repositori lokal ke repositori daring (GitHub).

```
[ Working Directory ]  --->  git add  --->  [ Staging Area ]  --->  git commit  --->  [ Local Repo ]  --->  git push  --->  [ GitHub ]
```

---

### 4. Persiapan Lingkungan Kerja (*Development Setup*)
Langkah-langkah penyiapan komputer sebelum mulai bekerja:
- Memasang perangkat lunak utama: **Git** dan editor kode **VS Code**.
- Mengonfigurasi identitas global Git:
  ```bash
  git config --global user.name "Dimas Sakti Satarsyah"
  git config --global user.email "email-anda@example.com"
  ```
- Menghubungkan autentikasi dengan **SSH Key**:
  1. Menghasilkan pasangan kunci SSH (`ssh-keygen -t ed25519`).
  2. Mendaftarkan kunci publik (*public key*) ke akun GitHub pada menu **Settings > SSH and GPG keys**.
  3. Memvalidasi koneksi menggunakan perintah:
     ```bash
     ssh -T git@github.com
     ```

---

### 5. Praktik Proyek: *Student Task Planner*
Peserta mempraktikkan alur kerja lengkap dari hulu ke hilir:
- Menulis prompt terstruktur ke AI untuk membuat aplikasi perencana tugas siswa (*Student Task Planner*) berbasis HTML, CSS, dan JavaScript.
- Menginisialisasi repositori lokal dengan `git init`.
- Melakukan *staging* dan *commit* awal terhadap berkas kode.
- Mengunggah repositori ke GitHub dengan `git push`.
- Memodifikasi kode, menguji perubahan, dan melakukan *commit* serta *push* ulang untuk melihat riwayat perubahan versi (*commit history*).

---

## 💡 Poin-Poin Penting & Pengetahuan Baru

1. **AI sebagai Asisten, Bukan Pengambil Keputusan Penuh:** Kualitas keluaran AI bergantung pada presisi instruksi kita. Sikap kritis untuk selalu menguji fungsionalitas kode sebelum menganggapnya selesai adalah kebiasaan baik seorang pengembang.
2. **Pemisahan Jelas Git dan GitHub:** Memahami bahwa Git tetap dapat berjalan sepenuhnya secara luring di laptop tanpa koneksi internet, sementara GitHub adalah media berbagi dan kolaborasi.
3. **Disiplin dalam Commit:** Membiasakan diri melakukan commit dengan pesan yang deskriptif dan alur yang teratur (`add` -> `commit` -> `push`).
4. **Keamanan Autentikasi Modern via SSH:** Memahami cara kerja pasangan kunci publik dan privat untuk autentikasi yang aman dan praktis tanpa harus memasukkan kata sandi berulang kali.

---

## 💭 Pendapat & Refleksi Pribadi tentang Day 1

Materi pada Day 1 Workshop ini sangat menyenangkan dan mudah diikuti, terutama bagi saya yang saat ini masih berada di semester 1. 

Hal yang paling membuka wawasan saya adalah konsep mengenai *Prompt Engineering*. Selama ini, saya terbiasa memberikan perintah singkat seperti *"buatin aplikasi ini"* ke AI dan sering merasa heran mengapa hasilnya sangat biasa atau generik. Setelah mempelajari kerangka peran (*Role*), tujuan (*Task*), konteks (*Context*), dan format (*Format*), hasil yang diperoleh jauh lebih tepat sasaran. Pesan penutup pada prompt yang melarang AI mengklaim sukses sebelum diuji juga menjadi pengingat berharga agar tidak menelan mentah-mentah hasil keluaran AI.

Selain itu, materi Git dan GitHub sangat membantu memperjelas konsep yang sebelumnya membingungkan. Sekarang saya mengerti bahwa Git adalah alat pelacaknya di komputer, sedangkan GitHub adalah wadah penyimpanannya di awan. Meskipun proses konfigurasi SSH key sempat cukup rumit dan membuat pusing di awal, kepuasan ketika koneksi berhasil divalidasi dengan `Hi Dimas Sakti Satarsyah! You've successfully authenticated...` memberikan dorongan semangat besar untuk melanjutkan ke sesi-sesi workshop berikutnya.

---

*Disusun oleh Dimas Sakti Satarsyah – Kelompok 8-Persona | Day 1 Workshop*
