# 🌫️ Hava Kalitesinin Sağlık Üzerindeki Etkisi

Bu proje, hava kirliliği verilerinin insan sağlığı üzerindeki etkilerini analiz etmeyi ve sınıflandırmayı amaçlamaktadır. Kaggle üzerinden temin edilen veri seti üzerinde çeşitli veri ön işleme adımları uygulanmış ve farklı makine öğrenmesi modelleri ile tahminleme yapılmıştır.

## 🗂️ Veri Seti Bilgisi
- **Kaynak**: [Kaggle Hava Kalitesi Verisi](https://www.kaggle.com/datasets/rabieelkharoua/air-quality-and-health-impact-dataset)
Veri seti bir `.csv` dosyası şeklinde olup toplam **5811 kayıt** içermektedir.

### 📌 Özellikler (Features)

| Kategori | Değişken | Açıklama |
|----------|----------|----------|
| **Kayıt Bilgisi** | `RecordID` | Her kayıt için benzersiz ID |
| **Hava Kalitesi** | `AQI` | Hava Kalitesi Endeksi |
| | `PM10` | 10 µm'den küçük partikül madde (μg/m³) |
| | `PM2_5` | 2.5 µm'den küçük partikül madde (μg/m³) |
| | `NO2` | Azot dioksit yoğunluğu (ppb) |
| | `SO2` | Kükürt dioksit yoğunluğu (ppb) |
| | `O3` | Ozon yoğunluğu (ppb) |
| **Hava Durumu** | `Temperature` | Sıcaklık (°C) |
| | `Humidity` | Nem (%) |
| | `WindSpeed` | Rüzgar hızı (m/s) |
| **Sağlık Verisi** | `RespiratoryCases` | Solunum vakası sayısı |
| | `CardiovascularCases` | Kardiyovasküler vakalar |
| | `HospitalAdmissions` | Hastane başvuruları |
| **Hedef Değişken** | `HealthImpactScore` | 0–100 arasında sağlık etki skoru |
| | `HealthImpactClass` | 0: Çok Yüksek, 1: Yüksek, 2: Orta, 3: Düşük, 4: Çok Düşük |

## 🧹 Veri Analizi ve Ön İşleme

- Eksik verilerin analizi ve doldurulması
- Yanlış değerlerin tespiti ve temizlenmesi
- Korelasyon analizi ve özellik seçimi
- Sınıf dağılımının incelenmesi
- Normalizasyon ve ölçekleme işlemleri

### 📊 Görselleştirmeler

- **Sınıf Dağılımı**: Her bir `HealthImpactClass` için örnek sayısı
- **Korelasyon Matrisi**: Değişkenler arası ilişki görselleştirmesi (heatmap)

## 🤖 Kullanılan Modeller

- `Random Forest Classifier`
- `Decision Tree Classifier`
- `Logistic Regression`
- `K-Nearest Neighbors`
- `TensorFlow` ile yapay sinir ağı (Neural Network)

### 🎯 Performans Ölçütleri

- Accuracy
- Precision, Recall, F1-Score

## ⚙️ Kurulum

Projeyi çalıştırmak için:

```bash
git clone https://github.com/aysenurgulsum/air_quality_health_impact_analysis.git
cd air_quality_health_impact_analysis
