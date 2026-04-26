# Bayesyen Laboratuvarı - Parlaklık Analizi

## Amaç
Bu projede, Bayesyen çıkarım ve MCMC yöntemi kullanılarak uzak bir galaksinin gerçek parlaklığı (μ) ve belirsizliği (σ) tahmin edilmektedir.



## Sonuçlar

- μ (ortalama parlaklık):
  ≈ 150  
  Güven aralığı: [147, 152]

- σ (gürültü / hata):
  ≈ 10  
  Güven aralığı: [8.5, 12.5]



## Yorum

Bayesyen model gerçek değerlere oldukça yakın sonuçlar vermiştir:

- Tahmin edilen μ değeri gerçek değer olan 150’ye çok yakındır  
- Gözlem sayısı arttıkça belirsizlik azalmaktadır  
- Model gürültüyü başarılı şekilde yönetmektedir  



## Analiz Soruları

### 1. Prior Etkisi
Eğer çok dar bir prior seçilirse (örneğin 100–110 arası), model gerçek değere ulaşamaz ve sonuçlar hatalı olur.



### 2. Veri Miktarı Etkisi
Gözlem sayısı azaltılırsa (n_obs = 5), belirsizlik artar ve posterior dağılım genişler.



### 3. Korelasyon
Corner plot grafiğinde μ ve σ arasında zayıf bir korelasyon görülmektedir (elips şekli dikine yakındır).


## Sonuç

Bayesyen çıkarım, gürültülü verilerde bile doğru ve güvenilir parametre tahmini sağlar.
