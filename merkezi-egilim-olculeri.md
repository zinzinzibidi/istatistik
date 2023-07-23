# Merkezî Eğilim Ölçüleri

Veri kümesinin ortasını belirlemeye yönelik ölçülerin tümüne merkezî eğilim ölçüsü (measure of central tendency) denir. Adından da anlaşılacağı üzere amaç, veri setinin ne yöne doğru eğilim gösterdiğini tespit etmektir. Bu eğilimi tespit etmek içinse ortalamalar kullanılmaktadır.

Ortalama denilince birçoğumuzun aklına aritmetik ortalama gelmektedir. Fakat istatistikte geometrik ve harmonik ortalama, mod, medyan gibi kimi durumlarda daha anlamlı sonuçlar veren ortalamalar da bulunmaktadır.

Duyarlı ortalamalar serideki aykırı değerlerden etkilenirken duyarlı olmayan ortalamalar etkilenmemektedir.

## Duyarlı Ortalamalar

* Aritmetik Ortalama
* Geometrik Ortalama
* Harmonik Ortalama
* Kareli Ortalama
* Ağırlıklık Ortalama
* Duyarlı Ortalamaların Karşılaştırılması
* SPSS'te Duyarlı Ortalamalar

## Duyarlı Olmayan Ortalamalar

* Medyan
* Mod
* Kartil
* Desil ve Persantil
* Düzeltilmiş Ortalama
* Kırpılmış Ortalama
* SPSS'te Duyarlı Olmayan Ortalamalar

### Aritmetik Ortalama

Aritmetik Ortalama (Arithmetic Mean), en bilinen ve en çok kullanılan ortalama türüdür. Seriyi oluşturan tüm değerlerin toplanıp gözlem sayısına bölünmesi ile bulunur.

Anakütlede <b>µ</b> (mü), örneklemde <b>x̄</b> (x üzeri çizgi, x-bar) notasyonu kullanılır.

<b>Σ</b> toplamı, <b>N</b> anakütlede, <b>n</b> örneklemde gözlem sayısını belirtir.

#### Anakütle Aritmetik Ortalaması

<div align="center">Basit Serilerde</div>

$$ \mu = {\Sigma X_i \over N} $$

<div align="center">Frekans Serilerinde</div>

$$ \mu = {\Sigma X_i f_i \over N} $$

<div align="center">Gruplandırılmış Serilerde</div>

$$ \mu = {\Sigma m_i f_i \over N} $$

#### Örneklem Aritmetik Ortalaması

<div align="center">Basit Serilerde</div>

$$ \bar x = {\Sigma x_i \over n}$$

<div align="center">Frekans Serilerinde</div>

$$ \bar x = {\Sigma x_i f_i \over n} $$

<div align="center">Gruplandırılmış Serilerde</div>

$$ \bar x = {\Sigma m_i f_i \over n} $$

<b>m</b>: Sınıf Orta Sayısı, <b>f</b>: Frekans

> Excel’de aritmetik ortalama almak için =ORTALAMA() formülünü kullanabiliriz.

<br>

<b>Uygulama</b>: Bir sınıftan seçilen 10 öğrencinin sınav notları aşağıda verilmiştir.

$$ x = 40, 55, 60, 60, 65, 70, 75, 80, 85, 90 $$

Notların aritmetik ortalamasını bulunuz.

$$ \bar x = {\Sigma x_i \over n}  $$

$$ \bar x = {40 + 55 + 60 + 60 + 65 + 70 + 75 + 80 + 85 + 90 \over 10} = 68 $$

<br>

<b>Uygulama</b>: Bir sınıftaki tüm öğrencilerin boy uzunlukları tabloda listelenmiştir.

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

Boy uzunluklarının aritmetik ortalamasını bulunuz.

<br>

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

<br>

<b>Uygulama</b>: Bir sınıftaki tüm öğrencilerin boy uzunlukları tabloda listelenmiştir.

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

Boy uzunluklarının aritmetik ortalamasını bulunuz.

<br>

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
    <td>175</td>
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

Sınıf aralıklarında son değer aralığa dahil, başlangıç değeri dahil değildir. 160 – 170 cm aralığı gerçekte 160’dan değil 160.0000…001’den başlamaktadır. 170.000…000’da bitmektedir.

$$ \mu = {\Sigma m_i f_i \over N} $$

$$ \mu = {(155 \times 4) + (165 \times 2) + (175 \times 36) + (185 \times 8) + (195 \times 2) \over 62} = 173.71 \approx 174 \text{ cm} $$

---

### Geometrik Ortalama

Geometrik Ortalama (Geometric Mean), serinin gözlem değerlerine eşit dereceden ortalamasıdır. Aykırı değerlerden[^1] daha az etkilenmesi sebebiyle aritmetik ortalamadan daha anlamlıdır. Buna rağmen seride sıfır ya da negatif değer olması durumunda kullanılamamaktadır.

#### Anakütle Geometrik Ortalaması

<div align="center">Basit Serilerde</div>

$$ \text{Geo Ort} = \sqrt[N]{X_1X_2...X_N} $$

$$ \text{Log Geo Ort} = {\Sigma logX_i \over N} $$

<div align="center">Frekans Serilerinde</div>

$$ \text{Log Geo Ort} = {\Sigma f_ilogX_i \over \Sigma f_i} $$

<div align="center">Gruplandırılmış Serilerde</div>

$$ \text{Log Geo Ort} = {\Sigma f_ilogm_i \over \Sigma f_i}  $$

#### Örneklem Geometrik Ortalaması

<div align="center">Basit Serilerde</div>

$$ \text{Geo Ort} = \sqrt[n]{x_1x_2...x_n} $$

$$ \text{Log Geo Ort} = {\Sigma logx_i \over n} $$

<div align="center">Frekans Serilerinde</div>

$$ \text{Log Geo Ort} = {\Sigma f_ilogx_i \over \Sigma f_i} $$

<div align="center">Gruplandırılmış Serilerde</div>

$$ \text{Log Geo Ort} = {\Sigma f_ilogm_i \over \Sigma f_i} $$

<b>m</b>: Sınıf Orta Sayısı, <b>f</b>: Frekans

Logaritmik geometrik ortalamanın antilogaritması geometrik ortalamayı vermektedir.

> Excel’de geometrik ortalama almak için =GEOORT() formülünü kullanabiliriz.

<br>

<b>Uygulama</b>: 10 hastanın kan tahlili sonuçları aşağıdaki gibidir.

$$ x = 84, 244, 246, 248, 248, 250, 251, 252, 254, 1486 $$

Kan tahlili sonuçlarının geometrik ortalamasını bulunuz.

$$ \text{Log Geo Ort} = {\Sigma logx_i \over n} $$

$$ \text{Log Geo Ort} = {log(84) + log(244) + log(246)\,+\,\,...\,+\,log(252) + log(254) + log(1486) \over 10} $$

$$ \text{Log Geo Ort} = 2.43  $$

$$ \text{AntiLog Geo Ort} = \text{Geo Ort} = 267.14 \approx 267 $$

Antilog alırken hesap makinemizde 10<sup>Log Geo Ort</sup> işlemini yapabiliriz. Diğer bir ifade ile 10 üzeri (Logaritmik Geometrik Ortalama) işlemini yapmaktayız. (10<sup>2.43</sup> = 267.14)

