
# Kimya Tesisi Reaksiyon Verimi Optimizasyonu

Bu proje, bir kimya tesisindeki reaksiyon verimini maksimize etmek için **Genetik Algoritma (GA)** kullanımını göstermektedir.

## 📝 Problem Tanımı
Kimyasal üretimde reaksiyon süresi ve sıcaklık ayarı verimi doğrudan etkilemektedir. 
Proje, belirli kısıtlar altında en ideal parametreleri bulmayı amaçlar.

### Matematiksel Model
- **Amaç Fonksiyonu (Verim):** $y = 8x_1 + 3x_2 - x_1x_2 + x_1^2$
- **Değişkenler:**
  - $x_1$: Reaksiyon süresi (10 - 60 dk)
  - $x_2$: Sıcaklık (40 - 120 °C)
- **Kısıtlar:**
  - $x_1 + x_2 \leq 140$
  - $x_2 \geq 60$

## 🚀 Kullanılan Teknolojiler
- Python 3
- [PyGAD](https://pygad.readthedocs.io/) (Genetik Algoritma Kütüphanesi)
- Matplotlib (Görselleştirme)
- NumPy

## 📊 Algoritma Parametreleri
- **Popülasyon:** 50
- **Nesil (Generation):** 100
- **Seçilim:** Steady State Selection (SSS)
- **Mutasyon Oranı:** %10

## 📈 Sonuç
Algoritma, nesiller ilerledikçe kısıtları ihlal etmeden verimi artıran en iyi değerleri bulmuş ve kararlı bir noktaya (convergence) ulaşmıştır.
"""
