#  Amazon Sales Forecasting: Prophet vs. ARIMA

This project analyzes Amazon India sales data to predict future sales performance. It compares a modern machine learning approach (**Prophet**) with a traditional statistical method (**ARIMA**).

##  Project Overview
The study involves time series decomposition (trend, seasonality, residuals) and forecasting for a 30-day horizon. Accurate forecasting is crucial for inventory management and financial planning in e-commerce operations.

##  Model Performance Comparison
Based on backtesting results, the error metrics (RMSE and MAE) for both models are as follows:

| Metric | Prophet Model | ARIMA(1, 0, 1) Model |
| :--- | :--- | :--- |
| **RMSE (Root Mean Squared Error)** | 239,944.38 | 291,220.89 |
| **MAE (Mean Absolute Error)** | 192,605.65 | 234,312.45 |

###  Key Insights
* **Accuracy:** The Prophet model outperformed ARIMA with an approximately **17.6% lower RMSE**.
* **Seasonality:** Prophet was superior in capturing weekly cycles and sudden fluctuations inherent in e-commerce data.
* **Stability:** While ARIMA provided a more conservative trend line, Prophet modeled the data "noise" more effectively, resulting in a more realistic projection.

##  Tech Stack
* **Python 3.x**
* **Pandas & NumPy:** Data manipulation
* **Prophet:** Time series forecasting library by Meta
* **Statsmodels:** ARIMA modeling and statistical testing (ADF test)
* **Matplotlib & Seaborn:** Data visualization

##  Featured Visuals
* **ACF & PACF Plots:** Identification of ARIMA parameters (p, d, q).
* **Seasonal Decomposition:** Breakdown of trend, seasonality, and residuals.
* **Model Comparison:** Visualizing the 30-day sales projections of both models.

##  Conclusion
Given the dynamic and volatile nature of e-commerce sales, the **Prophet** model proved to be more adept at understanding seasonal effects and providing more reliable forecasts with lower error margins.



---TURKİSH---

# Amazon Sales Forecasting: Prophet vs. ARIMA

Bu proje, Amazon Hindistan satış verilerini kullanarak gelecekteki satış performansını tahmin etmek amacıyla gerçekleştirilmiştir. Proje kapsamında modern makine öğrenmesi yaklaşımlarından **Prophet** ve geleneksel istatistiksel yöntemlerden **ARIMA** modelleri karşılaştırılmıştır.

## Proje Özeti
Satış verileri üzerinde zaman serisi analizi yapılarak mevsimsellik, trend ve hata payları incelenmiştir. Özellikle e-ticaret operasyonlarında stok yönetimi ve finansal planlama için kritik olan "gelecek 30 gün" projeksiyonu oluşturulmuştur.

## Model Performans Karşılaştırması
Yapılan Backtesting çalışmaları sonucunda modellerin hata payları (RMSE ve MAE) aşağıdaki gibi saptanmıştır:

| Metrik | Prophet Modeli | ARIMA(1, 0, 1) Modeli |
| :--- | :--- | :--- |
| **RMSE (Root Mean Squared Error)** | 239,944.38 | 291,220.89 |
| **MAE (Mean Absolute Error)** | 192,605.65 | 234,312.45 |

### Analiz Sonuçları
* **Hata Oranı:** Prophet modeli, ARIMA'ya göre yaklaşık **%17.6 daha düşük hata payı** (RMSE) ile çalışmaktadır.
* **Mevsimsellik:** Prophet, e-ticaret verilerindeki haftalık döngüleri ve ani dalgalanmaları yakalamada daha başarılı olmuştur.
* **Stabilite:** ARIMA modeli daha muhafazakar bir trend çizerken, Prophet verideki gürültüyü (noise) daha iyi modelleyerek gerçeğe daha yakın zikzaklar oluşturmuştur.

##  Kullanılan Teknolojiler
* **Python 3.x**
* **Pandas & NumPy:** Veri manipülasyonu
* **Prophet:** Facebook tarafından geliştirilen zaman serisi kütüphanesi
* **Statsmodels:** ARIMA modelleme ve istatistiksel testler (ADF test)
* **Matplotlib & Seaborn:** Veri görselleştirme

##  Öne Çıkan Görseller
* **ACF & PACF Grafik:** ARIMA parametrelerinin (p, d, q) belirlenmesi.
* **Seasonal Decomposition:** Trend, mevsimsellik ve artıkların ayrıştırılması.
* **Model Comparison:** İki modelin gelecek 30 günlük satış projeksiyonunun kıyaslanması.

##  Sonuç
E-ticaret verilerinin dinamik ve değişken yapısı göz önüne alındığında, **Prophet** modelinin mevsimsel etkileri daha iyi kavradığı ve daha düşük hata payı ile daha güvenilir tahminler sunduğu sonucuna varılmıştır.

--HAZIRLAYAN--
Edanur DEMİREL