Seri 84 ve 1486 olmak üzere iki aykırı değer (outlier) içermektedir. Aritmetik ortalama 356’dır ve geometrik ortalama 267 bulunmuştur. Verilerin çoğunluğu 244 ve 254 arasında dağılırken aritmetik ortalama (356) seriyi istatistiksel olarak anlamlı temsil etmemektedir. Geometrik ortalama nispeten daha anlamlıdır.

<br>

<b>Uygulama</b>: Anket sorularına verilen cevapların puan tablosu aşağıdaki gibidir.

<table align="center">
  <tr>
    <th>Puan</th>
    <th>Yanıt Sayısı</th>
  </tr>
  <tr align="center">
    <td>1</td>
    <td>12</td>
  </tr>
  <tr align="center">
    <td>2</td>
    <td>24</td>
  </tr>
  <tr align="center">
    <td>3</td>
    <td>30</td>
  </tr>
  <tr align="center">
    <td>4</td>
    <td>64</td>
  </tr>
  <tr align="center">
    <td>5</td>
    <td>145</td>
  </tr>
  <tr align="center">
    <td>Toplam (Σ)</td>
    <td>275</td>
  </tr>
</table>

Puanların geometrik ortalamasını bulunuz.

<br>

<table align="center">
  <tr>
    <th>Puan (X<sub>i</sub>)</th>
    <th>Yanıt Sayısı (f<sub>i</sub>)</th>
    <th>f<sub>i</sub>*log(X<sub>i</sub>)</th>
  </tr>
  <tr align="center">
    <td>1</td>
    <td>12</td>
    <td>12*log(1)</td>
  </tr>
  <tr align="center">
    <td>2</td>
    <td>24</td>
    <td>24*log(2)</td>
  </tr>
  <tr align="center">
    <td>3</td>
    <td>30</td>
    <td>30*log(3)</td>
  </tr>
  <tr align="center">
    <td>4</td>
    <td>64</td>
    <td>64*log(4)</td>
  </tr>
  <tr align="center">
    <td>5</td>
    <td>145</td>
    <td>145*log(5)</td>
  </tr>
  <tr align="center">
    <td>Toplam (Σ)</td>
    <td>275</td>
    <td>161.42</td>
  </tr>
</table>

$$ \text{Log Geo Ort} = {\Sigma f_ilogX_i \over \Sigma f_i} = {161.42 \over 275} = 0.5870 $$

$$ \text{AntiLog Geo Ort} = \text{Geo Ort} = 3.8635 \approx 3.86 \text{ puan} $$

3.86 değeri 10<sup>0.5870</sup> ifadesi ile denktir.

<br>

<b>Uygulama</b>: 67 hastanın hematoloji sonuçları aşağıdaki gibidir. (Hematoloji: Kan bilimi, NEUT: Nötrofil)

<table align="center">
  <tr>
    <th>NEUT (k/uL)</th>
    <th>Hasta Sayısı</th>
  </tr>
  <tr align="center">
    <td>0.00 - 1.00</td>
    <td>1</td>
  </tr>
  <tr align="center">
    <td>1.00 - 2.00</td>
    <td>14</td>
  </tr>
  <tr align="center">
    <td>2.00 - 3.00</td>
    <td>22</td>
  </tr>
  <tr align="center">
    <td>3.00 - 4.00</td>
    <td>18</td>
  </tr>
  <tr align="center">
    <td>4.00 - 5.00</td>
    <td>9</td>
  </tr>
   <tr align="center">
    <td>5.00 - 6.00</td>
    <td>2</td>
  </tr>
   <tr align="center">
    <td>6.00 - 7.00</td>
    <td>1</td>
  </tr>
  <tr align="center">
    <td>Toplam (Σ)</td>
    <td>67</td>
  </tr>
</table>

Nötrofil sonuçlarının geometrik ortalamasını bulunuz.

<br>

<table align="center">
  <tr>
    <th>NEUT (k/uL)</th>
    <th>Sınıf Orta Sayısı (m<sub>i</sub>)</th>
    <th>Hasta Sayısı (f<sub>i</sub>)</th>
    <th>f<sub>i</sub>*log(m<sub>i</sub>)</th>
  </tr>
  <tr align="center">
    <td>0.00 - 1.00</td>
    <td>0.50</td>
    <td>1</td>
    <td>1*log(0.50)</td>
  </tr>
  <tr align="center">
    <td>1.00 - 2.00</td>
    <td>1.50</td>
    <td>14</td>
    <td>14*log(1.50)</td>
  </tr>
  <tr align="center">
    <td>2.00 - 3.00</td>
    <td>2.50</td>
    <td>22</td>
    <td>22*log(2.50)</td>
  </tr>
  <tr align="center">
    <td>3.00 - 4.00</td>
    <td>3.50</td>
    <td>18</td>
    <td>18*log(3.50)</td>
  </tr>
  <tr align="center">
    <td>4.00 - 5.00</td>
    <td>4.50</td>
    <td>9</td>
    <td>9*log(4.50)</td>
  </tr>
   <tr align="center">
    <td>5.00 - 6.00</td>
    <td>5.50</td>
    <td>2</td>
    <td>2*log(5.50)</td>
  </tr>
   <tr align="center">
    <td>6.00 - 7.00</td>
    <td>6.50</td>
    <td>1</td>
    <td>1*log(6.50)</td>
  </tr>
  <tr align="center">
    <td>Toplam (Σ)</td>
    <td></td>
    <td>67</td>
    <td>28.88</td>
  </tr>
</table>

$$ \text{Log Geo Ort} = {\Sigma f_ilogm_i \over \Sigma f_i} = {28.88 \over 67} = 0.4311 $$

$$ \text{AntiLog Geo Ort} = \text{Geo Ort} = 2.6985 \approx 2.70 \text{ k/uL} $$

<br>

#### Bileşik Faiz Hesaplamaları

Bileşik faiz formülünün temeli geometrik ortalamaya dayanmaktadır.

<table align="center">
  <tr>
    <th>Yıl</th>
    <th>Anapara</th>
    <th>Faiz Oranı</th>
    <th>Faiz Geliri</th>
  </tr>
  <tr align="center">
    <td>1</td>
    <td>1000</td>
    <td>%10</td>
    <td>100</td>
  </tr>
  <tr align="center">
    <td>2</td>
    <td>1100</td>
    <td>%20</td>
    <td>220</td>
  </tr>
  <tr align="center">
    <td>3</td>
    <td>1320</td>
    <td>%15</td>
    <td>198</td>
  </tr>
</table>

3. yılın sonunda Anapara + Faiz Geliri = 1320 + 198 = 1518 TL’dir. Sonuç olarak yatırımcı 1000 TL ile açtığı mevduat hesabından vade sonunda %51.8 getiri elde etmiştir.

$$ \text{Geo Ort} = \sqrt[n]{X_1X_2...X_n} $$

Geometrik ortalamayı yukarıdaki gibi ifade etmiştik. Formül aynı zamanda

$$ \text{Geo Ort} = (X_1X_2...X_n)^{1 \over n} $$

gösterimi ile aynıdır.

$$ \text{Bilesik Faiz} = [(1 + r_1)(1 + r_2)...(1 + r_n)]^{1 \over n} - 1 $$

<b>r</b>: faiz oranı, <b>n</b>: dönem sayısı

Dikkat edilirse geometrik ortalama ve bileşik faiz formülü birbirine çok benzemektedir. Bu sebeple bileşik faize aynı zamanda faiz oranlarının geometrik ortalaması diyebiliriz.

