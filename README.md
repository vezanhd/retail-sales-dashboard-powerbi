# Dashboard Penjualan & Profitabilitas Retail 2023-2024

**Personal Practice Project** | Microsoft Power BI | 2026

Dashboard interaktif untuk menganalisis performa penjualan dan profitabilitas bisnis retail berdasarkan kategori produk, wilayah, dan tren waktu — dibangun menggunakan Microsoft Power BI Desktop dengan DAX (Data Analysis Expressions).

---

## 📥 Download File

- **[Download File Power BI (.pbix)](https://github.com/vezanhd/retail-sales-dashboard-powerbi/raw/main/dashboard/Dashboard_Penjualan_Retail_PowerBI.pbix)**
- **[Download Dataset (.xlsx)](https://github.com/vezanhd/retail-sales-dashboard-powerbi/raw/main/data/Dataset_Penjualan_Retail.xlsx)**

> **Catatan:** File .pbix dapat dibuka menggunakan [Power BI Desktop](https://powerbi.microsoft.com/en-us/desktop/) (gratis).

---

## 📁 Tentang Project

Project ini merupakan latihan pribadi untuk mengasah kemampuan analisis data dan visualisasi menggunakan Microsoft Power BI. Data yang digunakan adalah dataset penjualan retail dummy yang mencakup 300 transaksi dari tahun 2023–2024 dengan 5 kategori produk dan 4 wilayah di Indonesia.

---

## 📂 Struktur Repository

```
retail-sales-dashboard-powerbi/
├── data/
│   └── Dataset_Penjualan_Retail.xlsx
├── dashboard/
│   ├── Dashboard_Penjualan_Retail_PowerBI.pbix
└── README.md
```

---

## 📋 Dataset

| Kolom | Deskripsi |
|---|---|
| ID Transaksi | ID unik setiap transaksi |
| Tanggal | Tanggal transaksi (2023–2024) |
| Nama Pelanggan | Nama pelanggan |
| Kategori | Elektronik, Furnitur, Makanan, Olahraga, Pakaian |
| Produk | Nama produk spesifik |
| Wilayah | Jawa, Sumatera, Kalimantan, Sulawesi |
| Kota | Kota tempat transaksi |
| Sales | Total penjualan (Rp) |
| Quantity | Jumlah item terjual |
| Diskon | Persentase diskon |
| Profit | Keuntungan (Rp) |

---

## 🎯 Fitur Dashboard

### Page 1 — Dashboard Penjualan Retail
- **Bar Chart** — Total Sales per Kategori Produk (format Rp, warna per kategori)
- **Line Chart** — Tren Penjualan Bulanan 2023–2024 (dengan marker per bulan)
- **Pie Chart** — Distribusi Sales per Wilayah (dengan persentase)
- **Treemap** — Top Produk Berdasarkan Sales
- **Slicer** — Filter Wilayah dan Kategori (otomatis memfilter semua chart)

### Page 2 — Analisis Profitabilitas
- **Bar Chart** — Profit per Wilayah
- **Bar Chart** — Profit Margin % per Kategori (menggunakan DAX Measure)
- **Bar Chart** — Distribusi Status Profit (menggunakan DAX Column)
- **Slicer** — Filter Wilayah

---

## 🔍 Key Findings

**Penjualan:**
- **Elektronik** mendominasi total sales dengan Rp1,25 Miliar
- **Sulawesi** menjadi wilayah dengan kontribusi sales terbesar
- **Laptop** menjadi produk dengan sales tertinggi mencapai Rp635 Juta
- Penjualan mencapai puncak di bulan **Mei** pada tahun kedua

**Profitabilitas:**
- **Furnitur** memiliki profit margin tertinggi (24,55%) meski bukan kategori dengan sales terbesar
- **Elektronik** memiliki profit margin terendah (19,70%) meskipun dominan di sales
- **Sulawesi** menghasilkan profit terbesar (Rp149 Juta)
- **221 dari 300 transaksi** (73,7%) masuk kategori Profit Rendah (<Rp1 Juta)

---

## 🛠️ Tech Stack

- **Microsoft Power BI Desktop** — Visualisasi & Dashboard
- **DAX (Data Analysis Expressions)** — Kalkulasi measure dan kolom kustom
- **Microsoft Excel** — Dataset

---

## 💡 Teknik Power BI yang Digunakan

- **DAX Measure** — `Profit Margin % = DIVIDE(SUM([Profit]), SUM([Sales]))`
- **DAX Calculated Column** — `Status Profit` menggunakan `SWITCH(TRUE(),...)`
- **Slicer** — Filter interaktif otomatis tanpa perlu konfigurasi tambahan
- **Format Rupiah** — Custom format `Rp#,0,,` pada kolom Sales dan Profit
- **Date Handling** — Konversi serial date Excel ke format Date Power BI
- **Multiple Chart Types** — Bar, Line, Pie, Treemap

---

## 📊 Perbandingan dengan Tableau

Project ini menggunakan dataset yang sama dengan [Tableau version](https://github.com/vezanhd/retail-sales-dashboard-tableau), sehingga dapat digunakan sebagai perbandingan langsung antara kedua tools.

| Fitur | Tableau | Power BI |
|---|---|---|
| Warna otomatis per kategori | ✅ Mudah | ⚠️ Manual |
| Filter/Slicer | Perlu setting Action Filter | ✅ Otomatis |
| Calculated Field/DAX | Calculated Field | DAX (lebih powerful) |
| Publish gratis | ✅ Tableau Public | ⚠️ Butuh akun Pro |
| Integrasi Microsoft | ❌ | ✅ Excel, Teams, dll |

---

## 📸 Screenshot

### Page 1 — Dashboard Penjualan Retail 2023-2024
<img width="757" height="425" alt="image" src="https://github.com/user-attachments/assets/94e687eb-6ade-48b7-ae72-f4a7278c911c" />

### Page 2 — Analisis Profitabilitas 2023-2024
<img width="756" height="425" alt="image" src="https://github.com/user-attachments/assets/08ed737e-e109-450c-9a5e-23ffa5f4132c" />

---

## 👤 Author

**Vezan Hidayatullah**
