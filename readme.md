# 💳 Kredi Başvurusu Tahmini – Makine Öğrenmesi Projesi

Bu proje, bireylerin kredi başvurularının onaylanıp onaylanmayacağını tahmin etmek amacıyla yapılmıştır.  
Veri seti Almanya'daki başvuru sahiplerine ait anonim bilgiler içeriyor ve sınıflandırma algoritmaları kullanılarak analiz edildi.

---

## 🎯 Projenin Amacı

Bankalar, kredi verirken başvuru sahibinin riskini değerlendirir.  
Bu projede, verilen bazı finansal ve kişisel bilgilere bakarak bir başvurunun **kredi alıp almayacağını tahmin etmeye çalıştık**.

---

## 📁 Kullanılan Veri Seti

- **Kaynak:** [UCI German Credit Data](https://archive.ics.uci.edu/ml/datasets/statlog+(german+credit+data))
- **Toplam Gözlem:** 1000
- **Hedef Değişken:** `Kredi Onayı` (1 = Onaylandı, 0 = Reddedildi)

---

## 🔧 Uygulanan Adımlar

- Veriyi inceledim ve kategorik verileri uygun şekilde dönüştürdüm (`get_dummies` ile).
- Eğitim ve test verisini ayırdım (%80 / %20).
- KNN ve SVM için standartlaştırma uyguladım (`StandardScaler`).
- 3 farklı sınıflandırma algoritması denedim:
  - Random Forest ✅
  - K-Nearest Neighbors
  - Support Vector Machine

---

## 📊 Sonuçlar

En iyi sonucu `Random Forest` verdi. Accuracy değeri yaklaşık **%79.5** oldu.

| Model                | Accuracy |
|---------------------|----------|
| Random Forest       | **79.5% ✅** |
| KNN                 | 75.0%    |
| SVM                 | 78.0%    |
  
Feature importance grafiği ile modelin hangi değişkenlere daha çok dikkat ettiğini de gözlemledim.

---

## 🧪 Kullanılan Kütüphaneler

- `pandas`, `numpy`
- `scikit-learn` (modelleme ve değerlendirme)
- `matplotlib`, `seaborn` (görselleştirme)

---

## 📌 Dosya Yapısı

kredi-basvuru-tahmin/
│
├── main.ipynb # Model oluşturma dosyası
├── german_credit_data.csv
├──classification_report.txt
├── random_forest_model.pkl # Eğitilmiş modelin kaydı
└── README.md # Proje açıklaması


---

## 🙋🏻‍♂️ Neden Bu Projeyi Yaptım?

Veri bilimi yolculuğumda sınıflandırma modellerini gerçek bir veri seti üzerinde denemek istedim.  
Kredi başvurusu gibi bir konunun hem iş dünyasında hem de teknik anlamda önemli olduğunu düşündüm.  
Proje boyunca model performansını nasıl iyileştirebileceğimi ve veri ön işleme sürecinin ne kadar kritik olduğunu daha iyi anladım.

---

## 👨‍💻 Hazırlayan

**Şura Kaya**  
Bilgisayar Mühendisliği 3. sınıf öğrencisi  
Veri bilimi, yapay zekâ ve yazılım geliştirme alanlarına ilgim var.
 