$$ \text{Bilesik Faiz} = [(1 + 0.10)(1 + 0.20)(1 + 0.15)]^{1 \over 3} - 1 = 1.518^{1 \over 3} - 1 \approx 0.1493 \approx \text{Yüzde} 14.93 $$

Parantez içindeki çarpımların sonucu 1.518’dir. Anapara + faiz gelirini ise 1518 TL hesaplamıştık. Çarpımdan 1 çıkartırsak (1.518 – 1) toplam faiz gelirin yüzdesini buluruz. (%51.8) Bulduğumuz %14.93 bileşik faiz oranının sağlamasını yapmak istersek

$$ \text{Bilesik Faiz} = [(1 + 0.1493)(1 + 0.1493)(1 + 0.1493)]^{1 \over 3} - 1 = 1.518^{1 \over 3} - 1 \approx 0.1493 \approx \text{Yüzde} 14.93 $$

aynı sonuca ulaşırız.

Yorumlanması şu şekildedir:

Yatırımcı 1000 TL anaparasını 3 yıl boyunca sırasıyla %10, %15 ve %20 faiz oranlarından bileşik faize yatırmak yerine %14.93 sabit oranı ile bileşik faize yatırırsa vade sonunda aynı getiriyi elde edecektir. (%51.8)

---

### Harmonik Ortalama

Harmonik Ortalama (Harmonic Mean), değişkenlerden birinin sabit, diğerinin sabit olmadığı durumlarda kullanılan, genellikle hız, fiyat ve verimlilik hesaplamalarında tercih edilen ortalama türüdür. Aykırı değerlerden en az etkilenen duyarlı ortalamadır. Hesaplanabilmesi için seride sıfır ve negatif değer olmamalıdır.

#### Anakütle Harmonik Ortalaması

<div align="center">Basit Serilerde</div>

$$ \text{Hrm Ort} = {N \over \Sigma {1 \over X_i}} $$

<div align="center">Frekans Serilerinde</div>

$$ \text{Hrm Ort} = {\Sigma f_i \over \Sigma {f_i \over X_i}} $$

<div align="center">Gruplandırılmış Serilerde</div>

$$ \text{Hrm Ort} = {\Sigma f_i \over \Sigma {f_i \over m_i}} $$

#### Örneklem Harmonik Ortalaması

<div align="center">Basit Serilerde</div>

$$ \text{Hrm Ort} = {n \over \Sigma {1 \over x_i}} $$

<div align="center">Frekans Serilerinde</div>

$$ \text{Hrm Ort} = {\Sigma f_i \over \Sigma {f_i \over x_i}} $$

<div align="center">Gruplandırılmış Serilerde</div>

$$ \text{Hrm Ort} = {\Sigma f_i \over \Sigma {f_i \over m_i}} $$

<b>m</b>: Sınıf Orta Sayısı, <b>f</b>: Frekans

> Excel’de harmonik ortalama almak için =HARORT() formülünü kullanabiliriz.

<br>

<b>Uygulama</b>: Bir araç A noktasından B noktasına sırasıyla 40, 60 ve 80 km/saat hızla gitmektedir. Aracın ortalama hızını bulunuz.

$$ \text{Hrm Ort} = {n \over \Sigma {1 \over x_i}} = {3 \over {1 \over 40} + {1 \over 60} + {1 \over 80}} = 55.38 \text{ km/saat}  $$

Diyelim ki A ve B noktası arasındaki mesafe 240 km olsun. Araç A ve B noktasına toplamda 3 kere gitmekte ve 240 * 3 = 720 km yol yapmaktadır. Toplam mesafeyi 720/55.38 = <b>13 saat</b>te tamamlamaktadır.

Yolda geçen süreyi tek tek hesapladığımızda 240/40 = 6 saat, 240/60 = 4 saat, 240/80 = 3 saat

6 + 4 + 3 = <b>13 saat</b> sonucuna varırız. Bu şekilde harmonik ortalamanın sağlamasını yapabiliriz.

Yorumlaması ise şu şekildedir:

Araç aynı yolu 40, 60 ve 80 km/saat hızlarla gitmek yerine 55.38 km/saat gibi sabit bir hızla giderse aynı sürede tamamlar.

<br>

<b>Uygulama</b>: Bir sınıftaki tüm öğrencilerin boy uzunlukları tabloda listelenmiştir.

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

Boy uzunluklarının harmonik ortalamasını bulunuz.

<br>

<table align="center">
  <tr>
    <th>Boy Uzunluğu (X<sub>i</sub>)</th>
    <th>Öğrenci Sayısı (f<sub>i</sub>)</th>
    <th>f<sub>i</sub>/X<sub>i</sub></th>
  </tr>
  <tr align="center">
    <td>155 cm</td>
    <td>1</td>
    <td>1/155</td>
  </tr>
  <tr align="center">
    <td>160 cm</td>
    <td>2</td>
    <td>2/160</td>
  </tr>
  <tr align="center">
    <td>165 cm</td>
    <td>7</td>
    <td>7/165</td>
  </tr>
  <tr align="center">
    <td>170 cm</td>
    <td>16</td>
    <td>16/170</td>
  </tr>
  <tr align="center">
    <td>175 cm</td>
    <td>18</td>
    <td>18/175</td>
  </tr>
  <tr align="center">
    <td>180 cm</td>
    <td>6</td>
    <td>6/180</td>
  </tr>
  <tr align="center">
    <td>185 cm</td>
    <td>4</td>
    <td>4/185</td>
  </tr>
  <tr align="center">
    <td>190 cm</td>
    <td>1</td>
    <td>1/190</td>
  </tr>
  <tr align="center">
    <td>Toplam (Σ)</td>
    <td>55</td>
    <td>0.32</td>
  </tr>
</table>

$$ \text{Hrm Ort} = {\Sigma f_i \over \Sigma {f_i \over X_i}} = { 55 \over 0.32} = 172.65 \approx 173 \text{ cm} $$

<br>

<b>Uygulama</b>: Bir sınıftaki tüm öğrencilerin boy uzunlukları tabloda listelenmiştir.

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

Boy uzunluklarının harmonik ortalamasını bulunuz.

<br>

<table align="center">
  <tr>
    <th>Boy Uzunluğu</th>
    <th>m<sub>i</sub></th>
    <th>Öğrenci Sayısı (f<sub>i</sub>)</th>
    <th>f<sub>i</sub>/m<sub>i</sub></th>
  </tr>
  <tr align="center">
    <td>150 – 159 cm</td>
    <td>155 cm</td>
    <td>4</td>
    <td>4/155</td>
  </tr>
  <tr align="center">
    <td>160 – 169 cm</td>
    <td>165 cm</td>
    <td>12</td>
    <td>12/165</td>
  </tr>
  <tr align="center">
    <td>170 – 179 cm</td>
    <td>175</td>
    <td>36</td>
    <td>36/165</td>
  </tr>
  <tr align="center">
    <td>180 – 189 cm</td>
    <td>185 cm</td>
    <td>8</td>
    <td>8/185</td>
  </tr>
  <tr align="center">
    <td>190 – 200 cm</td>
    <td>195 cm</td>
    <td>2</td>
    <td>2/195</td>
  </tr>
  <tr align="center">
    <td>Toplam (Σ)</td>
    <td></td>
    <td>62</td>
    <td>0.36</td>
  </tr>
</table>

$$ \text{Hrm Ort} = {\Sigma f_i \over \Sigma {f_i \over m_i}} = {62 \over 0.36} = 173.31 \approx 173 \text{ cm} $$

