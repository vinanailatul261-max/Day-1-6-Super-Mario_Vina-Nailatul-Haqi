# Day-1-6-Super-Mario_Vina-Nailatul-Haqi

# Dokumentasi Workshop – Day 1

**Building with AI, Managing Change with GitHub**

| | |
|---|---|
| **Nama Lengkap** | Vina Nailatul Haqi |
| **Kelas** | TMD 1B – D4 Teknik Multimedia dan Digital |
| **Kampus** | Politeknik Negeri Jakarta (PNJ) |

---

## Daftar Isi

1. [Deskripsi Repository](#-deskripsi-repository)
2. [Tujuan Repository](#-tujuan-repository)
3. [Informasi Kegiatan Workshop](#-informasi-kegiatan-workshop)
4. [Rangkuman Materi](#-rangkuman-materi)
   - [Sesi 1 – Building with AI, Managing Change with GitHub](#sesi-1--building-with-ai-managing-change-with-github)
   - [Sesi 2 – Kurikulum Merdeka di Perguruan Tinggi (MBKM & MSIB)](#sesi-2--kurikulum-merdeka-di-perguruan-tinggi-mbkm--msib)
   - [Sesi 3 – Paparan Kurikulum OBE 2026 D4 Teknik Informatika](#sesi-3--paparan-kurikulum-obe-2026-d4-teknik-informatika)
5. [Poin Penting & Pengetahuan Baru](#-poin-penting--pengetahuan-baru)
6. [Pendapat Pribadi tentang Day 1](#-pendapat-pribadi-tentang-day-1)
7. [Referensi](#-referensi)

---

## Deskripsi Repository

Repository ini adalah dokumentasi pribadi saya selama mengikuti **Day 1 Proyek Workshop**. Isinya berupa rangkuman materi yang disampaikan, catatan hal-hal baru yang saya pelajari, dan pendapat saya tentang jalannya kegiatan. Seluruh dokumentasi ditulis dalam satu file `README.md` supaya mudah dibaca langsung di halaman utama repository.

## Tujuan Repository

- Menyimpan dan merapikan catatan materi workshop di satu tempat yang bisa diakses secara daring.
- Melatih saya memakai GitHub untuk menyimpan, mengelola, dan mempublikasikan dokumentasi.
- Membiasakan diri mendokumentasikan hal yang dipelajari, bukan hanya mengikutinya.
- Melatih penulisan catatan terstruktur dengan Markdown (`README.md`).
- Menjadi bahan membaca ulang saya sendiri, dan acuan bagi orang lain yang ingin tahu isi Day 1.

## Informasi Kegiatan Workshop

| Keterangan | Detail |
|---|---|
| **Nama kegiatan** | Proyek Workshop – Day 1 |
| **Tema sesi praktik** | Building with AI, Managing Change with GitHub |
| **Pemateri sesi AI & GitHub** | Nugi Farhan (Senior Product Designer, pengalaman 6 tahun) |
| **Materi pendukung** | Kurikulum Merdeka (MBKM & MSIB); Kurikulum OBE 2026 D4 Teknik Informatika PNJ |
| **Pemateri paparan kurikulum** | Bambang Warsuta, S.Kom., M.T.I. (Kepala Program Studi D4 TI PNJ) |
| **Jenis tugas** | Individu – dokumentasi di repository GitHub Public |

**Capaian yang ditargetkan pada sesi AI & GitHub:**

1. Menjelaskan bagaimana prompt AI yang lebih spesifik menghasilkan hasil yang lebih baik.
2. Mengidentifikasi *repository*, *commit*, *branch*, dan *pull request*.
3. Membedakan Git dan GitHub.
4. Melakukan *version controlling*.

---

## Rangkuman Materi

### Sesi 1 – Building with AI, Managing Change with GitHub

Sesi ini terdiri dari dua bagian besar: **Prompt Engineering** (cara memberi instruksi ke AI) dan **Git & GitHub** (cara mengelola perubahan kode), lalu ditutup dengan praktik membuat aplikasi sederhana.

#### A. Prompt Engineering

**Apa itu prompt?** Instruksi atau masukan yang kita berikan ke model AI untuk mendapatkan hasil tertentu. Bentuknya bisa pertanyaan sederhana, kata kunci, instruksi yang rumit, atau potongan kode.

**Prompt engineering** adalah cara merancang instruksi agar AI memberi jawaban yang tepat, relevan, dan layak dipakai.

**Context is key.** Prompt tanpa konteks membuat AI menebak-nebak. Prompt yang memuat konteks (siapa penggunanya, batasan teknologinya, hasil yang diharapkan) menghasilkan jawaban yang jauh lebih terarah.

**Struktur prompt yang baik: Role – Task – Context – Format**

| Unsur | Fungsi | Contoh dari materi (Student Task Planner) |
|---|---|---|
| **Role** | Menetapkan peran AI | "Kamu membantu saya membangun aplikasi *student task planner* yang ramah pemula" |
| **Task** | Menjelaskan tujuan dan kebutuhan | Pengelola tugas untuk mahasiswa tahun pertama: daftar tugas, judul, tenggat, status selesai, tombol tandai selesai, filter *all / pending / completed*, tampilan bersih dan responsif |
| **Context** | Memberi batasan dan situasi | Pakai HTML, CSS, dan JavaScript murni; sederhana untuk pemula; tanpa library tambahan; kode rapi dengan penjelasan tiap file |
| **Format** | Menentukan bentuk keluaran | Kode lengkap per file, cara menjalankan, cara menguji interaksi utama, dan AI tidak boleh mengklaim aplikasinya berfungsi sebelum diverifikasi |

**Keuntungan prompt engineering:**
- Meningkatkan performa model AI.
- Mengurangi bias dan respons yang menyinggung.
- Meningkatkan kontrol dan keterprediksian hasil.
- Memberikan pengalaman pengguna yang lebih baik.

#### B. Git dan GitHub

**Apa itu Git?** Sistem *version control* yang mencatat siapa, kapan, dan apa saja yang diubah dalam sebuah file. Git dibuat oleh Linus Torvalds pada 2005.

**Git vs GitHub**

| | Git | GitHub |
|---|---|---|
| **Sifat** | Sistem version control terdistribusi (DVCS) | Platform berbasis web |
| **Fungsi** | Melacak dan mengelola perubahan kode secara lokal | Menyimpan repository Git secara online dan mendukung kolaborasi |

**Tiga area dalam Git workflow**

| Area | Penjelasan |
|---|---|
| **Working directory (working tree)** | Salinan satu versi proyek yang sedang dikerjakan di komputer. Filenya diambil dari database Git. |
| **Staging area (index)** | Tempat menampung perubahan yang akan dimasukkan ke *commit* berikutnya. |
| **Git directory** | Tempat Git menyimpan metadata dan *object database*. Bagian inilah yang disalin saat `git clone`. |

Alurnya: **ubah file** (working directory) → **`git add`** (staging area) → **`git commit`** (tersimpan di repository).

**Perintah dasar Git**

```bash
git init                    # memulai repository baru
git add .                   # memindahkan file ke staging area
git commit -m "pesan"       # menyimpan perubahan ke repository