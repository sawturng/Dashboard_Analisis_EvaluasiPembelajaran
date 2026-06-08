# Dashboard Analisis Butir Soal Evaluasi Pembelajaran

## Deskripsi

Dashboard Analisis Butir Soal merupakan aplikasi berbasis web yang dikembangkan untuk membantu proses evaluasi pembelajaran melalui analisis kualitas instrumen tes. Aplikasi ini digunakan untuk menghitung dan menampilkan hasil analisis validitas, daya pembeda, tingkat kesukaran, dan reliabilitas KR-20 secara otomatis dalam bentuk dashboard interaktif.

Proyek ini dibuat sebagai tugas UAS Mata Kuliah Evaluasi Pembelajaran.

## Tujuan

Tujuan pengembangan aplikasi ini adalah:

- Mengotomatisasi proses analisis butir soal.
- Menampilkan hasil analisis dalam bentuk dashboard interaktif.
- Membantu pendidik mengevaluasi kualitas instrumen tes.
- Menyediakan visualisasi data yang mudah dipahami.
- Mempermudah interpretasi hasil evaluasi pembelajaran.

## Fitur Utama

### Dashboard Utama

- Total Responden
- Jumlah Soal
- Nilai Tertinggi
- Nilai Terendah
- Reliabilitas KR-20
- Kategori Reliabilitas

### Analisis Siswa

- Jumlah Jawaban Benar
- Jumlah Jawaban Salah
- Nilai Akhir
- Ranking Siswa

### Analisis Butir Soal

- Validitas Butir Soal
- Daya Pembeda
- Tingkat Kesukaran
- Keputusan Soal

### Visualisasi Data

- Grafik Perolehan Nilai Siswa
- Grafik Validitas Soal
- Grafik Tingkat Kesukaran
- Grafik Daya Pembeda
- Ringkasan Analisis Instrumen


## 📖 Metode Analisis

### 1. Validitas

Validitas digunakan untuk mengetahui sejauh mana suatu butir soal mampu mengukur apa yang seharusnya diukur.

Metode yang digunakan adalah Korelasi Product Moment Pearson.

Rumus:

```math
r_{xy} = \frac{N\Sigma XY - (\Sigma X)(\Sigma Y)}
{\sqrt{[N\Sigma X^2-(\Sigma X)^2][N\Sigma Y^2-(\Sigma Y)^2]}}
```

### 2. Daya Pembeda

Daya pembeda digunakan untuk mengetahui kemampuan soal dalam membedakan peserta didik yang berkemampuan tinggi dan rendah.

Rumus:

```math
DP = \frac{BA - BB}{JA}
```

Keterangan:

- BA = Banyaknya siswa kelompok atas yang menjawab benar
- BB = Banyaknya siswa kelompok bawah yang menjawab benar
- JA = Jumlah siswa kelompok atas


### 3. Tingkat Kesukaran

Tingkat kesukaran digunakan untuk mengetahui tingkat kesulitan suatu butir soal.

Rumus:

```math
P = \frac{B}{JS}
```

Keterangan:

- P = Indeks Kesukaran
- B = Jumlah siswa menjawab benar
- JS = Jumlah seluruh siswa

Kategori:

| Nilai P | Kategori |
|----------|-----------|
| 0.00 - 0.30 | Sukar |
| 0.31 - 0.70 | Sedang |
| 0.71 - 1.00 | Mudah |


### 4. Reliabilitas KR-20

Reliabilitas digunakan untuk mengetahui tingkat konsistensi instrumen tes.

Rumus:

```math
KR20 = \frac{k}{k-1}
\left(
1-\frac{\Sigma pq}{S_t^2}
\right)
```

Keterangan:

- k = Jumlah soal
- p = Proporsi jawaban benar
- q = Proporsi jawaban salah
- St² = Varians total

## 📊 Dataset

Dataset yang digunakan terdiri dari:

- 20 Responden
- 25 Butir Soal Pilihan Ganda
- Kunci Jawaban
- Skoring Benar Salah (0 dan 1)

Data digunakan sebagai simulasi analisis butir soal pada mata kuliah Evaluasi Pembelajaran.

## 📈 Hasil Analisis

Berdasarkan hasil pengolahan data diperoleh:

| Komponen | Hasil |
|-----------|---------|
| Jumlah Responden | 20 |
| Jumlah Soal | 25 |
| Reliabilitas KR-20 | 0.546 |
| Kategori Reliabilitas | Cukup |

Secara umum sebagian besar soal memerlukan revisi karena belum memenuhi kriteria validitas dan daya pembeda yang baik.

## 🚀 Cara Menjalankan

1. Download project ini.
2. Buka menggunakan Visual Studio Code.
3. Jalankan file:

```text
index.html
```

4. Atau gunakan ekstensi Live Server.

## 👨‍💻 Pengembang

**Nama:** Anggia Dhini Hanifa  
**Program Studi:** Pendidikan Ilmu Komputer  
**Universitas:** Universitas Pendidikan Indonesia  
**Mata Kuliah:** Evaluasi Pembelajaran  
**Tahun:** 2026

Proyek ini dibuat untuk keperluan akademik dan pembelajaran.