---

### Kareli Ortalama

Kareli Ortalama (Root Mean Square, RMS, Quadratic Mean), aritmetik ortalamaya benzemekle birlikte serideki 0 ve negatif değerleri nötralize etmek için kullanılan ortalama türüdür. Diğer bir ifade ile seride 0 veya negatif değerler göz ardı edilmek isteniyorsa kareli ortalama kullanılmalıdır.

#### Anakütle Kareli Ortalaması

<div align="center">Basit Serilerde</div>

$$ \text{Kareli Ort} = \sqrt { {\Sigma {X_i}^2} \over N } $$

<div align="center">Frekans Serilerinde</div>

$$ \text{Kareli Ort} = \sqrt { {\Sigma f_i{X_i}^2} \over \Sigma f_i }  $$

<div align="center">Gruplandırılmış Serilerde</div>

$$ \text{Kareli Ort} = \sqrt { {\Sigma f_i{m_i}^2} \over \Sigma f_i } $$

#### Örneklem Kareli Ortalaması

<div align="center">Basit Serilerde</div>

$$ \text{Kareli Ort} = \sqrt { {\Sigma {x_i}^2} \over n } $$

<div align="center">Frekans Serilerinde</div>

$$ \text{Kareli Ort} = \sqrt { {\Sigma f_i{x_i}^2} \over \Sigma f_i } $$

<div align="center">Gruplandırılmış Serilerde</div>

$$ \text{Kareli Ort} = \sqrt { {\Sigma f_i{m_i}^2} \over \Sigma f_i } $$

<b>m</b>: Sınıf Orta Sayısı, <b>f</b>: Frekans

> Excel’de kareli ortalamanın formülü bulunmamaktadır. =KAREKÖK(TOPKARE()/BAĞ_DEĞ_SAY()) formül kombinasyonu kullanılabilir.

<br>

<b>Uygulama</b>: Yedi günlük hava sıcaklığı değerleri aşağıda verilmiştir.

$$ x = -4, -2, 0, 4, 8, 13, 13 \text{ } ^{\circ}C $$

Sıcaklık değerlerinin kareli ortalamasını bulunuz.

<br>

$$ \text{Kareli Ort} = \sqrt { {\Sigma {x_i}^2} \over n } = \sqrt { { {-4}^2 + {-2}^2 \,+\,\,...\,+\, 13^2 + 13^2 } \over 7 } = \sqrt { 438 \over 7 } = 7.91 \approx 8^{\circ}C $$

<br>

<b>Uygulama</b>: Bir sınıftaki tüm öğrencilerin boy uzunlukları tabloda listelenmiştir.

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

Boy uzunluklarının kareli ortalamasını bulunuz.

<br>

<table align="center">
  <tr>
    <th>Boy Uzunluğu (X<sub>i</sub>)</th>
    <th>Öğrenci Sayısı (f<sub>i</sub>)</th>
    <th>f<sub>i</sub>*X<sub>i</sub><sup>2</sup></th>
  </tr>
  <tr align="center">
    <td>155 cm</td>
    <td>1</td>
    <td>1*155<sup>2</sup></td>
  </tr>
  <tr align="center">
    <td>160 cm</td>
    <td>2</td>
    <td>2*160<sup>2</sup></td>
  </tr>
  <tr align="center">
    <td>165 cm</td>
    <td>7</td>
    <td>7*165<sup>2</sup></td>
  </tr>
  <tr align="center">
    <td>170 cm</td>
    <td>16</td>
    <td>16*170<sup>2</sup></td>
  </tr>
  <tr align="center">
    <td>175 cm</td>
    <td>18</td>
    <td>18*175<sup>2</sup></td>
  </tr>
  <tr align="center">
    <td>180 cm</td>
    <td>6</td>
    <td>6*180<sup>2</sup></td>
  </tr>
  <tr align="center">
    <td>185 cm</td>
    <td>4</td>
    <td>4*185<sup>2</sup></td>
  </tr>
  <tr align="center">
    <td>190 cm</td>
    <td>1</td>
    <td>1*190<sup>2</sup></td>
  </tr>
  <tr align="center">
    <td>Toplam (Σ)</td>
    <td>55</td>
    <td>1,646,850</td>
  </tr>
</table>

$$ \text{Kareli Ort} = \sqrt { {\Sigma f_i{X_i}^2} \over \Sigma f_i } = \sqrt { 1646850 \over 55} = 173.04 \approx 173 \text{ cm} $$

<br>

<b>Uygulama</b>: Bir sınıftaki tüm öğrencilerin boy uzunlukları tabloda listelenmiştir.

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

Boy uzunluklarının kareli ortalamasını bulunuz.

<br>

<table align="center">
  <tr>
    <th>Boy Uzunluğu</th>
    <th>m<sub>i</sub></th>
    <th>Öğrenci Sayısı (f<sub>i</sub>)</th>
    <th>f<sub>i</sub>*m<sub>i</sub><sup>2</sup></th>
  </tr>
  <tr align="center">
    <td>150 – 159 cm</td>
    <td>155 cm</td>
    <td>4</td>
    <td>4*155<sup>2</sup></td>
  </tr>
  <tr align="center">
    <td>160 – 169 cm</td>
    <td>165 cm</td>
    <td>12</td>
    <td>12*165<sup>2</sup></td>
  </tr>
  <tr align="center">
    <td>170 – 179 cm</td>
    <td>175</td>
    <td>36</td>
    <td>36*165<sup>2</sup></td>
  </tr>
  <tr align="center">
    <td>180 – 189 cm</td>
    <td>185 cm</td>
    <td>8</td>
    <td>8*185<sup>2</sup></td>
  </tr>
  <tr align="center">
    <td>190 – 200 cm</td>
    <td>195 cm</td>
    <td>2</td>
    <td>2*195<sup>2</sup></td>
  </tr>
  <tr align="center">
    <td>Toplam (Σ)</td>
    <td></td>
    <td>62</td>
    <td>1,875,150</td>
  </tr>
</table>

$$ \text{Kareli Ort} = \sqrt { {\Sigma f_i{m_i}^2} \over \Sigma f_i } = \sqrt { 1875150 \over 62} = 173.91 \approx 174 \text{ cm} $$

---

### Ağırlıklı Ortalama

Ağırlıklı Ortalama (Weighted Mean) ya da Tartılı Aritmetik Ortalama finans alanında sıkça kullanılan duyarlı ortalamalardan biridir. Aralarındaki ilişkiden dolayı değişkenlerden biri ya da birkaçı ağırlıklandırılır, hesaplanmak istenen asıl değişkenin ortalaması bulunur. Özel durumlarda kullanılır ve diğer ortalama türlerine göre istatistiksel olarak daha anlamlıdır.

#### Anakütle Ağırlıklı Ortalaması

<div align="center">Basit Serilerde</div>

$$ \text{Agırlıklı Ort} = { {\Sigma w_iX_i} \over \Sigma X_i }$$

#### Örneklem Ağırlıklı Ortalaması

<div align="center">Basit Serilerde</div>

$$ \text{Agırlıklı Ort} = { {\Sigma w_ix_i} \over \Sigma x_i } $$

> Excel’de ağırlıklı ortalamanın formülü bulunmamaktadır. =TOPLA.ÇARPIM()/TOPLA() formül kombinasyonu kullanılabilir.

<br>

