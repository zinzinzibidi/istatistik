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
* <a href="#kartiller-arasi-fark">Sheppard Düzeltmesi</a>
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

<strong>R</strong>: Range, Değişim Aralığı, <strong>X<sub>max</sub></strong>: Serinin en büyük değeri, <strong>X<sub>min</sub></strong>: Serinin en küçük değeri

> Excel’de değişim aralığını bulmak için =MAK()-MİN() formülünü kullanabiliriz.

<br>

<strong>Uygulama</strong>: Bir sınıftan seçilen 10 öğrencinin sınav notları aşağıda verilmiştir.

$$ x = 40, 55, 60, 60, 65, 70, 75, 80, 85, 90 $$

Notların değişim aralığını bulunuz.

<br>

$$ R = x_{max} - x_{min} = 90 - 40 = 50 $$

Serinin en büyük değeri 90, en küçük değeri 40’tır. İki değer arasındaki mesafe (range), değişim aralığını vermektedir.

<br>

---

### Kartiller Arası Fark (IQR)

Kartiller Arası Fark (Interquartile Range, IQR)[^3] ya da Çeyrekler Arası Açıklığı serinin %75. dilimine denk gelen Q<sub>3</sub> kartili ve %25. dilime denk gelen Q<sub>1</sub> kartili arasındaki farkı belirtmektedir.

#### Anakütle ve Örneklem Kartiller Arası Farkı

<div align="center">Tüm Serilerde</div>

$$ IQR = Q_3 - Q_1 $$

<p align="center">
  <img src="https://zinzinzibidi.com/img/istatistik/kartiller-arasi-fark.png" style="width: 480px;"/>
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

<br>

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

$$ MAD = { { |40 - 68| + |55 - 68| \ + ... + \ |85 - 68| + |90 - 68| } \over 10 } $$

$$ MAD = { { 23 + 13 + ... +\ 17 + 22 } \over 10 } = 12 \text{ puan} $$

<br>

<strong>Uygulama</strong>: Bir sınıftaki tüm öğrencilerin boy uzunlukları tabloda listelenmiştir.

<table align="center">
  <tr>
    <th>Boy Uzunluğu</th>
    <th>Öğrenci Sayısı</th>
  </tr>
  <tr align="center">
    <td>155 cm</td>
    <td>1</td>
  </tr>
  <tr align="center">
    <td>160 cm</td>
    <td>2</td>
  </tr>
  <tr align="center">
    <td>165 cm</td>
    <td>7</td>
  </tr>
  <tr align="center">
    <td>170 cm</td>
    <td>16</td>
  </tr>
  <tr align="center">
    <td>175 cm</td>
    <td>18</td>
  </tr>
  <tr align="center">
    <td>180 cm</td>
    <td>6</td>
  </tr>
  <tr align="center">
    <td>185 cm</td>
    <td>4</td>
  </tr>
  <tr align="center">
    <td>190 cm</td>
    <td>1</td>
  </tr>
  <tr align="center">
    <td>Toplam (Σ)</td>
    <td>55</td>
  </tr>
</table>

Boy uzunluklarının ortalama mutlak sapmasını (MAD’ini) bulunuz.

<br>

Öncelikle aritmetik ortalamayı buluruz.

<table align="center">
  <tr>
    <th>Boy Uzunluğu (X<sub>i</sub>)</th>
    <th>Öğrenci Sayısı (f<sub>i</sub>)</th>
    <th>X<sub>i</sub>f<sub>i</sub></th>
  </tr>
  <tr align="center">
    <td>155 cm</td>
    <td>1</td>
    <td>155</td>
  </tr>
  <tr align="center">
    <td>160 cm</td>
    <td>2</td>
    <td>320</td>
  </tr>
  <tr align="center">
    <td>165 cm</td>
    <td>7</td>
    <td>1155</td>
  </tr>
  <tr align="center">
    <td>170 cm</td>
    <td>16</td>
    <td>2720</td>
  </tr>
  <tr align="center">
    <td>175 cm</td>
    <td>18</td>
    <td>3150</td>
  </tr>
  <tr align="center">
    <td>180 cm</td>
    <td>6</td>
    <td>1080</td>
  </tr>
  <tr align="center">
    <td>185 cm</td>
    <td>4</td>
    <td>740</td>
  </tr>
  <tr align="center">
    <td>190 cm</td>
    <td>1</td>
    <td>190</td>
  </tr>
  <tr align="center">
    <td>Toplam (Σ)</td>
    <td>55</td>
    <td>9510</td>
  </tr>
