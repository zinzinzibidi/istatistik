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

<br>

<strong>Uygulama</strong>: Bir sınıftan seçilen 10 öğrencinin sınav notları aşağıda verilmiştir.

$$ x = 40, 55, 60, 60, 65, 70, 75, 80, 85, 90 $$

Notların değişim aralığını bulunuz.

<br>

$$ R = x_{max} - x_{min} = 90 - 40 = 50 $$

Serinin en büyük değeri 90, en küçük değeri 40’tır. İki değer arasındaki mesafe (range), değişim aralığını vermektedir.

---

### Kartiller Arası Fark (IQR)

Kartiller Arası Fark (Interquartile Range, IQR)[^3] ya da Çeyrekler Arası Açıklığı serinin %75. dilimine denk gelen Q<sub>3</sub> kartili ve %25. dilime denk gelen Q<sub>1</sub> kartili arasındaki farkı belirtmektedir.

#### Anakütle ve Örneklem Kartiller Arası Farkı

<div align="center">Tüm Serilerde</div>

$$ IQR = Q_3 - Q_1 $$

<p align="center">
  <img src="https://zinzinzibidi.com/img/istatistik/kartiller-arasi-fark.png" style="width: 600px;"/>
</p>

Kartiller Arası Fark (IQR) çoğunlukla kutu grafiklerinde[^4] yoğun olarak kullanılmakla birlikte olasılık yoğunluk fonkisyonu ve standart normal dağılım grafiklerinde dağılımın %50’sini oluşturmaktadır.

> Excel’de Kartiller Arası Fark almak için =DÖRTTEBİRLİK(seri;3)-DÖRTTEBİRLİK(seri;1) hesaplamasını yapabiliriz.

<br>

<strong>Uygulama</strong>: X<sub>1</sub> = 12, 14, 14, 16, 18, 18, 18, 18, 18, 20, 24 serisinin kartiller arası farkını (IQR'ını) bulunuz.

<br>

n: 11’dir. Gözlem sayısı tek sayı olduğu için

$$ Q_1 = { X_{ { N+2 } \over 4 } } = { X_{ { 11+2 } \over 4 } } = X_{3.25} \approx X_3 = 14 $$

$$ Q_3 = { X_{ { 3N+2 } \over 4 } } = { X_{ { 3(11)+2 } \over 4 } } = X_{8.75} \approx X_9 = 18 $$

$$ IQR = Q_3 - Q_1 = 18 - 14 = 4 $$

---

### Ortalama Mutlak Sapma (MAD)

Ortalama Mutlak Sapma (Mean Absolute Deviation, MAD), verilerin ortalamadan sapmalarının mutlak değerlerinin ortalamasıdır. Bu dağılım ölçüsünde her gözlemin sapmasına eşit ağırlık tanınır ve standart sapma kadar aykırı değerlerden etkilenmez. Kimi durumlarda ortalama yerine medyan da kullanılabilmektedir.

#### Anakütle Ortalama Mutlak Sapması

<div align="center">Basit Serilerde</div>

$$ MAD = { { \Sigma|X_i - \mu| } \over N } $$

<div align="center">Frekans Serilerinde</div>

$$ MAD = { { \Sigma f_i|X_i - \mu| } \over \Sigma f_i } $$

<div align="center">Gruplandırılmış Serilerde</div>

$$ MAD = { { \Sigma f_i|m_i - \mu| } \over \Sigma f_i } $$

#### Örneklem Ortalama Mutlak Sapması

<div align="center">Basit Serilerde</div>

$$ MAD = { { \Sigma|x_i - \bar x| } \over n }  $$

<div align="center">Frekans Serilerinde</div>

$$ MAD = { { \Sigma f_i|x_i - \bar x| } \over \Sigma f_i } $$

<div align="center">Gruplandırılmış Serilerde</div>

$$ MAD = { { \Sigma f_i|m_i - \bar x| } \over \Sigma f_i } $$

m: Sınıf Orta Sayısı, f: Frekans

> Excel’de ortalama mutlak sapmanın formülü bulunmamaktadır. Buna rağmen mutlak değerleri hesaplarken
=MUTLAK() formülünü kullanabiliriz.

<br>

Uygulama</strong>: Bir sınıftan seçilen 10 öğrencinin sınav notları aşağıda verilmiştir.

$$ x = 40, 55, 60, 60, 65, 70, 75, 80, 85, 90 $$

Notların ortalama mutlak sapmasını (MAD’ini) bulunuz.

<br>

Öncelikle aritmetik ortalamayı buluruz.

$$ \bar x = { { \Sigma x_i } \over n } $$

$$ \bar x = { { 40+55+60+60+65+70+75+80+85+90 } \over 10 } = 68 $$

Ardından ortalama mutlak sapmayı (MAD’i) hesaplarız.

$$ MAD = { { \Sigma|x_i - \bar x| } \over n } $$

$$ MAD = { { |40 - 68| + |55 - 68|\, +\, ... +\, |85 - 68| + |90 - 68| } \over 10 } $$

$$ MAD = { { 23 + 13\, +\, ... +\, 17 + 22 } \over 10 } = 12 \text{ puan} $$

<br>

<strong>Uygulama</strong>: Bir sınıftaki tüm öğrencilerin boy uzunlukları tabloda listelenmiştir.












[^1]: <a href="https://www.wikiwand.com/en/Statistical_dispersion" target="_blank">Statistical Dispersion</a> olarak da bilinir.

[^2]: Standart sapma kavramına birazdan değinilecektir.

[^3]: IQR için yabancı kaynaklarda midspread, middle 50%, H‑spread terimleri de kullanılmaktadır.

[^4]: Boxplot
