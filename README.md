# reklam-etki-analizi
Çoklu Lineer Regresyon modeli kullanılarak reklam harcamalarının satışlar üzerindeki etkisinin analizi ve tahmini.
# 📈 Satış Tahmini: Çoklu Lineer Regresyon Analizi 
*(Sales Prediction with Multiple Linear Regression)*

Bu proje, bir şirketin çeşitli kanallara (TV, Radyo ve Gazete) ayırdığı reklam bütçelerinin toplam satışlar üzerindeki etkisini incelemek ve makine öğrenmesi teknikleri kullanarak gelecekteki satışları tahmin etmek amacıyla hazırlanmıştır.

## 🎯 Projenin Amacı
Veri bilimi ve makine öğrenmesi araçlarını kullanarak:
* Hangi reklam kanalının satışlara en yüksek getiriyi (ROI) sağladığını tespit etmek.
* İşe yaramayan reklam harcamalarını belirleyerek bütçe optimizasyonu sağlamak.
* Çoklu Lineer Regresyon modeli kurarak yeni bütçe planlarına göre satış tahmini yapmak.

## 📊 Kullanılan Veri Seti
Projede Kaggle platformunda yer alan **"Advertising Dataset"** kullanılmıştır. Veri setinde 200 farklı pazardaki reklam harcamaları ve karşılığında elde edilen satış rakamları (bin adet cinsinden) bulunmaktadır.
* **Bağımsız Değişkenler (Özellikler):** TV, Radyo, Gazete harcamaları.
* **Bağımlı Değişken (Hedef):** Satışlar (Sales).

## 🛠️ Kullanılan Teknolojiler ve Kütüphaneler
* **Python** (Veri manipülasyonu ve modelleme)
* **Pandas & NumPy** (Veri analizi)
* **Scikit-Learn** (Makine öğrenmesi ve model değerlendirme)
* **Matplotlib & Seaborn** (Veri görselleştirme ve Korelasyon Isı Haritası)

## 💡 Temel Bulgular ve İş İçgörüleri
Gerçekleştirilen Keşifçi Veri Analizi (EDA) ve modelleme sonucunda şu kritik iş içgörüleri elde edilmiştir:

1. **Yüksek Tahmin Gücü:** Kurulan Çoklu Lineer Regresyon modeli, satışlardaki değişimin **%90'ını** ($R^2 = 0.90$) açıklayabilmektedir.
2. **En Verimli Kanallar:** Satışlar üzerinde en büyük pozitif etkiye sahip reklam kanallarının sırasıyla **TV** ve **Radyo** olduğu gözlemlenmiştir.
3. **Bütçe Optimizasyonu (Özellik Seçimi):** Korelasyon analizi incelendiğinde, **Gazete** reklamlarının satışlar üzerinde neredeyse hiçbir anlamlı etkisi olmadığı tespit edilmiştir. Modelin başarısını düşürmemek ve sadeliği korumak adına Gazete verisi modelden çıkarılmış ve kaynakların TV/Radyo kanallarına kaydırılması önerilmiştir.
