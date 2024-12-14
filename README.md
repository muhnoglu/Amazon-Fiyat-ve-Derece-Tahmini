
# Amazon-Fiyat-ve-Derece-Tahmini
![Ekran görüntüsü 2024-12-14 193743](https://github.com/user-attachments/assets/4baecabd-88d3-4dea-8a74-907502b3e9d6)




Proje Özeti ve Modelleme Süreci
Bu projede, ürünlerin özelliklerinden faydalanarak iki ana görev gerçekleştirildi:

# Kategorilerin Ortalama Rating Değerlerine Göre Sınıflandırma:

Kategorilerin, ürünlerin rating değerlerinin ortalamalarına dayalı olarak sınıflandırılması gerçekleştirildi. Bu işlemde, Random Forest sınıflandırıcı modeli kullanıldı.
Bu model ile, her bir kategoriye ait ortalama rating değeri tahmin edilerek, ürünler için 'rating_class' sınıfları belirlendi.

# Ürünlerin Gerçek Fiyatlarının Tahmini:
Random Forest Regressor modeli kullanılarak, ürünlerin gerçek fiyatlarının tahmini yapıldı. Bağımsız değişkenler (features) olarak, discounted_price, category_encoded, weighted_rating, rating, ve rating_count gibi özellikler kullanıldı.
Modelin doğruluğu, test veri seti üzerinde yapılan değerlendirme sonuçlarıyla ölçüldü.
# Model Değerlendirme Sonuçları
# 1. Kategorilerin Ortalama Rating Değerlerinin Sınıflandırılması (Random Forest Sınıflandırıcı)
Modelin doğruluk oranı (Accuracy): Bu model, tüm test verileri üzerinde %100 doğruluk (Validation Accuracy: 1.0) sağladı.

# Sınıflandırma performansı:

Bu başarı, kategorilerin ortalama rating değerlerinin doğru şekilde tahmin edilmesine olanak tanıdı ve modelin iyi bir genel performans sergilediğini gösteriyor.
# 2. Ürünlerin Gerçek Fiyatlarının Tahmini (Random Forest Regressor)
Mean Absolute Error (MAE): 544.57

Modelin tahmin ettiği fiyat ile gerçek fiyatlar arasındaki ortalama mutlak farktır. Yüksek MAE, modelin tahminlerinin gerçek fiyatlardan belirli bir miktarda sapma gösterdiğini ifade eder.
Mean Squared Error (MSE): 951813.60

MSE, tahmin hatalarının karesinin ortalamasını alarak modelin genel hatalarını gösterir. Yüksek MSE, modelin hatalarının büyüklüğüne işaret eder.
Root Mean Squared Error (RMSE): 975.61

RMSE, MSE'nin karekökünü alarak daha anlaşılır bir ölçüt sunar. Yüksek RMSE değeri, modelin fiyat tahminlerindeki hataların büyüklüğünü gözler önüne serer.
R-squared (R²): 0.90

Modelin tahminlerinin gerçek fiyatlarla ne kadar uyumlu olduğunu gösteren R² değeri, %90.1'lik bir uyum sağlamaktadır. Bu, modelin büyük ölçüde başarılı olduğunu ve verilerin büyük bir kısmını doğru tahmin ettiğini gösteriyor.
# Sonuç ve Değerlendirme
Kategorilerin Rating Değerlerinin Tahmini: Random Forest sınıflandırma modeli ile kategori başına ortalama rating değeri tahmin edilmesi çok başarılı bir şekilde gerçekleştirildi. Modelin %100 doğruluk oranı, sınıflandırmanın doğru yapıldığını göstermektedir.

Fiyat Tahmini (Regresyon): Random Forest Regressor modeli, ürünlerin fiyatlarını tahmin etmekte iyi bir performans gösterdi. R-squared değeri %90.1 olan model, fiyat tahminlerinde yüksek doğruluk sağlamaktadır. Ancak, tahmin hatalarının büyüklüğünü yansıtan MAE, MSE ve RMSE metrikleri, bazı sapmalar olduğunu göstermektedir. Bu, modelin belirli durumlarda fiyat tahminlerinde hata yapabileceğini gösterir.
 # Kaggle:https://www.kaggle.com/code/muhammedhanolu/amazon-fiyat-ve-derece-tahmini
