# Dağılım Ölçüleri

Yayılım ya da Değişkenlik Ölçüleri olarak da adlandırılan Dağılım Ölçüleri (measure of dispersion)[^1] veri birimlerinin genelinin ortalamadan ne kadar uzak ya da ortalamaya ne kadar yakın olduğunu gösteren temel ölçülerden biridir. Merkezî eğilim ölçülerinden olan aritmetik ortalama, mod ve medyan her zaman serinin heterojen ya da homojen dağıldığını göstermemektedir. Bu sebeple serinin dağılımı hakkında merkezî eğilim ölçülerine göre daha anlamlı sonuçlar veren standart sapma ve değişim katsayısı gibi dağılım ölçüleri kullanılır.

<p align="center">
  <img src="https://zinzinzibidi.com/img/istatistik/dagilim-olculeri2.png" style="width: 600px;"/>
</p>

Yukarıdaki grafikte kişi başına günlük harcama tutarlarını gösteren iki gruba ait veriler dağılım grafiğinde gösterilmiştir. İki grubun da kişi başına günlük ortalama harcaması 100 TL olmasına rağmen kırmızı grubun standart sapması[^2] 10 TL iken mavi grubun standart sapması 50 TL’dir. Bu sebeple iki grubun da aynı karakteristik özelliklere sahip olduğunu söyleyemeyiz. İki grubu birbiri ile karşılaştırmak için dağılım ölçülerinden yararlanırız.

## Dağılım Ölçüleri

* Değişim Aralığı (Range)
* Kartiller Arası Fark (IQR)
* Ortalama Mutlak Sapma (MAD)
* Standart Sapma (SD) ve Varyans
* Sheppard Düzeltmesi
* Standart Hata
* Değişim Katsayısı (CV)
* Kutu Diyagramı (Box-Plot)

### Değişim Aralığı

Değişim Aralığı ya da Ranj (Range), en kolay anlaşılan dağılım ölçüsü olmakla birlikte uygulaması da en kolay yayılım ölçüsüdür. Aykırı değerlerden hemen etkilenir ve açık uçlu dağılımlar için hesaplanamaz.

#### Anakütle Değişim Aralığı

<div align="center">Tüm Serilerde</div>

$$ R = X_{max} - X_{min} $$

#### Örneklem Değişim Aralığı

<div align="center">Tüm Serilerde</div>

$$ R = x_{max} - x_{min} $$

R: Range, Değişim Aralığı

X<sub>max</sub>: Serinin en büyük değeri

X<sub>min</sub>: Serinin en küçük değeri

> Excel’de değişim aralığını bulmak için =MAK()-MİN() formülünü kullanabiliriz.

<strong>Uygulama</strong>: Bir sınıftan seçilen 10 öğrencinin sınav notları aşağıda verilmiştir.

$$ x = 40, 55, 60, 60, 65, 70, 75, 80, 85, 90 $$

Notların değişim aralığını bulunuz.

<br>

$$ R = x_{max} - x_{min} = 90 - 40 = 50 $$

Serinin en büyük değeri 90, en küçük değeri 40’tır. İki değer arasındaki mesafe (range), değişim aralığını vermektedir.

---

### Kartiller Arası Fark (IQR)










[^1]: <a href="https://www.wikiwand.com/en/Statistical_dispersion" target="_blank">Statistical Dispersion</a> olarak da bilinir.

[^2]: Standart sapma kavramına birazdan değinilecektir.

