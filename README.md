### README.md
```markdown
# NHANES Health Clustering with K-Means & DBSCAN

## 📖 Deskripsi
Proyek ini membandingkan dua metode clustering:
- **K-Means** → berbasis centroid
- **DBSCAN** → berbasis kepadatan & deteksi outlier

Dataset: `NHANES_age_prediction.csv` (2.278 observasi, 10 fitur)  
Fokus: Segmentasi berdasarkan variabel metabolik (BMI, glukosa, insulin, usia).  

---

## 🛠️ Metodologi
1. **Preprocessing**: Normalisasi fitur numerik (z-score)  
2. **K-Means**: Eksperimen k=2–10 → Elbow & Silhouette untuk jumlah cluster optimal  
3. **DBSCAN**: Eksperimen parameter eps (k-distance graph) & min_samples  
4. **Evaluasi**: Silhouette Score, Davies-Bouldin Index, validasi eksternal `age_group`  
5. **Interpretasi**: Analisis profil tiap cluster  

---

## 📊 Hasil Utama
- **K-Means**: optimal di **k=5**, menghasilkan klaster mulai dari *muda sehat* hingga *lansia berisiko metabolik*.  
- **DBSCAN**: eps≈2, min_samples=5 → 8 cluster bermakna + outlier. Mendeteksi detail risiko seperti resistensi insulin & gangguan glukosa berat.  

---

## 🧰 Tools yang Digunakan
- **Python (Colab/Jupyter)** → implementasi K-Means & DBSCAN  
- **Excel** → eksplorasi awal dataset, distribusi variabel  
- **Word** → dokumentasi hasil & interpretasi  

---

## 🚀 Cara Menjalankan
```bash
git clone https://github.com/username/NHANES-Health-Clustering-KMeans-DBSCAN.git
cd NHANES-Health-Clustering-KMeans-DBSCAN
