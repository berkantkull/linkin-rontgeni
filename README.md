# Linkin Röntgeni

[Canlı demoyu aç](https://berkantkull.github.io/linkin-rontgeni/)

Bir URL yapıştır, bilinen takip parametrelerini gör ve temiz bağlantıyı kopyala. Araç bağlantıları tarayıcında işler. Kurulum ve sunucu gerektirmez.

## Çalıştırma

`index.html` dosyasını tarayıcıda aç. **Örnek dene** düğmesi, paylaşılacak bağlantıda hangi bölümlerin korunduğunu gösterir.

GitHub Pages için dosyaları deponun köküne koy. GitHub'da **Settings → Pages → Deploy from a branch** altında ana dalın `/(root)` dizinini seç.

## Örnek

- Girdi: `https://example.com/yazi?dil=tr&utm_source=bulten&fbclid=ornek#kaynaklar`
- Çıktı: `https://example.com/yazi?dil=tr#kaynaklar`

Araç bilinen takip parametrelerini ve `utm_*` anahtarlarını kaldırır. Diğer parametrelerin sırasını ve kodlamasını, ayrıca `#` ile başlayan bölümü korur. Bir bağlantının imzası sorgu parametrelerini kapsıyorsa değişiklik imzayı geçersiz kılabilir. Tanınan anahtarlar `index.html` içindeki `trackingKeys` listesinde tutulur.
