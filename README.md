# 📚 Learning Journey 365

365 günlük makine öğrenmesi ve yapay zeka öğrenme yolculuğumu belgelediğim kişisel repository'mdir.

## 🎯 Hedef

Bu repo, makine öğrenmesi ve yapay zeka alanında günlük olarak öğrendiklerimi, notlarımı ve projelerimi paylaştığım bir öğrenme günlüğüdür. Amacım, sürekli ve düzenli bir şekilde öğrenmeyi sürdürmek ve bu süreci belgelemektir.

## 📖 Okuduğum Kitaplar

### ✅ Tamamlanan
- **Machine Learning for Absolute Beginners** - Detaylı notlar ve öğrendiklerim `notes/` klasöründe

### 📘 Devam Eden
- **Hands-On Machine Learning with Scikit-Learn, Keras, and TensorFlow** (O'Reilly) - Yakında başlayacağım!

## 📁 Repository Yapısı

```
learning-journey-365/
│
├── notes/                      # Günlük öğrenme notları
│   ├── 2025-09-18/            # AI for Absolute Beginners notları
│   ├── 2025-09-19/            # K-Nearest Neighbors (KNN) notları
│   ├── 2025-09-22/            # KNN Clustering notları
│   ├── 2025-09-23/            # Bias-Variance Trade-off notları
│   ├── 2025-09-24/            # StatQuest video notları
│   ├── 2025-09-25/            # Artificial Neural Networks (ANN) notları
│   └── 2025-09-26/            # Decision Trees notları
│
└── ml-project/                 # Makine öğrenmesi projeleri
    └── 1-titanic/             # Titanic hayatta kalma tahmini
```

## 🚀 Projeler

### 1️⃣ Titanic - Hayatta Kalma Tahmini

**Klasör:** [`ml-project/1-titanic/`](ml-project/1-titanic/)

Titanic felaketinde yolcuların hayatta kalıp kalmadığını tahmin eden klasik bir makine öğrenmesi projesi.

**🎯 Proje Hedefi:**
- Titanic yolcularının özelliklerini (yaş, cinsiyet, bilet sınıfı, vb.) kullanarak hayatta kalma durumunu tahmin etmek

**🛠️ Kullanılan Teknolojiler:**
- Python 3.x
- Pandas - Veri işleme ve analiz
- NumPy - Sayısal hesaplamalar
- Seaborn & Matplotlib - Veri görselleştirme
- Scikit-learn - Makine öğrenmesi modeli

**📊 Model Detayları:**
- **Algoritma:** Logistic Regression
- **Veri Ön İşleme:**
  - Eksik verilerin doldurulması (Age: ortalama ile, Embarked: mod ile)
  - Gereksiz sütunların çıkarılması (PassengerId, Name, Cabin, Ticket)
  - Kategorik verilerin dönüştürülmesi (Sex: Label Encoding, Embarked: One-Hot Encoding)
- **Train/Test Split:** %80 eğitim, %20 test
- **Max Iterations:** 4000

**🎯 Sonuçlar:**
- **Test Seti Doğruluğu:** %81
- **Kaggle Skoru:** %78.6 (0.7855)

**📁 Proje Dosyaları:**
- `titanic.ipynb` - Detaylı analiz ve adım adım açıklamalar içeren Jupyter Notebook
- `titanic.py` - Python script versiyonu
- `train.csv` - Eğitim veri seti (891 yolcu)
- `test.csv` - Test veri seti (418 yolcu)

**🔍 Öğrenilenler:**
- Eksik veri (missing data) yönetimi
- Kategorik verilerin dönüştürülmesi (Label Encoding vs One-Hot Encoding)
- Keşifsel Veri Analizi (EDA) teknikleri
- Model değerlendirme metrikleri
- Kaggle yarışmalarına submission süreci

## 📝 Notlar

`notes/` klasöründe günlük olarak öğrendiklerimi not ediyorum. Konular şunları içeriyor:

- **K-Nearest Neighbors (KNN)** - Sınıflandırma ve clustering
- **Bias-Variance Trade-off** - Model kompleksitesi ve genelleme
- **Support Vector Machines (SVM)** - Destek vektör makineleri
- **Artificial Neural Networks (ANN)** - Yapay sinir ağları temel kavramları
- **Decision Trees** - Karar ağaçları
- **StatQuest Video Notları** - Josh Starmer'ın harika ML açıklamaları

## 🎓 Öğrenme Kaynakları

- 📚 Kitaplar: Machine Learning for Absolute Beginners, Hands-On Machine Learning (O'Reilly)
- 🎥 YouTube: StatQuest with Josh Starmer
- 🏆 Kaggle: Pratik yapma ve yarışmalar
- 📊 Colab: Projeleri geliştirme ortamı

## 📈 İlerleme

Bu repo, makine öğrenmesi yolculuğumun canlı bir belgesidir. Her gün yeni şeyler öğreniyor, notlar alıyor ve projeler geliştiriyorum.

**Güncel Durum:**
- ✅ Machine Learning for Absolute Beginners kitabı tamamlandı
- ✅ İlk Kaggle projesi (Titanic) tamamlandı - %78.6 accuracy
- 🔄 Hands-On Machine Learning kitabına başlayacağım
- 🔄 Günlük not alma devam ediyor

## 💡 İletişim

Bu öğrenme yolculuğu hakkında sorularınız veya önerileriniz varsa, issue açabilir veya pull request gönderebilirsiniz!

---

⭐ Bu repo'yu beğendiyseniz yıldızlamayı unutmayın!

**Son Güncelleme:** Ekim 2025