<b>Uygulama</b>: Aşağıda beş farklı mevduat hesabının tutarları ve faiz oranları verilmiştir.

<table align="center">
  <tr>
    <th>Hesap Numarası</th>
    <th>Tutar</th>
    <th>Faiz Oranı</th>
  </tr>
  <tr align="center">
    <td>A000001</td>
    <td>2,000,000</td>
    <td>10.20</td>
  </tr>
  <tr align="center">
    <td>A000002</td>
    <td>5,000,000</td>
    <td>10.40</td>
  </tr>
  <tr align="center">
    <td>A000003</td>
    <td>1,000,000</td>
    <td>10.10</td>
  </tr>
  <tr align="center">
    <td>A000004</td>
    <td>4,000,000</td>
    <td>10.30</td>
  </tr>
  <tr align="center">
    <td>A000005</td>
    <td>120,000,000</td>
    <td>11.10</td>
  </tr>
  <tr align="center">
    <td>Toplam (Σ)</td>
    <td>132,000,000 TL</td>
    <td></td>
  </tr>
</table>

Faiz oranlarının ağırlıklı ortalamasını bulunuz.

<br>

<table align="center">
  <tr>
    <th>Hesap Numarası</th>
    <th>Tutar (x<sub>i</sub>)</th>
    <th>Faiz Oranı (w<sub>i</sub>)</th>
    <th>Faiz Oranı (w<sub>i</sub>)*Tutar (x<sub>i</sub>)</th>
  </tr>
  <tr align="center">
    <td>A000001</td>
    <td>2,000,000</td>
    <td>10.20</td>
    <td>10.20*(2,000,000)</td>
  </tr>
  <tr align="center">
    <td>A000002</td>
    <td>5,000,000</td>
    <td>10.40</td>
    <td>10.40*(5,000,000)</td>
  </tr>
  <tr align="center">
    <td>A000003</td>
    <td>1,000,000</td>
    <td>10.10</td>
    <td>10.10*(1,000,000)</td>
  </tr>
  <tr align="center">
    <td>A000004</td>
    <td>4,000,000</td>
    <td>10.30</td>
    <td>10.30*(4,000,000)</td>
  </tr>
  <tr align="center">
    <td>A000005</td>
    <td>120,000,000</td>
    <td>11.10</td>
    <td>11.10*(120,000,000)</td>
  </tr>
  <tr align="center">
    <td>Toplam (Σ)</td>
    <td>132,000,000 TL</td>
    <td></td>
    <td>1,455,700,000 TL</td>
  </tr>
</table>

$$ \text{Agırlıklı Ort} = { {\Sigma w_ix_i} \over \Sigma x_i } = { 1,455,700,000 \over 132,000,000 } = 11.03 $$

Faiz oranlarının aritmetik ortalaması 10.42’dir ve istatistiksel olarak anlamlı değildir. İşlem tutarlarının büyük çoğunluğu (%91’lik kısmı oluşturan 132 milyon TL’lik hesap) 11.10 faiz oranı ile fiyatlanmıştır. Ortalamanın 11.10’a yakın olması beklenir. Bu sebeple 11.03 ağırlıklı ortalama faiz oranı, 10.42 aritmetik ortalamasına göre istatistiksel olarak daha anlamlıdır.

Finans dünyasında ağırlıklı ortalama TLREF (Türk Lirası Gecelik Referans Faiz Oranı) hesaplamasında kullanılmakta ve ticari kredilerin faiz oranını belirlemektedir.

---

### Duyarlı Ortalamaların Karşılaştırılması

Uygulamada çoğunlukla aritmetik ortalama kullanılsa da aykırı değerlerin yüksek olduğu serilerde geometrik ve harmonik ortalama tercih edilebilir. Geometrik ve harmonik ortalama hesaplamalarında seride negatif ve sıfır değerlerinin bulunmamasına dikkat edilmelidir. Ağırlıklı ortalama ise stok faiz oranı gibi özel durumlarda tercih edilen, basit serilerde kullanılamayan özel bir duyarlı ortalamadır.

$$ \text{Kareli Ort} \geq \text{Aritmetik Ort} \geq \text{Geometrik Ort} \geq \text{Harmonik Ort} $$

Tüm serilerde yukarıdaki büyüklük sıralaması geçerlidir. Harmonik ortalama aykırı değerlerden en az etkilenen duyarlı ortalama olmakla birlikte aykırı değerlerin yoğun olduğu serilerde kareli ortalama güvenirliği en az olan ortalama türüdür.

X<sub>1</sub> = 10, 10, 11, 11, 12, 12, 480 basit serisinin duyarlı ortalamaları hesaplandığında sırasıyla

$$ \text{Kareli Ort} \geq \text{Aritmetik Ort} \geq \text{Geometrik Ort} \geq \text{Harmonik Ort} $$

$$ 182 \geq 78 \geq 19 \geq 13 $$

ortalamaları bulunur. 480 aykırı değeri seriden çıkarıldığında serinin aritmetik ortalaması 11 olmaktadır. Bu sebeple aykırı değerin varlığı durumunda harmonik ortalama (13) seri ortalamasını istatistiksel olarak daha anlamlı ifade ettiği sonucuna varılabilir.

Seri karşılaştırmalarında harmonik ortalama istatistiksel olarak daha anlamlı iken aykırı değerlerin varlığı kabul edildiği durumlarda aritmetik ortalamanın kullanılmasında sakınca bulunmamaktadır. Bununla birlikte aykırı değerlerin yoğun olduğu serilerde medyan gibi duyarlı olmayan ortalamalar tercih edilmektedir. Günümüzde gini katsayısının yüksek olduğu ülkelerde medyan değerleri, kişi başına milli gelir karşılaştırmalarında aritmetik ortalamaya göre daha gerçekçi sonuçlar vermektedir.[^2]

---

### SPSS'te Duyarlı Ortalamalar

#### Aritmetik Ortalama

Sadece aritmetik ortalama bulunmak isteniyorsa aşağıdaki adımlar uygulanır.[^3]

<p align="center">
  <img src="https://zinzinzibidi.com/img/istatistik/spss-aritmetik-ortalama-01.png" style="width: 600px;"/>
</p>

Analyze > Descriptive Statistics > Descriptives… yolu izlenir.

<p align="center">
  <img src="https://zinzinzibidi.com/img/istatistik/spss-aritmetik-ortalama-02.png" style="width: 600px;"/>
</p>

İlgili değişken Variable(s)[^4] alanına taşınır. Options[^5]’a tıklanır.

<p align="center">
  <img src="https://zinzinzibidi.com/img/istatistik/spss-aritmetik-ortalama-03.png" style="width: 600px;"/>
</p>

Açılan pencerede sadece Mean[^6] seçilir.

<p align="center">
  <img src="https://zinzinzibidi.com/img/istatistik/spss-aritmetik-ortalama-04.png" style="width: 600px;"/>
</p>

OK'a tıklanır.

<p align="center">
  <img src="https://zinzinzibidi.com/img/istatistik/spss-aritmetik-ortalama-05.png" style="width: 600px;"/>
</p>

x<sub>1</sub> = 10, 10, 11, 11, 12, 12, 480 serisine ait aritmetik ortalamanın 78 olduğu bulunur.

<br>

#### Aritmetik, Geometrik ve Harmonik Ortalama

Aritmetik, geometrik ve harmonik ortalama birlikte bulunmak isteniyorsa aşağıdaki adımlar uygulanır.