</table>

$$ \mu = {\Sigma X_i f_i \over N} $$

$$ \mu = {155 + 320 + 1155 + 2720 + 3150 + 180 + 740 + 190 \over 55} = 172.91 \approx 173 \text{ cm} $$

Ardından ortalama mutlak sapmayı (MAD’i) hesaplarız.

<table align="center">
  <tr>
    <th>Boy Uzunluğu (X<sub>i</sub>)</th>
    <th>Öğrenci Sayısı (f<sub>i</sub>)</th>
    <th>f<sub>i</sub>|X<sub>i</sub>-µ|</th>
  </tr>
  <tr align="center">
    <td>155 cm</td>
    <td>1</td>
    <td>1|155-173|</td>
  </tr>
  <tr align="center">
    <td>160 cm</td>
    <td>2</td>
    <td>2|160-173|</td>
  </tr>
  <tr align="center">
    <td>165 cm</td>
    <td>7</td>
    <td>7|165-173|</td>
  </tr>
  <tr align="center">
    <td>170 cm</td>
    <td>16</td>
    <td>16|170-173|</td>
  </tr>
  <tr align="center">
    <td>175 cm</td>
    <td>18</td>
    <td>18|175-173|</td>
  </tr>
  <tr align="center">
    <td>180 cm</td>
    <td>6</td>
    <td>6|180-173|</td>
  </tr>
  <tr align="center">
    <td>185 cm</td>
    <td>4</td>
    <td>4|185-173|</td>
  </tr>
  <tr align="center">
    <td>190 cm</td>
    <td>1</td>
    <td>1|190-173|</td>
  </tr>
  <tr align="center">
    <td>Toplam (Σ)</td>
    <td>55</td>
    <td>351</td>
  </tr>
</table>

$$ MAD = { { \Sigma f_i|X_i - \mu| } \over \Sigma f_i } = { 351 \over 55 } = 6.38 \approx 6 \text{ cm} $$

<br>

<strong>Uygulama</strong>: Bir sınıftaki tüm öğrencilerin boy uzunlukları tabloda listelenmiştir.

<table align="center">
  <tr>
    <th>Boy Uzunluğu</th>
    <th>Öğrenci Sayısı</th>
  </tr>
  <tr align="center">
    <td>150 – 159 cm</td>
    <td>4</td>
  </tr>
  <tr align="center">
    <td>160 – 169 cm</td>
    <td>12</td>
  </tr>
  <tr align="center">
    <td>170 – 179 cm</td>
    <td>36</td>
  </tr>
  <tr align="center">
    <td>180 – 189 cm</td>
    <td>8</td>
  </tr>
  <tr align="center">
    <td>190 – 200 cm</td>
    <td>2</td>
  </tr>
  <tr align="center">
    <td>Toplam (Σ)</td>
    <td>62</td>
  </tr>
</table>

Boy uzunluklarının ortalama mutlak sapmasını (MAD’ini) bulunuz.

<br>

Öncelikle ortalamayı buluruz.

