# 🛠️ Vida Üretim Süreci: İstatistiksel Analiz ve Outlier Tespiti

Bu proje, bir üretim bandından çıkan vida boylarını Python ile simüle ederek **Normal Dağılım** ve **Aykırı Değer (Outlier)** yönetimi üzerine yapılmış bir çalışmadır.

## 🧐 Karşılaşılan Problem
Analizin ilk aşamasında, ham verideki aykırı değerlerin (7.5mm, 13mm gibi uç değerler) standart sapmayı yapay olarak şişirdiği görülmüştür. Bu durum, teorik Normal Dağılım eğrisinin (PDF) gerçek verilerle örtüşmemesine ve basık görünmesine neden olmuştur.

## 🧪 Uygulanan Çözüm
- **Veri Temizleme:** John Tukey'in **1.5 IQR (Interquartile Range)** kuralı kullanılarak aykırı değerler veri setinden arındırılmıştır.
- **İstatistiksel Doğrulama:** Temizleme sonrası Kurtosis değeri ideal seviyeye yaklaşmış ve standart sapma gerçek değerine çekilmiştir.
- **Sonuç:** Veri temizlendikten sonra teorik eğri ile gerçek üretim verilerinin tam uyum sağladığı kanıtlanmıştır.

## 📊 Teknik Detaylar
- **Kütüphaneler:** Pandas, NumPy, Matplotlib, Scipy.
- **Yöntem:** Outlier Detection (IQR Method) & PDF Visualization.