<p align="center">
  <img src="https://zinzinzibidi.com/img/istatistik/spss-aritmetik-geometrik-harmonik-ortalama-01.png" style="width: 600px;"/>
</p>

Analyze > Reports > Case Summaries… yolu izlenir.

<p align="center">
  <img src="https://zinzinzibidi.com/img/istatistik/spss-aritmetik-geometrik-harmonik-ortalama-02.png" style="width: 600px;"/>
</p>

Display cases seçimi kaldırılır. (Kaldırılmadığı takdirde tüm seri değerleri rapora eklenecektir.)

Statistics…’e tıklanır.

<p align="center">
  <img src="https://zinzinzibidi.com/img/istatistik/spss-aritmetik-geometrik-harmonik-ortalama-03.png" style="width: 600px;"/>
</p>

Statistics listesinden Mean, Geometric Mean ve Harmonic Mean seçilir. Cell Statistics alanına aktarılır.

<p align="center">
  <img src="https://zinzinzibidi.com/img/istatistik/spss-aritmetik-geometrik-harmonik-ortalama-04.png" style="width: 600px;"/>
</p>

Summarize Cases penceresinde OK'a tıklanır.

<p align="center">
  <img src="https://zinzinzibidi.com/img/istatistik/spss-aritmetik-geometrik-harmonik-ortalama-05.png" style="width: 600px;"/>
</p>

Aritmetik, geometrik ve harmonik ortalamalar görseldeki gibi bulunur.

Aritmetik ortalama ve harmonik ortalama arasındaki fark ne kadar büyükse seride aykırı değerlerin varlığından söz edilebilir. Aykırı değerleri tespit edebilmek için Summarize Cases penceresinde “Display cases” kutusu seçilmelidir.

---

### Medyan

Medyan (Median) ya da Ortanca küçükten büyüğe sıralanmış veri dizisinin ortasındaki değeri ifade eden duyarlı olmayan ortalamadır. Aykırı değerlerin olduğu serilerde diğer ortalama türlerine göre daha güvenilirdir.

<b>x̃</b> işareti (x üzeri tilde) medyanın istatistikteki sembolüdür.

#### Anakütle Medyan Değeri

<div align="center">Gözlem Sayısının Tek Olduğu Basit Serilerde</div>

$$ \tilde X = {X_{N+1 \over 2}} $$

<div align="center">Gözlem Sayısının Çift Olduğu Basit Serilerde</div>

$$ \tilde X = { { X_{N\over 2} } + { X_{ { N\over 2}+1 } } \over 2} $$

<div align="center">Frekans Toplamının Tek Sayı Olduğu Frekans Serilerinde</div>

$$ \tilde X = { X_{ {(\Sigma f_i) + 1 } \over 2 } } $$

<div align="center">Frekans Toplamının Çift Sayı Olduğu Frekans Serilerinde</div>

$$ \tilde X = { { X_{ \Sigma f_i \over 2 } + X_{ { \Sigma f_i \over 2 } + 1 } } \over 2 } $$

<div align="center">Gruplandırılmış Serilerde</div>

$$ \tilde X = Low_{med} + { { { \Sigma f_i \over 2 } - f_{medPre} } \over f_{med} } * ClassInt $$

<ul>
    <li>Low<sub>med</sub>: Medyan sınıfının alt değeri. (Medyan sınıfı bulunurken toplam frekans (Σfi) 2’ye bölünür.)</li>
    <li>f<sub>medPre</sub>: Medyan sınıfından bir önceki sınıfa kadar olan frekanslar toplamı</li>
    <li>f<sub>med</sub>: Medyan sınıfının frekansı</li>
    <li>ClassInt (Class Interval): Sınıf aralığı</li>
</ul>

#### Örneklem Medyan Değeri

<div align="center">Gözlem Sayısının Tek Olduğu Basit Serilerde</div>

$$ \tilde x = {x_{n+1 \over 2}} $$

<div align="center">Gözlem Sayısının Çift Olduğu Basit Serilerde</div>

$$ \tilde x = { { x_{n\over 2} } + { x_{ { n\over 2}+1 } } \over 2} $$

<div align="center">Frekans Toplamının Tek Sayı Olduğu Frekans Serilerinde</div>

$$  \tilde x = { x_{ {(\Sigma f_i) + 1 } \over 2 } }$$

<div align="center">Frekans Toplamının Çift Sayı Olduğu Frekans Serilerinde</div>

$$ \tilde x = { { x_{ \Sigma f_i \over 2 } + x_{ { \Sigma f_i \over 2 } + 1 } } \over 2 } $$

<div align="center">Gruplandırılmış Serilerde</div>

$$ \tilde x = Low_{med} + { { { \Sigma f_i \over 2 } - f_{medPre} } \over f_{med} } * ClassInt $$
<ul>
    <li>Low<sub>med</sub>: Medyan sınıfının alt değeri. (Medyan sınıfı bulunurken toplam frekans (Σfi) 2’ye bölünür.)</li>
    <li>f<sub>medPre</sub>: Medyan sınıfından bir önceki sınıfa kadar olan frekanslar toplamı</li>
    <li>f<sub>med</sub>: Medyan sınıfının frekansı</li>
    <li>ClassInt (Class Interval): Sınıf aralığı</li>
</ul>

<strong>f</strong>: Frekans, <strong>N</strong> ve <strong>n</strong> Gözlem Sayısı

> Excel’de medyan değerini bulmak için =ORTANCA() formülünü kullanabiliriz.

<br>

<b>Uygulama</b>: x = 24, 12, 17, 13, 8, 8, 8, 8, 46 serisinin medyan değerini bulunuz.

<br>

Medyan değeri hesaplanırken öncelikle seri küçükten büyüğe sıralanır.

X = 8, 8, 8, 8, 12, 13, 17, 24, 46

N: 9’dur. (9 adet gözlem sayısı vardır.) Gözlem sayısı tek sayı olduğu için

$$ \tilde x = {x_{n+1 \over 2}} = {x_{9+1 \over 2}} = {x_5} = 12 $$

x<sub>5</sub>, serinin 5. değeri 12 medyan değeridir.

<br>

<b>Uygulama</b>: x = 48, 50, 50, 52, 54, 54, 54, 56 serisinin medyan değerini bulunuz.

<br>

n: 8’dir. Gözlem sayısı çift sayı olduğu için

$$ \tilde x = { { x_{n\over 2} } + { x_{ { n\over 2}+1 } } \over 2 } = { { x_{8\over 2} } + { x_{ { 8\over 2}+1 } } \over 2 } = { { x_4 + x_5 } \over 2 } = { { 52 + 54 } \over 2 } = 53 $$

4. ve 5. değerler toplamı 2’ye bölünür ve medyan değeri 53 bulunur.

<br>

<b>Uygulama</b>: Ağırlıkların listelendiği tablo aşağıda verilmiştir.

<table align="center">
  <tr>
    <th>Ağırlık (kg)</th>
    <th>Kişi Sayısı</th>
  </tr>
  <tr align="center">
    <td>60</td>
    <td>4</td>
  </tr>
  <tr align="center">
    <td>65</td>
    <td>8</td>
  </tr>
  <tr align="center">
    <td>70</td>
    <td>12</td>
  </tr>
  <tr align="center">
    <td>75</td>
    <td>14</td>
  </tr>
  <tr align="center">
    <td>80</td>
    <td>6</td>
  </tr>
  <tr align="center">
    <td>85</td>
    <td>3</td>
  </tr>
  <tr align="center">
    <td>90</td>
    <td>2</td>
  </tr>
  <tr align="center">
    <td>Toplam (Σ)</td>
    <td>49</td>
  </tr>