<table align="center">
  <tr>
    <th>Boy Uzunluğu</th>
    <th>m<sub>i</sub></th>
    <th>Öğrenci Sayısı (f<sub>i</sub>)</th>
    <th>m<sub>i</sub>f<sub>i</sub></th>
  </tr>
  <tr align="center">
    <td>150 – 159 cm</td>
    <td>155 cm</td>
    <td>4</td>
    <td>620</td>
  </tr>
  <tr align="center">
    <td>160 – 169 cm</td>
    <td>165 cm</td>
    <td>12</td>
    <td>1980</td>
  </tr>
  <tr align="center">
    <td>170 – 179 cm</td>
    <td>175 cm</td>
    <td>36</td>
    <td>6300</td>
  </tr>
  <tr align="center">
    <td>180 – 189 cm</td>
    <td>185 cm</td>
    <td>8</td>
    <td>1480</td>
  </tr>
  <tr align="center">
    <td>190 – 200 cm</td>
    <td>195 cm</td>
    <td>2</td>
    <td>390</td>
  </tr>
  <tr align="center">
    <td>Toplam (Σ)</td>
    <td></td>
    <td>62</td>
    <td>10770</td>
  </tr>
</table>

$$ \mu = {\Sigma m_i f_i \over N} $$

$$ \mu = {(155 \times 4) + (165 \times 2) + (175 \times 36) + (185 \times 8) + (195 \times 2) \over 62} = 173.71 \approx 174 \text{ cm} $$

Ardından ortalama mutlak sapmayı (MAD’i) hesaplarız.

<table align="center">
  <tr>
    <th>Boy Uzunluğu</th>
    <th>m<sub>i</sub></th>
    <th>Öğrenci Sayısı (f<sub>i</sub>)</th>
    <th>f<sub>i</sub>|m<sub>i</sub>-µ|</th>
  </tr>
  <tr align="center">
    <td>150 – 159 cm</td>
    <td>155 cm</td>
    <td>4</td>
    <td>4|155 – 174|</td>
  </tr>
  <tr align="center">
    <td>160 – 169 cm</td>
    <td>165 cm</td>
    <td>12</td>
    <td>12|165 – 174|</td>
  </tr>
  <tr align="center">
    <td>170 – 179 cm</td>
    <td>175</td>
    <td>36</td>
    <td>36|175 – 174|</td>
  </tr>
  <tr align="center">
    <td>180 – 189 cm</td>
    <td>185 cm</td>
    <td>8</td>
    <td>8|185 – 174|</td>
  </tr>
  <tr align="center">
    <td>190 – 200 cm</td>
    <td>195 cm</td>
    <td>2</td>
    <td>2|195 – 174|</td>
  </tr>
  <tr align="center">
    <td>Toplam (Σ)</td>
    <td></td>
    <td>62</td>
    <td>350</td>
  </tr>
</table>

$$ MAD = { { \Sigma f_i|m_i - \mu| } \over \Sigma f_i } = { 350 \over 62 } = 5.65 \approx 6 \text{ cm} $$

<br>

---

### Standart Sapma (SD) ve Varyans

Standart Sapma (Standart Deviation, SD, STDEV) gözlem değerlerinin aritmetik ortalamadan sapmalarının kareli ortalamasıdır. Standart sapmanın karesi ise Varyans (Variance, VAR) olarak adlandırılır.

En çok kullanılan ve en önemli dağılım ölçüsüdür. Açık uçlu dağılımlar için hesaplanamaz.

Anakütle için <strong>σ</strong> (küçük sigma), örneklem için <strong>s</strong> notasyonu ile gösterilir.

#### Anakütle Standart Sapması

<div align="center">Basit Serilerde</div>

$$ \sigma = \sqrt{ { \Sigma (X_i - \mu)^2 } \over N } $$

<div align="center">Frekans Serilerinde</div>

$$ \sigma = \sqrt{ { \Sigma f_i(X_i - \mu)^2 } \over N } $$

<div align="center">Gruplandırılmış Serilerde</div>

$$ \sigma = \sqrt{ { \Sigma f_i(m_i - \mu)^2 } \over N } $$

#### Örneklem Standart Sapması

<div align="center">Basit Serilerde</div>

$$ s = \sqrt{ { \Sigma (x_i - \bar x)^2 } \over n } $$

<div align="center">Frekans Serilerinde</div>

$$ s = \sqrt{ { \Sigma f_i(x_i - \bar x)^2 } \over n } $$

<div align="center">Gruplandırılmış Serilerde</div>

