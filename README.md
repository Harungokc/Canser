# 🧠 Kanser Sınıflandırması - Makine Öğrenmesi Modelleri ile Karşılaştırmalı Çalışma

## 1. 📌 Proje Tanımı

Bu proje, kanser teşhisinde kullanılabilecek farklı makine öğrenmesi algoritmalarını karşılaştırmalı olarak değerlendirerek, hangi modelin daha iyi performans gösterdiğini belirlemeyi amaçlamaktadır. Amaç; doğruluk oranı yüksek ve uygulanabilirliği kolay bir model tespit etmektir.

## 2. 📊 Kullanılan Modeller

Aşağıda yer alan yaygın gözetimli öğrenme algoritmaları kullanılarak sınıflandırma işlemi gerçekleştirilmiştir:

- **K-Nearest Neighbors (KNN)**
- **Lojistik Regresyon**
- **Naive Bayes (GaussianNB)**
- **Random Forest**
- **Support Vector Classifier (SVC)**
- **Decision Tree**

Her bir model aynı eğitim ve test veri setleri üzerinde çalıştırılarak performansları karşılaştırılmıştır.

## 3. 🧪 Veri Seti ve Özellikler

Kullanılan veri seti, kanserli ve kanser olmayan vakaları içeren etiketli tıbbi verilerden oluşmaktadır. Özellikler hücrelerin çeşitli morfolojik ölçütlerine dayanmaktadır (örneğin: boyut, doku yoğunluğu, çekirdek şekli). Hedef değişken, kanserin iyi huylu (*benign*) ya da kötü huylu (*malignant*) olduğunu belirtir.

## 4. ⚙️ Model Eğitimi ve Değerlendirme

Her model aşağıdaki ortak adımlar ile eğitilmiştir:

- Verilerin eğitim (%80) ve test (%20) olarak ayrılması
- Modelin eğitilmesi (`fit` metodu)
- Test verileri üzerinde tahmin yapılması (`predict` metodu)
- Aşağıdaki metrikler ile değerlendirme:
  - Accuracy (Doğruluk)
  - Precision (Kesinlik)
  - Recall (Duyarlılık)
  - F1-Score
- Ek olarak:
  - Karışıklık Matrisi Görselleştirmesi
  - ROC-AUC Eğrisi (varsa)

Tüm modeller aynı pipeline içerisinde eğitilmiş ve doğrulukları eş zamanlı olarak karşılaştırılmıştır.

## 5. 🥇 Sonuçlar

Model başarı skorları aşağıdaki gibidir:

| Model                | Accuracy | Precision | Recall | F1-Score |
|---------------------|----------|-----------|--------|----------|
| KNeighbors           | 0.9473  |  0.9365   | 0.9219 |  0.9291  |
| Logistic Regression  | 0.9473  |  0.9365   | 0.9219 |  0.9291  |
| Naive Bayes          | 0.9415  |  0.8857   | 0.9688 |  0.9254  |
| Random Forest        | 0.9356  |  0.9206   | 0.9062 |  0.9134  |
| SVC                  | 0.9532  |  0.9242   | 0.9531 |  0.9385  |
| Decision Tree        | 0.9590  |  0.9385   | 0.9531 |  0.9457  |


## 6. 🧠 En İyi Performansı Veren Model

Bu çalışmada en yüksek başarı oranına ulaşan model:

**➡️ (Decision Tree)**

## 7. 🔧 Nasıl Kullanılır?

Projeyi kendi bilgisayarınızda çalıştırmak için aşağıdaki adımları izleyebilirsiniz:

1. Depoyu klonlayın:
   ```bash
   git clone git@github.com:Harungokc/Canser.git
   cd Canser

👨‍💻 Katkıda Bulunma
Projeye katkıda bulunmak isterseniz fork edip pull request gönderebilirsiniz. Model performanslarını iyileştirme önerileri veya veri seti çeşitlendirmeleri her zaman memnuniyetle karşılanır.