</table>

Ağırlıkların medyan değerini bulunuz.

<br>

<table align="center">
  <tr>
    <th>Ağırlık (X<sub>i</sub>)</th>
    <th>f<sub>i</sub></th>
    <th>Σf<sub>i</sub></th>
  </tr>
  <tr align="center">
    <td>60</td>
    <td>4</td>
    <td>4</td>
  </tr>
  <tr align="center">
    <td>65</td>
    <td>8</td>
    <td>12</td>
  </tr>
  <tr align="center">
    <td>70</td>
    <td>12</td>
    <td>24</td>
  </tr>
  <tr align="center">
    <td>75</td>
    <td>14</td>
    <td>38</td>
  </tr>
  <tr align="center">
    <td>80</td>
    <td>6</td>
    <td>44</td>
  </tr>
  <tr align="center">
    <td>85</td>
    <td>3</td>
    <td>47</td>
  </tr>
  <tr align="center">
    <td>90</td>
    <td>2</td>
    <td>49</td>
  </tr>
  <tr align="center">
    <td>Toplam (Σ)</td>
    <td>49</td>
    <td></td>
  </tr>
</table>

$$ \tilde X = { X_{ {(\Sigma f_i) + 1 } \over 2 } } = { X_{ { 49 + 1 } \over 2 } } = X_{25} = 75 $$

Medyan frekansının (X<sub>25</sub>) içinde bulunduğu birikimli frekans grubuna denk gelen gözlem değeri aynı zamanda frekans serisinin medyanıdır.

<br>

<strong>Uygulama</strong>: Boy uzunluklarının listelendiği tablo aşağıda verilmiştir.

<table align="center">
  <tr>
    <th>Boy (cm)</th>
    <th>Kişi Sayısı</th>
  </tr>
  <tr align="center">
    <td>165</td>
    <td>2</td>
  </tr>
  <tr align="center">
    <td>170</td>
    <td>4</td>
  </tr>
  <tr align="center">
    <td>175</td>
    <td>4</td>
  </tr>
  <tr align="center">
    <td>180</td>
    <td>7</td>
  </tr>
  <tr align="center">
    <td>185</td>
    <td>3</td>
  </tr>
  <tr align="center">
    <td>Toplam (Σ)</td>
    <td>20</td>
  </tr>
</table>

Boy uzunluklarının medyan değerini bulunuz.

<br>

<table align="center">
  <tr>
    <th>Boy (x<sub>i</sub>)</th>
    <th>f<sub>i</sub></th>
    <th>Σf<sub>i</sub></th>
  </tr>
  <tr align="center">
    <td>165</td>
    <td>2</td>
    <td>2</td>
  </tr>
  <tr align="center">
    <td>170</td>
    <td>4</td>
    <td>6</td>
  </tr>
  <tr align="center">
    <td>175</td>
    <td>4</td>
    <td>10</td>
  </tr>
  <tr align="center">
    <td>180</td>
    <td>7</td>
    <td>17</td>
  </tr>
  <tr align="center">
    <td>185</td>
    <td>3</td>
    <td>20</td>
  </tr>
  <tr align="center">
    <td>Toplam (Σ)</td>
    <td>20</td>
    <td></td>
  </tr>
</table>

Frekans toplamı çift sayı olduğu için

$$ \tilde x = { { x_{ \Sigma f_i \over 2 } + x_{ { \Sigma f_i \over 2 } + 1 } } \over 2 } = { { x_{ 20 \over 2 } + x_{ { 20 \over 2 } + 1 } } \over 2 } = { { x_{10} + x_{11} } \over 2 } = { { 175 + 180 } \over 2 } = 177.5 \approx 178 \text{ cm} $$

Birikimli frekans içerisinde 10. ve 11. sıraya karşılık gelen boy uzunlukları toplanır ve 2’ye bölünür. Elde edilen değer frekans serisinin medyan değeridir.

<br>

<strong>Uygulama</strong>: Sınav notları aşağıdaki tabloda gruplandırılmıştır.

<table align="center">
  <tr>
    <th>Sınav Notu</th>
    <th>Öğrenci Sayısı</th>
  </tr>
  <tr align="center">
    <td>00 - 20</td>
    <td>4</td>
  </tr>
  <tr align="center">
    <td>20 - 40</td>
    <td>16</td>
  </tr>
  <tr align="center">
    <td>40 - 60</td>
    <td>24</td>
  </tr>
  <tr align="center">
    <td>60 - 80</td>
    <td>43</td>
  </tr>
  <tr align="center">
    <td>80 - 100</td>
    <td>13</td>
  </tr>
  <tr align="center">
    <td>Toplam (Σ)</td>
    <td>100</td>
  </tr>
</table>

Notların medyan değerini bulunuz.

<br>

<table align="center">
  <tr>
    <th>Sınav Notu (X<sub>i</sub>)</th>
    <th>Öğrenci Sayısı (f<sub>i</sub>)</th>
    <th>Σf<sub>i</sub></th>
  </tr>
  <tr align="center">
    <td>00 - 20</td>
    <td>4</td>
    <td>4</td>
  </tr>
  <tr align="center">
    <td>20 - 40</td>
    <td>16</td>
    <td>20</td>
  </tr>
  <tr align="center">
    <td>40 - 60</td>
    <td>24</td>
    <td>44</td>
  </tr>
  <tr align="center">
    <td>60 - 80</td>
    <td>43</td>
    <td>87</td>
  </tr>
  <tr align="center">
    <td>80 - 100</td>
    <td>13</td>
    <td>100</td>
  </tr>
  <tr align="center">
    <td>Toplam (Σ)</td>
    <td>100</td>
    <td></td>
  </tr>
</table>

$$ \tilde X = Low_{med} + { { { \Sigma f_i \over 2 } - f_{medPre} } \over f_{med} } * ClassInt $$

<ul>
    <li>Low<sub>med</sub>: Birikimli frekanslar içerisinde (Σfi)/2 = 100/2 = 50. sıraya denk gelen 60 – 80 aralığının alt değeri 60’dır.</li>
    <li>f<sub>medPre</sub>: Medyan sınıfından bir önceki sınıfa kadar olan frekanslar toplamı (44)</li>
    <li>f<sub>med</sub>: Medyan sınıfının frekans değeri (43)</li>
    <li>ClassInt: Sınıf aralığı (80 – 60 = 20)</li>
</ul>

$$ \tilde X = { 60 + { { { 100 \over 2 } - { 44 } }\over 43 } * 20 } = 62.79 \approx 63 \text{ puan} $$

---

### Mod

Mod (Mode) seride en çok tekrar eden değerdir. Çift tepeli gruplandırılmış serilerde ve frekans serilerinde mod hesaplanamamaktadır. Gruplandırılmış serilerde gruplandırmanın daraltılması gerekmektedir.

#### Anakütle ve Örneklem Modu

<div align="center">Basit Serilerde</div>

$$ \text{Mod} = \text{En Cok Tekrar Eden Deger} $$

<div align="center">Frekans Serilerinde</div>

$$ \text{Mod} = \text{En Cok Tekrar Eden Frekans Sınıfı} $$

<div align="center">Gruplandırılmış Serilerde</div>

$$ \text{Mod} = \text{Low}_\text{mod} + { \Delta_{1} \over { \Delta_{1} + \Delta_{2} } } * \text{ClassInt} $$

