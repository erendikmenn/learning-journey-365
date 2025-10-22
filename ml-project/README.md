# Machine Learning Projeleri

Bu klasör, makine öğrenmesi projelerimi içermektedir.

## Projeler

### 1. Titanic - Hayatta Kalma Tahmini
- **Klasör:** `1-titanic/`
- **Açıklama:** Titanic yolcularının hayatta kalıp kalmadığını tahmin eden bir makine öğrenmesi projesi
- **Model:** Logistic Regression
- **Doğruluk:** %81 (test seti), %78.6 (Kaggle skoru)
- **Dosyalar:**
  - `titanic.ipynb` - Jupyter Notebook ile detaylı analiz
  - `titanic.py` - Python script versiyonu
  - `train.csv` - Eğitim verisi
  - `test.csv` - Test verisi

### 2. California Housing - Ev Fiyat Tahmini
- **Klasör:** `2-california/`
- **Açıklama:** California'daki ev fiyatlarını tahmin eden regresyon projesi
- **Veri Seti:** sklearn.datasets - California Housing Dataset
- **Modeller:** 
  - Linear Regression
  - Random Forest Regressor
- **Dosyalar:**
  - `california.ipynb` - Jupyter Notebook ile detaylı analiz
  - `california.py` - Python script versiyonu
- **Özellikler:**
  - Korelasyon analizi ve ısı haritası görselleştirme
  - Scatter plot ile özellik-fiyat ilişkileri
  - Farklı regresyon modellerinin karşılaştırması

## Kullanılan Teknolojiler
- Python
- Pandas
- NumPy
- Seaborn
- Matplotlib
- Scikit-learn