$$ s = \sqrt{ { \Sigma f_i(m_i - \bar x)^2 } \over n } $$

<strong>m</strong>: Sınıf Orta Sayısı, <strong>f</strong>: Frekans, <strong>σ</strong>: Anakütle Standart Sapması, <strong>s</strong>: Örneklem Standart Sapması

Formüller biraz daha detaylı yazılırsa…

#### Anakütle Standart Sapması

<div align="center">Basit Serilerde</div>

$$ \sigma = \sqrt{ { \Sigma (X_i - { {\Sigma X_i } \over N })^2 } \over N } $$

<div align="center">Frekans Serilerinde</div>

$$ \sigma = \sqrt{ { \Sigma (X_i - { {\Sigma X_i f_i } \over N })^2 } \over N } $$

<div align="center">Gruplandırılmış Serilerde</div>

$$ \sigma = \sqrt{ { \Sigma (X_i - { {\Sigma m_i f_i } \over N })^2 } \over N } $$

#### Örneklem Standart Sapması

<div align="center">Basit Serilerde</div>

$$ s = \sqrt{ { \Sigma (x_i - { {\Sigma x_i } \over n })^2 } \over n } $$

<div align="center">Frekans Serilerinde</div>

$$ s = \sqrt{ { \Sigma (x_i - { {\Sigma x_i f_i } \over n })^2 } \over n }  $$

<div align="center">Gruplandırılmış Serilerde</div>

$$ s = \sqrt{ { \Sigma (x_i - { {\Sigma m_i f_i } \over n })^2 } \over n }  $$

<p align="center">
  <img src="https://zinzinzibidi.com/img/istatistik/normal-dagilim.png" style="width: 480px;"/>
</p>

Normal dağılım grafikleri[^5] standart sapma ile hesaplanmaktadır. Ortalamanın 0 (sıfır) alınması durumunda “standart normal dağılım” olarak adlandırılmaktadır. Normal dağılımda 68-95-99.7 Kuralı adlı verilen özel bir kural geçerlidir. Bu kurala göre ortalamadan ±1σ (artı eksi 1 standart sapma) uzaklığa kadar olan alan, tüm olasılıkların %68.2’sini, ±2σ uzaklığa kadar olan alan %95.4’ünü, ±3σ uzaklığa kadar olan alan ise %99.6’sını kapsamaktadır. İlerleyen konularda normal dağılım detaylıca anlatılacak olup standart sapmanın tüm dağılım ölçüleri içerisinde neden en önemli ölçü olduğu dağılımı grafiklerinden de anlaşılabilir.

Varyans, standart sapmanın karesi olmakla birlikte anakütle için σ<sup>2</sup>, örneklem içinse s<sup>2</sup> notasyonu ile gösterilir. Basit serilerde varyansı formülize etmek istersek

#### Anakütle için

$$ \sigma^2 = { { \Sigma(X_i - \mu)^2 } \over N } $$

#### Örneklem için

$$ s^2 = { { \Sigma(x_i - \bar x)^2 } \over n } $$

şeklinde gösterebiliriz. Örneklem hacminin 40’tan küçük olduğu serilerde n yerine (n-1) kullanılmalıdır.[^6]

<strong>n ≤ 40</strong> ise standart sapmanın formülü şu şekilde olmaktadır:

$$ s = \sqrt{ { \Sigma(x_i - \bar x)^2 } \over n - 1 } $$

> Excel’de anakütle standart sapmasını hesaplamak için =STDSAPMA.P(), örneklem standart sapmasını hesaplamak içinse =STDSAPMA.S() formüllerini kullanabiliriz.

<br>

<strong>Uygulama</strong>: Bir sınıftan seçilen 10 öğrencinin sınav notları aşağıda verilmiştir.

$$ x = 40, 55, 60, 60, 65, 70, 75, 80, 85, 90 $$

Notların standart sapmasını bulunuz.

<br>

Standart sapmayı bulmak için öncelikle ortalamayı bulmalıyız.

$$ \bar x = {\Sigma x_i \over n} $$

