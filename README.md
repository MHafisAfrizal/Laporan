# Laporan
# Proyek Akhir: Menyelesaikan Permasalahan Perusahaan Edutech

## Business Understanding

### Latar Belakang Bisnis
Jaya Jaya Maju adalah perusahaan edutech multinasional yang berfokus pada penyediaan platform pembelajaran online untuk lebih dari 1000 karyawan di berbagai departemen, seperti pengembangan konten, teknologi, dan dukungan pelanggan. Perusahaan ini berkembang pesat, namun menghadapi tantangan signifikan akibat tingginya *attrition rate* (tingkat turnover karyawan) yang melebihi 10%. Tingginya turnover ini mengakibatkan hilangnya keahlian, biaya rekrutmen yang besar, dan gangguan dalam operasional, yang pada akhirnya dapat memengaruhi kualitas layanan edukasi yang diberikan kepada pengguna.

### Permasalahan Bisnis
1. Tingginya *attrition rate* (>10%) yang menyebabkan kehilangan talenta berpengalaman.
2. Kurangnya pemahaman mendalam tentang faktor-faktor yang memicu karyawan keluar, seperti kepuasan kerja, gaji, lembur, atau masa kerja.
3. Ketidakmampuan departemen HR untuk memantau dan mengambil tindakan preventif terhadap *attrition* secara real-time.
4. Biaya operasional yang meningkat akibat proses rekrutmen dan pelatihan karyawan baru.

### Cakupan Proyek
Proyek ini mencakup:
- Analisis data karyawan untuk mengidentifikasi faktor-faktor utama yang memengaruhi *attrition*.
- Pengembangan model machine learning untuk memprediksi kemungkinan karyawan keluar.
- Pembuatan *business dashboard* untuk memantau faktor-faktor *attrition* secara visual.
- Dokumentasi temuan dan rekomendasi action items untuk membantu HR mengurangi *attrition rate*.

### Persiapan
- **Sumber Data**: Dataset berisi informasi karyawan (`employee_data.csv`) dengan 1470 baris dan 35 kolom, meliputi data demografi, gaji, kepuasan kerja, dan status *attrition*.
- **Setup Environment**:
- ***Instalasi dependensi***
```pip install -r requirements.txt```

- ***Requirements***
```pandas==1.5.3
numpy==1.24.3
matplotlib==3.7.1
seaborn==0.12.2
scikit-learn==1.2.2
```
## Business Dashboard
Business dashboard dibuat untuk memantau faktor-faktor utama yang memengaruhi *attrition rate* di Jaya Jaya Maju. Dashboard ini mencakup visualisasi berikut:
- **Attrition berdasarkan Kepuasan Kerja**: Menunjukkan bahwa karyawan dengan kepuasan kerja rendah (1-2) lebih cenderung keluar.
- **Attrition berdasarkan Pendapatan Bulanan**: Mengindikasikan bahwa karyawan dengan pendapatan rendah memiliki risiko *attrition* lebih tinggi.
- **Attrition berdasarkan Lembur**: Menyoroti bahwa karyawan yang sering lembur (OverTime = 1) lebih mungkin keluar.
- **Attrition berdasarkan Masa Kerja**: Mengungkapkan bahwa karyawan dengan masa kerja pendek (0-5 tahun) lebih rentan keluar.

Dashboard disimulasikan menggunakan Python (Matplotlib/Seaborn) dan disimpan sebagai screenshot dalam file `<username_dicoding>-dashboard.png`. Karena ini adalah simulasi berbasis kode, tidak ada link akses langsung. File ini dapat dilihat di folder submission untuk analisis visual.

## Conclusion
Berdasarkan analisis data dan pemodelan, ditemukan bahwa faktor utama *attrition* meliputi kepuasan kerja rendah, pendapatan bulanan rendah, kebiasaan lembur, dan masa kerja yang singkat. Model machine learning (Random Forest) yang dikembangkan mencapai akurasi sekitar 85%, memungkinkan prediksi *attrition* dengan baik. Dashboard yang dibuat memberikan alat visual untuk HR guna memantau tren *attrition* secara berkala. Proyek ini berhasil memberikan wawasan yang dapat digunakan untuk mengurangi turnover karyawan dan meningkatkan retensi.

### Rekomendasi Action Items (Optional)
- **Meningkatkan Kepuasan Kerja**: Mengadakan survei rutin dan program kesejahteraan karyawan, seperti pelatihan atau dukungan mental, untuk meningkatkan kepuasan kerja.
- **Menyesuaikan Gaji**: Meninjau ulang struktur gaji agar kompetitif, terutama untuk karyawan dengan pendapatan rendah.
- **Mengurangi Lembur**: Membatasi jam lembur dan memberikan kompensasi yang adil untuk karyawan yang bekerja ekstra.
- **Program Retensi Awal**: Mengimplementasikan program orientasi dan *mentoring* untuk karyawan baru agar mereka lebih betah di perusahaan.
