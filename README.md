# Capstone 3: Bank Marketing Campaign Optimization

### Prediksi Nasabah untuk Deposito Berjangka

## Deskripsi Proyek

Proyek ini bertujuan untuk mengoptimalkan kampanye pemasaran bank dengan menggunakan model machine learning. Fokus utama adalah memprediksi nasabah yang potensial untuk membuka deposito berjangka, sehingga dapat meningkatkan efektivitas pemasaran dan profitabilitas bank.

---

## Struktur Proyek

1. **Permasalahan Bisnis**:
   - **Latar Belakang**: Bank menghadapi tantangan untuk menarik nasabah baru dan mempertahankan nasabah yang sudah ada.
   - **Tujuan**:
     - Mengidentifikasi nasabah potensial.
     - Menyusun strategi pemasaran yang efektif.
     - Meningkatkan pendapatan bank.

2. **Pemahaman Data**:
   - **EDA (Exploratory Data Analysis)**: Analisis data profil nasabah dan data pemasaran.
   - **Pra-pemrosesan Data**:
     - Penanganan nilai `unknown` dan outliers.
     - Encoding dan scaling fitur.
     - Data splitting (train, test, validation).
   - **Distribusi Data**:
     - Data relatif seimbang dengan rasio kelas positif dan negatif sekitar 1:1.09.

3. **Pemodelan Machine Learning**:
   - Model utama: **LGBM Classifier**.
   - Fokus pada optimasi metrik **Recall** untuk meminimalkan False Negatives.

4. **Evaluasi Model**:
   - Model menghasilkan Recall terbaik pada set testing (63%).
   - Fitur paling penting: `pdays`, `poutcome`, dan `campaign`.

5. **Kesimpulan**:
   - Penggunaan model LGBM memberikan efisiensi biaya pemasaran hingga Rp 538 juta dibandingkan tanpa model.
   - Model mampu meningkatkan targeting nasabah dengan akurasi yang lebih baik.

6. **Rekomendasi**:
   - Tambahkan fitur seperti segmentasi nasabah (usia, status pernikahan, dsb.).
   - Gunakan algoritma tambahan untuk benchmarking.
   - Lakukan update model secara berkala sesuai perubahan data historis dan tren pasar.

---

## Teknologi yang Digunakan

- **Python Libraries**: `pandas`, `numpy`, `scikit-learn`, `lightgbm`, dan lainnya.
- **Machine Learning Frameworks**: LightGBM, Random Forest, Decision Tree.
- **Data Preprocessing**: One-hot encoding, Binary encoding, RobustScaler.

---

## Cara Menjalankan Proyek

1. Clone repositori:
   ```bash
   git clone <repository-url>
   cd bank-marketing-capstone