$$ \bar x = {40 + 55 + 60 + 60 + 65 + 70 + 75 + 80 + 85 + 90 \over 10} = 68 $$

Standart sapmayı hesapladığımızda

$$ s = \sqrt{ { \Sigma(x_i - \bar x)^2 } \over n - 1 } $$

$$ s = \sqrt{ { (40-68)^2 + (55-68)^2\,+\,...\,+\,(85-68)^2+(90-68)^2 } \over 10 - 1 } $$

$$ s = \sqrt{ 2090 \over 9 } = \sqrt{228.89} = 15.13 \approx 15 \text{ puan} $$

sonucunu elde ederiz. Dikkat ederseniz gözlem değerlerimiz 40’tan küçüktür. n ≤ 40 olduğu için payda kısmını n yerine n – 1 aldık.

<br>

<strong>Uygulama</strong>: Bir sınıftaki tüm öğrencilerin boy uzunlukları tabloda listelenmiştir.

<table align="center">
  <tr>
    <th>Boy Uzunluğu</th>
    <th>Öğrenci Sayısı</th>
  </tr>
  <tr align="center">
    <td>155 cm</td>
    <td>1</td>
  </tr>
  <tr align="center">
    <td>160 cm</td>
    <td>2</td>
  </tr>
  <tr align="center">
    <td>165 cm</td>
    <td>7</td>
  </tr>
  <tr align="center">
    <td>170 cm</td>
    <td>16</td>
  </tr>
  <tr align="center">
    <td>175 cm</td>
    <td>18</td>
  </tr>
  <tr align="center">
    <td>180 cm</td>
    <td>6</td>
  </tr>
  <tr align="center">
    <td>185 cm</td>
    <td>4</td>
  </tr>
  <tr align="center">
    <td>190 cm</td>
    <td>1</td>
  </tr>
  <tr align="center">
    <td>Toplam (Σ)</td>
    <td>55</td>
  </tr>
</table>

Boy uzunluklarının standart sapmasını bulunuz.

Öncelikle aritmetik ortalamayı buluruz.

<table align="center">
  <tr>
    <th>Boy Uzunluğu (X<sub>i</sub>)</th>
    <th>Öğrenci Sayısı (f<sub>i</sub>)</th>
    <th>X<sub>i</sub>f<sub>i</sub></th>
  </tr>
  <tr align="center">
    <td>155 cm</td>
    <td>1</td>
    <td>155</td>
  </tr>
  <tr align="center">
    <td>160 cm</td>
    <td>2</td>
    <td>320</td>
  </tr>
  <tr align="center">
    <td>165 cm</td>
    <td>7</td>
    <td>1155</td>
  </tr>
  <tr align="center">
    <td>170 cm</td>
    <td>16</td>
    <td>2720</td>
  </tr>
  <tr align="center">
    <td>175 cm</td>
    <td>18</td>
    <td>3150</td>
  </tr>
  <tr align="center">
    <td>180 cm</td>
    <td>6</td>
    <td>1080</td>
  </tr>
  <tr align="center">
    <td>185 cm</td>
    <td>4</td>
    <td>740</td>
  </tr>
  <tr align="center">
    <td>190 cm</td>
    <td>1</td>
    <td>190</td>
  </tr>
  <tr align="center">
    <td>Toplam (Σ)</td>
    <td>55</td>
    <td>9510</td>
  </tr>
</table>

$$ \mu = {\Sigma X_i f_i \over N} $$

$$ \mu = {155 + 320 + 1155 + 2720 + 3150 + 180 + 740 + 190 \over 55} = 172.91 \approx 173 \text{ cm} $$

Ardından standart sapmayı hesaplarız.

