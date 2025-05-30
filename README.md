# Tugas Akhir Visi Komputer

**Nama:** Eka Putri Difayanti  
**NIM:** D121221035

## Tentang Program

Program ini merupakan **simulasi efek Depth of Field (DoF)** menggunakan metode **Gaussian Blur manual** berbasis **Python** dengan library **OpenCV** dan **NumPy**.

Tujuan dari program ini adalah untuk:
- Mendeteksi **rambu lalu lintas** berdasarkan **warna merah dan putih**.
- Menyorot rambu (foreground) agar tetap tajam.
- Menerapkan **efek blur pada latar belakang (background)**, menyerupai efek kamera depth-of-field.


## Dataset Citra Input

- Gambar input dapat diakses pada folder `Images`.
- Dataset rambu jalan lainnya dapat diperoleh dari:
  👉 [Roboflow Road Signs Dataset](https://universe.roboflow.com/roboflow-100/road-signs-6ih4y)

## Cara Menjalankan Program

### **1. Melalui Google Colab**

1. Buka [Google Colab](https://colab.research.google.com/)
2. Upload file Python notebook (`.ipynb`) atau salin isi dari file `Simulasi_DoF_with_gaussian_blur.ipynb`.
3. Upload gambar rambu ke Colab (`Files` → Upload).
4. Ubah path gambar pada bagian ini di script:
   ```
   python
   image = cv2.imread('/content/nama_file_gambar.jpg')
6. Jalankan seluruh sel (Ctrl + F9 atau klik `Runtime > Run all`)
7. Output akan tampil berupa visualisasi proses segmentasi dan hasil blur akhir.


### **2. Jalankan Secara Lokal (PC dengan Python & OpenCV)**

#### Persyaratan

Pastikan Python dan library berikut sudah terinstal:

```bash
pip install numpy opencv-python matplotlib
```

#### Jalankan Program

1. Clone repository ini atau unduh file `.ipynb`
2. Simpan gambar input di direktori yang sama, atau sesuaikan path file gambar.
3. Buka terminal dan jalankan:

```bash
python Simulasi_DoF_with_gaussian_blur.ipynb
```

4. Program akan menampilkan hasil visualisasi berupa:

   * Mask warna merah
   * Mask putih (standalone & dalam area merah)
   * Hasil segmentasi
   * Output akhir: **rambu fokus, background blur**

---

## Struktur File

```
├── tugas_viskom.py            # File utama program simulasi
├── Images/                    # Folder untuk menyimpan input gambar
├── README.md                  # Dokumentasi ini
```

---
