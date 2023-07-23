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
    <th>Boy Uzunluğu</th>
    <th>Öğrenci Sayısı</th>
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
    <th>Öğrenci Sayısı</th>
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

$$ \text{Geo Ort} = \sqrt[N]{X_1X_2...X_N} \] $$

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

$$ \text{Log Geo Ort} = {\Sigma f_ilogx_i \over \Sigma f_i}  $$

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













[^1]: Aykırı değer (outlier)