<table align="center">
  <tr>
    <th>Boy Uzunluğu (X<sub>i</sub>)</th>
    <th>Öğrenci Sayısı (f<sub>i</sub>)</th>
    <th>f<sub>i</sub>(X<sub>i</sub>-µ)<sup>2</sup></th>
  </tr>
  <tr align="center">
    <td>155 cm</td>
    <td>1</td>
    <td>1(155-173)<sup>2</sup></td>
  </tr>
  <tr align="center">
    <td>160 cm</td>
    <td>2</td>
    <td>2(160-173)<sup>2</sup></td>
  </tr>
  <tr align="center">
    <td>165 cm</td>
    <td>7</td>
    <td>7(165-173)<sup>2</sup></td>
  </tr>
  <tr align="center">
    <td>170 cm</td>
    <td>16</td>
    <td>16(170-173)<sup>2</sup></td>
  </tr>
  <tr align="center">
    <td>175 cm</td>
    <td>18</td>
    <td>18(175-173)<sup>2</sup></td>
  </tr>
  <tr align="center">
    <td>180 cm</td>
    <td>6</td>
    <td>6(180-173)<sup>2</sup></td>
  </tr>
  <tr align="center">
    <td>185 cm</td>
    <td>4</td>
    <td>4(185-173)<sup>2</sup></td>
  </tr>
  <tr align="center">
    <td>190 cm</td>
    <td>1</td>
    <td>1(190-173)<sup>2</sup></td>
  </tr>
  <tr align="center">
    <td>Toplam (Σ)</td>
    <td>55</td>
    <td>2485</td>
  </tr>
</table>

$$ \sigma = \sqrt{ { \Sigma f_i(X_i - \mu)^2 } \over N } = \sqrt{2485 \over 55} = \sqrt{45.15} = 6.72 \approx 7 \text{ cm} $$

<br>

<strong>Uygulama</strong>: Bir sınıftaki tüm öğrencilerin boy uzunlukları tabloda listelenmiştir.

<table align="center">
  <tr>
    <th>Boy Uzunluğu</th>
    <th>Öğrenci Sayısı</th>
  </tr>
  <tr align="center">
    <td>150 – 159 cm</td>
    <td>4</td>
  </tr>
  <tr align="center">
    <td>160 – 169 cm</td>
    <td>12</td>
  </tr>
  <tr align="center">
    <td>170 – 179 cm</td>
    <td>36</td>
  </tr>
  <tr align="center">
    <td>180 – 189 cm</td>
    <td>8</td>
  </tr>
  <tr align="center">
    <td>190 – 200 cm</td>
    <td>2</td>
  </tr>
  <tr align="center">
    <td>Toplam (Σ)</td>
    <td>62</td>
  </tr>
</table>

Boy uzunluklarının standart sapmasını bulunuz.

<br>

Öncelikle ortalamayı buluruz.

Öncelikle ortalamayı buluruz.

<table align="center">
  <tr>
    <th>Boy Uzunluğu</th>
    <th>m<sub>i</sub></th>
    <th>Öğrenci Sayısı (f<sub>i</sub>)</th>
    <th>m<sub>i</sub>f<sub>i</sub></th>
  </tr>
  <tr align="center">
    <td>150 – 159 cm</td>
    <td>155 cm</td>
    <td>4</td>
    <td>620</td>
  </tr>
  <tr align="center">
    <td>160 – 169 cm</td>
    <td>165 cm</td>
    <td>12</td>
    <td>1980</td>
  </tr>
  <tr align="center">
    <td>170 – 179 cm</td>
    <td>175 cm</td>
    <td>36</td>
    <td>6300</td>
  </tr>
  <tr align="center">
    <td>180 – 189 cm</td>
    <td>185 cm</td>
    <td>8</td>
    <td>1480</td>
  </tr>
  <tr align="center">
    <td>190 – 200 cm</td>
    <td>195 cm</td>
    <td>2</td>
    <td>390</td>
  </tr>
  <tr align="center">
    <td>Toplam (Σ)</td>
    <td></td>
    <td>62</td>
    <td>10770</td>
  </tr>
</table>

m<sub>i</sub> sınıf orta sayısını belirtmektedir. (150 + 160) / 2 = 155 cm

$$ \mu = {\Sigma m_i f_i \over N} $$

