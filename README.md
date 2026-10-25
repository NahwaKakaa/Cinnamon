# Cinnamon Disease Classification & Model Comparison

Proyek klasifikasi penyakit pada tanaman kayu manis (Cinnamon) menggunakan deep learning berbasis Transfer Learning dan perbandingan arsitektur CNN:
- **EfficientNetB0** (Akurasi Validasi: **94.10%**)
- **DenseNet121** (Akurasi Validasi: **90.68%**)
- **ResNet50** (Akurasi Validasi: **90.68%**)
- **MobileNetV2** (Akurasi Validasi: **89.44%**)

## 📁 Struktur Repositori

```text
├── cinnamon.ipynb                  # Jupyter Notebook lengkap untuk training & evaluasi
├── cinnamon-output/
│   ├── best_DenseNet121_comparison.keras     # Model checkpoint DenseNet121 (<100MB)
│   ├── best_EfficientNetB0_comparison.keras   # Model checkpoint EfficientNetB0 (<100MB)
│   ├── best_MobileNetV2_comparison.keras     # Model checkpoint MobileNetV2 (<100MB)
│   ├── cinnamon.log                          # Log pelatihan lengkap
│   ├── model_comparison_results.json         # Hasil metrik perbandingan model
│   ├── model_comparison_histories.json       # History loss & akurasi training
│   ├── model_comparison_plots/               # Grafik kurva training & evaluasi
│   ├── visualisasi_hasil/                    # Visualisasi confusion matrix & perbandingan
│   └── model_backups/                        # Checkpoint bobot fase pelatihan
└── Cinnamon.code-workspace         # Konfigurasi workspace
```

> **Catatan:** File bobot model ResNet50 (>100MB) dan dataset gambar dikecualikan dari repository via `.gitignore` sesuai batasan ukuran file GitHub.
