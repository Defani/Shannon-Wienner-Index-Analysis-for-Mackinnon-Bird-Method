# 🐦 Analisis Keanekaragaman Hayati dengan Indeks Shannon–Wiener (H′)

**Penulis:** Defani Arman Alfitriansyan  
**Tools:** R (dengan library `vegan`, `dplyr`, `readxl`, dan `ggplot2`)  
**Dokumen:** _Shannon Wienner - Colab.pdf_

---

## 📘 Deskripsi

Proyek ini berisi **analisis keanekaragaman hayati** menggunakan **Indeks Shannon–Wiener (H′)**.  
Metode ini digunakan untuk menilai seberapa beragam suatu komunitas berdasarkan jumlah spesies (_richness_) dan keseragaman individu tiap spesies (_evenness_).

Analisis dilakukan menggunakan **metode daftar jenis MacKinnon** pada data pengamatan burung di kawasan _Leuwung Gede_, serta divisualisasikan menggunakan _kurva akumulasi jenis_.

---

## 🔢 Rumus Indeks Shannon–Wiener

Rumus umum yang digunakan adalah:

$$
H' = - \sum_{i=1}^{S} p_i \ln(p_i)
$$

Keterangan:
- \( H' \) = Indeks keanekaragaman Shannon–Wiener  
- \( S \) = Jumlah total spesies (species richness)  
- \( p_i \) = Proporsi individu jenis ke-\( i \) terhadap total individu  
- \( \ln \) = Logaritma natural (basis \( e \))  

Interpretasi nilai \( H' \):

| Nilai \(H'\) | Kategori Keanekaragaman | Keterangan |
|---------------|------------------------|-------------|
| < 1.0         | Rendah                 | Komunitas didominasi oleh sedikit jenis |
| 1.0 – 3.0     | Sedang                 | Keanekaragaman cukup stabil |
| > 3.0         | Tinggi                 | Komunitas beragam dan seimbang |

---

