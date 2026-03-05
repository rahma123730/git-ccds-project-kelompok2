# 🚀 Team 2 - Git Collaboration & CCDS Project

[![Standard: CCDS](https://img.shields.io/badge/standard-CCDS-orange?style=flat-square)](https://cookiecutter-data-science.drivendata.org/)
[![Gitmoji](https://img.shields.io/badge/gitmoji-%20😜%20-FFDD67.svg?style=flat-square)](https://gitmoji.dev)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg?style=flat-square)](https://opensource.org/licenses/MIT)

Selamat datang di repository **Team 2 - Kelas 24IC1**. Proyek ini merupakan implementasi kolaborasi tim menggunakan alur kerja Git yang ketat dan standarisasi struktur proyek berbasis **Cookiecutter Data Science (CCDS)**.

---

## 👥 Profil Anggota Tim
Kami adalah tim multidisiplin yang berdedikasi untuk menciptakan workflow data science yang bersih dan terukur.

| Foto | NIM | Nama | Peran |
| :---: | :---: | :--- | :--- |
| 👨‍💼 | **20124033** | Rahma Aulia Dini | **Product Manager** |
| 🎨 | **20124028** | Muhammad Faqih Dienul Haq | **UI/UX Designer** |
| 🧪 | **20124021** | Lailani Alifah | **Data Scientist** |
| 💻 | **20124009** | Widya Novianti | **Software Engineer** |
| 🖌️ | **20124025** | Muhafidz Ikram Ramadhan | **UI/UX Designer** |

---

## 🛠️ Alur Kerja Proyek (Workflow)
Untuk menjaga integritas kode di cabang utama (`main`), kami menerapkan aturan berikut:

1. **Branching Strategy**: Setiap fitur dikembangkan di branch terpisah (`feat/`, `fix/`, `docs/`).
2. **Commit Standard**: Wajib menggunakan **Gitmoji** (Contoh: `✨ :sparkles: add preprocessing script`).
3. **Collaboration**: Penggabungan kode hanya dilakukan melalui **Pull Request (PR)** setelah melalui proses review oleh Product Manager.

```mermaid
graph LR
    A[main] -- checkout --> B(feature branch)
    B -- commits with gitmoji --> B
    B -- pull request --> C{Review PM}
    C -- approved --> A

    ├── data
│   ├── external       # Data dari sumber pihak ketiga.
│   ├── interim        # Data yang telah diubah sebagian.
│   ├── processed      # Dataset final untuk pemodelan.
│   └── raw            # Dataset asli yang tidak boleh diubah (immutable).
├── models             # Model yang telah dilatih (pickle/joblib).
├── notebooks          # Jupyter notebooks untuk EDA dan eksperimen.
├── references         # Kamus data, manual, dan aset visual.
├── reports            # Analisis yang dihasilkan (HTML, PDF, dsb).
│   └── figures        # Grafik dan visualisasi untuk laporan.
├── src                # Source code Python untuk digunakan di proyek ini.
└── README.md          # Dokumentasi utama proyek.