<ul>
    <li>Low<sub>mod</sub>: Mod sınıfının alt değeri (En çok frekansa sahip grup, mod sınıfıdır.)</li>
    <li>Δ<sub>1</sub>: Mod Sınıfı Frekansı – Mod Sınıfından Bir Önceki Sınıfın Frekansı</li>
    <li>Δ<sub>2</sub>: Mod Sınıfı Frekansı – Mod Sınıfından Bir Sonraki Sınıfın Frekansı</li>
    <li>ClassInt (Class Interval): Sınıf aralığı</li>
</ul>

> Excel’de mod almak için =ENÇOK_OLAN.TEK() formülünü kullanabiliriz.

<br>

<strong>Uygulama</strong>: X<sub>1</sub> = 12, 14, 14, 16, 18, 18, 18, 18, 18, 20, 24 serisinin mod değerini bulunuz.

<br>

Seride en çok tekrar eden 18 olduğu için serinin modu 18’dir.

<br>

<strong>Uygulama</strong>: Boy uzunluklarının listelendiği tablo aşağıda verilmiştir.

<table align="center">
  <tr>
    <th>Boy (cm)</th>
    <th>Kişi Sayısı</th>
  </tr>
  <tr align="center">
    <td>165</td>
    <td>2</td>
  </tr>
  <tr align="center">
    <td>170</td>
    <td>4</td>
  </tr>
  <tr align="center">
    <td>175</td>
    <td>4</td>
  </tr>
  <tr align="center">
    <td>180</td>
    <td>7</td>
  </tr>
  <tr align="center">
    <td>185</td>
    <td>3</td>
  </tr>
  <tr align="center">
    <td>Toplam (Σ)</td>
    <td>20</td>
  </tr>
</table>

Boy uzunluklarının mod değerini bulunuz.

<br>

En çok tekrar eden frekansa sahip grup 180 cm boy uzunluğu sınıfı olduğu için mod değeri 180’dir.

<br>

<strong>Uygulama</strong>: Sınav notları aşağıdaki tabloda gruplandırılmıştır.

<table align="center">
  <tr>
    <th>Sınav Notu</th>
    <th>Öğrenci Sayısı</th>
  </tr>
  <tr align="center">
    <td>00 - 20</td>
    <td>4</td>
  </tr>
  <tr align="center">
    <td>20 - 40</td>
    <td>16</td>
  </tr>
  <tr align="center">
    <td>40 - 60</td>
    <td>24</td>
  </tr>
  <tr align="center">
    <td>60 - 80</td>
    <td>43</td>
  </tr>
  <tr align="center">
    <td>80 - 100</td>
    <td>13</td>
  </tr>
  <tr align="center">
    <td>Toplam (Σ)</td>
    <td>100</td>
  </tr>
</table>

Notların mod değerini bulunuz.

<br>

$$ \text{Mod} = \text{Low}_\text{mod} + { \Delta_{1} \over { \Delta_{1} + \Delta_{2} } } * \text{ClassInt} $$

<ul>
    <li>Low<sub>mod</sub>: Mod sınıfının alt değeri (En çok frekansa sahip grup, mod sınıfıdır.)</li>
    <li>Δ<sub>1</sub>: Mod Sınıfı Frekansı – Mod Sınıfından Bir Önceki Sınıfın Frekansı</li>
    <li>Δ<sub>2</sub>: Mod Sınıfı Frekansı – Mod Sınıfından Bir Sonraki Sınıfın Frekansı</li>
    <li>ClassInt (Class Interval): Sınıf aralığı</li>
</ul>

En çok frekansa sahip grup 60 – 80 nota sahip aralıktır. Bu sebeple bu sınıf aynı zamanda mod sınıfıdır.

$$ \text{Mod} = 60 + { {(43 - 24)} \over { (43 - 24) + (43 - 13) } } * (80 - 60) = 67.76 \approx 68 \text{ puan} $$

--- 

### Kartil

Kartil (Quartile) ya da Dörttebirlik seriyi dört eşit parçaya ayıran değerlerdir.

#### Anakütle Kartilleri

<div align="center">Basit Serilerde</div>

$$ Q_1 = X_{ {N+2} \over 4} $$ 

<div align="center">Gözlem Sayısının Tek Olduğu Basit Serilerde</div>

$$ Q_2 = \tilde X = X_{ {N+1} \over 2} $$

<div align="center">Gözlem Sayısının Çift Olduğu Basit Serilerde</div>

$$Q_2 = \tilde X ={ { X_{ {N} \over 2} } + { X_{ { {N} \over 2} + 1 } } \over 2 } $$

<div align="center">Frekans Toplamının Tek Sayı Olduğu Basit Serilerde</div>

$$ \tilde X = { X_{ {(\Sigma f_i) + 1 } \over 2 } } $$

$$ Q_3 = X_{ {3N+2} \over 4} $$

$$ Q_4 = \text{Serinin Son Elemanı} $$

<div align="center">Frekans Serilerinde</div>

$$ Q_1 = X_{ { {\Sigma f_i} + 2 } \over 4} $$

<div align="center">Frekans Toplamının Tek Sayı Olduğu Frekans Serilerinde</div>

$$ Q_2 = \tilde X = { X_{ { \Sigma f_i} + 1 } \over 2 } $$

<div align="center">Frekans Toplamının Çift Sayı Olduğu Frekans Serilerinde</div>

$$ Q_2 = \tilde X = { { X_{ \Sigma f_i \over 2 } + X_{ { \Sigma f_i \over 2 } + 1 } } \over 2 } $$

$$ Q_3 = X_{ { {3\Sigma f_i} + 1 } \over 4} $$

$$ Q_4 = \text{Serinin Son Elemanı} $$

<div align="center">Gruplandırılmış Serilerde</div>

$$ \tilde x = Low_{med} + { { { \Sigma f_i \over 2 } - f_{medPre} } \over f_{med} } * ClassInt $$
<ul>

$$ \text{Q}_1 $$

<ul>
    <li>Low<sub>Q</sub>:Kartil sınıfının alt değeri. (Q<sub>1</sub> Kartil Sınıfı=  Σf<sub>i</sub>/4, Q<sub>2</sub> Kartil Sınıfı=  2Σf<sub>i</sub>/4, Q<sub>3</sub> Kartil Sınıfı=  3Σf<sub>i</sub>/4)</li>
    <li>f<sub>QPre</sub>: Kartil sınıfından bir önceki sınıfa kadar olan frekanslar toplamı</li>
    <li>f<sub>Q</sub>: Kartil sınıfının frekansı</li>
    <li>ClassInt (Class Interval): Sınıf aralığı</li>
</ul>

Kartil indisi ondalıklı ise en yakın tamsayıya tamamlanır. Ondalık .5 ise iki sayının ortalaması alınır.











[^1]: Aykırı değer (outlier)

[^2]: Ortalama Gelir, Medyan Gelir ve Gini Katsayısı örneği için <a href="https://www.givingwhatwecan.org/blog/measuring-global-inequality-median-income-gdp-per-capita-and-the-gini-index#countries-by-gdp-per-capita-ppp-mean-income-ppp-median-income-ppp-gini-index-and--below-poverty-line3" target="_blank">tıklayınız</a>.

[^3]: IBM SPSS Statistics | version 26.0.0.0

[^4]: Değişken(ler)

[^5]: Seçenekler

[^6]: Ortalama