$$ \mu = {(155 \times 4) + (165 \times 2) + (175 \times 36) + (185 \times 8) + (195 \times 2) \over 62} = 173.71 \approx 174 cm $$

Ardından standart sapmayı hesaplarız.

<table align="center">
  <tr>
    <th>Boy Uzunluğu</th>
    <th>m<sub>i</sub></th>
    <th>Öğrenci Sayısı (f<sub>i</sub>)</th>
    <th>f<sub>i</sub>(m<sub>i</sub>-µ)<sup>2</sup></th>
  </tr>
  <tr align="center">
    <td>150 – 159 cm</td>
    <td>155 cm</td>
    <td>4</td>
    <td>4(155 – 174)<sup>2</sup></td>
  </tr>
  <tr align="center">
    <td>160 – 169 cm</td>
    <td>165 cm</td>
    <td>12</td>
    <td>12(165 – 174)<sup>2</sup></td>
  </tr>
  <tr align="center">
    <td>170 – 179 cm</td>
    <td>175</td>
    <td>36</td>
    <td>36(175 – 174)<sup>2</sup></td>
  </tr>
  <tr align="center">
    <td>180 – 189 cm</td>
    <td>185 cm</td>
    <td>8</td>
    <td>8(185 – 174)<sup>2</sup></td>
  </tr>
  <tr align="center">
    <td>190 – 200 cm</td>
    <td>195 cm</td>
    <td>2</td>
    <td>2(195 – 174)<sup>2</sup></td>
  </tr>
  <tr align="center">
    <td>Toplam (Σ)</td>
    <td></td>
    <td>62</td>
    <td>4302</td>
  </tr>
</table>

$$ \sigma = \sqrt{ { \Sigma f_i(m_i - \mu)^2 } \over N } = \sqrt{4302 \over 62} = \sqrt{69.39} = 8.33 \approx 8 \text{ cm} $$

<br>

<span id="sheppard-duzeltmesi"></span>

---

### Sheppard Düzeltmesi

Düzeltilmiş Standart Sapma ya da Sheppard Düzeltmesi (Sheppard’s Correction) sınıflandırılmış (gruplandırılmış) serilerde standart sapmanın hatalı hesaplanması sonucu William Fleetwood Sheppard[^7] tarafından geliştirilen standart sapmadır.

$$ \sigma^* = \sqrt{ \sigma^2 - { c^2 \over 12} } $$

<strong>σ<sup>*</sup></strong>: Sheppard Düzeltmesi (Düzeltilmiş Standart Sapma), <strong>c</strong>: Sınıf Aralığı

<br>

<strong>Uygulama</strong>: Bir önceki örneğimizde standart sapmayı 8.3299 (8.33) bulmuştuk. Sınıf aralığı (c) 10’dur.

Düzeltilmiş standart sapmayı aşağıdaki gibi hesaplarız.

$$ \sigma^* = \sqrt{ \sigma^2 - { c^2 \over 12} } = \sqrt{ 8.3299^2 - { 10^2 \over 12} } = \sqrt{ 69.3871 - { 100 \over 12} } $$

$$ = \sqrt{69.3871 - 8.33} = \sqrt{61.0538} = 7.81 \approx 8 \text{ cm} $$

Sheppard düzeltmesi yapılabilmesi için serinin normal ya da normale yakın dağılması, frekansların büyük ve serinin iki ucunun da asimptotik sıfıra yaklaşması gerekmektedir.



















[^1]: <a href="https://www.wikiwand.com/en/Statistical_dispersion" target="_blank">Statistical Dispersion</a> olarak da bilinir.

[^2]: Standart sapma kavramına birazdan değinilecektir.

[^3]: IQR için yabancı kaynaklarda midspread, middle 50%, H‑spread terimleri de kullanılmaktadır.

[^4]: Boxplot

[^5]: Normal distribution diagram

[^6]: Kimi kaynaklarda 30’dan küçük olması şartı aranmaktadır.

[^7]: 20 Kasım 1863 – 12 Ekim 1936 tarihleri arasında yaşayan Avustralyalı – İngiliz istatistikçi
