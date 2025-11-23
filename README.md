# 🛍️ Kalkulator Diskon

<div align="center">

![Python Version](https://img.shields.io/badge/python-3.7%2B-blue)
![License](https://img.shields.io/badge/license-MIT-green)
![Status](https://img.shields.io/badge/status-active-success)
![GUI](https://img.shields.io/badge/GUI-Tkinter-orange)

**Aplikasi kalkulator diskon dengan GUI modern dan sistem penyimpanan history otomatis**

[Fitur](#-fitur) • [Instalasi](#-instalasi) • [Penggunaan](#-penggunaan) • [Dokumentasi](#-dokumentasi)

</div>

## 📋 Daftar Isi

- [Gambaran Umum](#-gambaran-umum)
- [Fitur](#-fitur)
- [Instalasi](#-instalasi)
- [Penggunaan](#-penggunaan)
- [Dokumentasi](#-dokumentasi)
- [Contoh Penggunaan](#-contoh-penggunaan)
- [FAQ](#-faq)

## 🚀 Gambaran Umum

**Kalkulator Diskon** adalah aplikasi Python yang dirancang untuk menghitung harga diskon dengan antarmuka grafis yang modern dan intuitif. Aplikasi ini tidak hanya melakukan perhitungan dasar, tetapi juga dilengkapi dengan sistem penyimpanan history otomatis, export data, dan berbagai fitur profesional lainnya.

### ✨ Highlights

- 🎨 **GUI Modern** dengan desain yang user-friendly
- 💾 **Penyimpanan Otomatis** semua perhitungan ke file JSON
- 📊 **Riwayat Lengkap** dengan timestamp dan detail perhitungan
- 📁 **Export Data** ke format CSV untuk analisis lebih lanjut
- ✅ **Validasi Input** yang robust dan informatif
- 💰 **Format Rupiah** yang sesuai standar Indonesia

## 🌟 Fitur

### 🧮 Core Features
- **Perhitungan Diskon Akurat** - Menghitung harga setelah diskon dengan presisi
- **Validasi Input** - Pengecekan input harga dan diskon yang komprehensif
- **Format Mata Uang** - Tampilan harga dalam format Rupiah yang benar
- **Multi-Validation** - Validasi untuk berbagai skenario input

### 💾 Data Management
- **Auto-save History** - Setiap perhitungan langsung tersimpan
- **JSON Storage** - Penyimpanan data terstruktur dalam format JSON
- **CSV Export** - Ekspor data history ke format spreadsheet
- **History Management** - Lihat, hapus, dan kelola riwayat perhitungan
- **Backup Otomatis** - Data tersimpan aman dan dapat diakses kapan saja

### 🎨 GUI Features
- **Modern Interface** - Antarmuka yang clean dan profesional
- **Responsive Design** - Adaptif untuk berbagai ukuran layar
- **Real-time Results** - Hasil perhitungan ditampilkan secara instan
- **Keyboard Navigation** - Support tombol Enter untuk navigasi cepat
- **Color-coded Feedback** - Visual feedback yang informatif

### 🛠️ Utility Features
- **Reset Function** - Bersihkan input dengan satu klik
- **Error Handling** - Penanganan error yang elegant
- **Input Validation** - Validasi real-time untuk input pengguna
- **Timestamp Recording** - Waktu setiap perhitungan terekam otomatis


## 📥 Instalasi

### Prerequisites

- Python 3.7 atau lebih tinggi
- pip (Python package manager)

### Step-by-Step Installation

1. **Download atau Clone Project**
   ```bash
   git clone https://github.com/username/kalkulator-diskon-super.git
   cd kalkulator-diskon-super
   ```

2. **Buat Virtual Environment (Recommended)**
   ```bash
   python -m venv diskon_env
   source diskon_env/bin/activate  # Linux/Mac
   diskon_env\Scripts\activate    # Windows
   ```

3. **Install Dependencies**
   ```bash
   pip install -r requirements.txt
   ```

4. **Jalankan Aplikasi**
   ```bash
   python main.py
   ```

### Quick Install (Windows)
```bash
# Download project, ekstrak, dan jalankan:
python main.py
```

## 🎮 Penggunaan

### Menjalankan Aplikasi

```bash
python main.py
```

### Basic Usage

1. **Input Data**
   - Masukkan **Harga Asal** (dalam Rupiah) di field pertama
   - Masukkan **Persentase Diskon** (tanpa simbol %) di field kedua

2. **Melakukan Perhitungan**
   - Tekan tombol **"Hitung Diskon"** atau tekan **Enter**
   - Hasil akan langsung ditampilkan di bagian "Hasil Perhitungan"

3. **Melihat History**
   - Riwayat perhitungan otomatis tersimpan dan ditampilkan
   - Gunakan tombol **"Muat Ulang History"** untuk refresh data

### Advanced Features

1. **Export Data**
   - Klik tombol **"Export ke CSV"** untuk mengekspor history
   - File CSV akan tersimpan dengan format yang rapi

2. **Management History**
   - **Hapus History**: Tombol untuk menghapus semua riwayat
   - **Auto-refresh**: History otomatis terupdate setelah perhitungan baru

### Keyboard Shortcuts

| Shortcut | Action |
|----------|--------|
| `Enter` (di field harga) | Pindah ke field diskon |
| `Enter` (di field diskon) | Jalankan perhitungan |
| `Tab` | Navigasi antar field |

## 📚 Dokumentasi

### Data Flow

1. **Input Phase**: User memasukkan harga dan diskon
2. **Validation Phase**: Sistem memvalidasi input
3. **Calculation Phase**: Melakukan perhitungan diskon
4. **Storage Phase**: Menyimpan hasil ke history
5. **Display Phase**: Menampilkan hasil dan update history

---

### File Descriptions

| File | Description |
|------|-------------|
| `main.py` | Entry point aplikasi, menjalankan GUI utama |
| `diskon_core.py` | Inti logika perhitungan diskon dan validasi |
| `history_manager.py` | Mengelola penyimpanan dan load history |
| `gui_app.py` | Antarmuka pengguna dengan Tkinter |
| `requirements.txt` | Dependencies yang diperlukan |


## 💡 Contoh Penggunaan

### Basic Calculation
```
Harga Asal: Rp 1.000.000
Diskon: 20%
Hasil: Rp 800.000

Detail:
• Harga Asal: Rp 1.000.000
• Diskon: 20%
• Total Diskon: Rp 200.000
```

### Multiple Calculations
```
Perhitungan 1:
Harga Asal: Rp 500.000
Diskon: 10%
Hasil: Rp 450.000

Perhitungan 2:
Harga Asal: Rp 2.500.000  
Diskon: 15%
Hasil: Rp 2.125.000

Perhitungan 3:
Harga Asal: Rp 75.000
Diskon: 5%
Hasil: Rp 71.250
```

### Export Example
```csv
Waktu,Harga Asal,Diskon (%),Harga Diskon
2024-01-15 10:30:15,1000000,20,800000
2024-01-15 10:35:22,500000,10,450000
2024-01-15 11:20:45,2500000,15,2125000
```

## ❓ FAQ

### Q: Apakah data history tersimpan secara otomatis?
**A:** Ya, setiap perhitungan baru otomatis tersimpan ke file JSON.

### Q: Bagaimana cara backup data history?
**A:** Cukup backup file `history_diskon.json` di folder data.

### Q: Format apa saja yang didukung untuk export?
**A:** Saat ini mendukung CSV, dan mudah dikembangkan untuk format lain.

### Q: Apakah ada batasan untuk nilai harga atau diskon?
**A:** Diskon maksimal 100%, harga harus positif. Validasi error akan muncul jika input tidak valid.

### Q: Bisakah digunakan untuk perhitungan diskon bertingkat?
**A:** Saat ini belum, tapi architecture sudah siap untuk dikembangkan.

### Q: Apakah perlu koneksi internet?
**A:** Tidak! Aplikasi ini berjalan sepenuhnya offline.


### Troubleshooting Common Issues

**Problem**: Aplikasi tidak bisa dijalankan
**Solution**: Pastikan Python 3.7+ terinstall dan semua file dalam folder yang sama

**Problem**: History tidak tersimpan
**Solution**: Check permission folder dan pastikan tidak ada file yang sedang terbuka

**Problem**: Export CSV gagal
**Solution**: Pastikan file CSV tidak sedang dibuka di program lain

---

<div align="center">

**⭐ Jangan lupa beri bintang! ⭐**

*Terima kasih telah menggunakan Kalkulator Diskon!*

</div>