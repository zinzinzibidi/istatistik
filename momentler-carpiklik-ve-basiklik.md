# Momentler, Çarpıklık ve Basıklık

Momentler, çarpıklık (asimetri) ve basıklık bir serinin ortalamaya göre nasıl dağıldığını belirlemek için kullanılan temel istatistik ölçüleridir.

<table align="center">
  <tr align="center">
    <td><a href="#moment">Moment</a></td>
  </tr>
  <tr align="center">
    <td><a href="#konig">Könik Teoremi</a></td>
  </tr>
  <tr align="center">
    <td><a href="#carpiklik">Çarpıklık</a></td>
  </tr>
  <tr align="center">
    <td><a href="#basiklik">Basıklık</a></td>
  </tr>
  <tr align="center">
    <td><a href="#spss-carpiklik-basiklik">SPSS'te Çarpıklık ve Basıklık</a></td>
  </tr>
</table>

<br>

<span id="moment"></span>

## Moment

Terimlerin sıfırdan veya aritmetik ortalamadan sapmalarının çeşitli kuvvetlerine moment[^1] adı verilmektedir. Moment, bir serideki gözlem değerlerinin sıfırdan veya aritmetik ortalamadan farklarının kuvvetlerinin aritmetik ortalamasıdır.

Momentler 2 gruba ayrılır:

1. Sıfıra Göre Momentler
2. Aritmetik Ortalamaya Göre Momentler
   
### Sıfıra Göre Momentler

<div align="center">Anakütle Sıfıra Göre Momentleri</div>

Basit Serilerde

$$ M_1 = { \Sigma X_i \over N } $$

$$ M_2 = { \Sigma X_i^2 \over N } $$

$$ M_3 = { \Sigma X_i^3 \over N } $$

$$ M_4 = { \Sigma X_i^4 \over N } $$

$$ M_r = { \Sigma X_i^r \over N } $$

Frekans Serlerinde

$$ M_1 = { \Sigma f_i X_i \over \Sigma f_i } $$

$$ M_2 = { \Sigma f_i X_i^2 \over \Sigma f_i } $$

$$ M_3 = { \Sigma f_i X_i^3 \over \Sigma f_i } $$

$$ M_4 = { \Sigma f_i X_i^4 \over \Sigma f_i } $$

$$ M_r = { \Sigma f_i X_i^r \over \Sigma f_i } $$

Gruplandırılmış Serilerde

$$ M_1 = { \Sigma f_i m_i \over \Sigma f_i } $$

$$ M_2 = { \Sigma f_i m_i^2 \over \Sigma f_i } $$

$$ M_3 = { \Sigma f_i m_i^3 \over \Sigma f_i }  $$

$$ M_4 = { \Sigma f_i m_i^4 \over \Sigma f_i } $$

$$ M_r = { \Sigma f_i m_i^r \over \Sigma f_i } $$

<br>

<div align="center">Örneklem Sıfıra Göre Momentleri</div>

Basit Serilerde

$$ M_1 = { \Sigma x_i \over n } $$

$$ M_2 = { \Sigma x_i^2 \over n } $$

$$ M_3 = { \Sigma x_i^3 \over n } $$

$$ M_4 = { \Sigma x_i^4 \over n } $$

$$ M_r = { \Sigma x_i^r \over n } $$

Frekans Serlerinde

$$ M_1 = { \Sigma f_i x_i \over \Sigma f_i } $$

$$ M_2 = { \Sigma f_i x_i^2 \over \Sigma f_i } $$

$$ M_3 = { \Sigma f_i x_i^3 \over \Sigma f_i } $$

$$ M_4 = { \Sigma f_i x_i^4 \over \Sigma f_i } $$

$$ M_r = { \Sigma f_i x_i^r \over \Sigma f_i } $$

Gruplandırılmış Serilerde

$$ M_1 = { \Sigma f_i m_i \over \Sigma f_i }  $$

$$ M_2 = { \Sigma f_i m_i^2 \over \Sigma f_i } $$

$$ M_3 = { \Sigma f_i m_i^3 \over \Sigma f_i } $$

$$ M_4 = { \Sigma f_i m_i^4 \over \Sigma f_i } $$

$$ M_r = { \Sigma f_i m_i^r \over \Sigma f_i } $$

<br>

m: Sınıf Orta Sayısı, f: Frekans

M<sub>1</sub>: 1. Dereceden Moment, M<sub>4</sub>: 4. Dereceden Moment, M<sub>r</sub>: r. Dereceden Moment

<br>

### Aritmetik Ortalamaya Göre Momentler

<div align="center">Anakütle Aritmetik Ortalamaya Göre Momentleri</div>

Basit Serilerde

$$ M_1 = { \Sigma (X_i - \mu) \over N } $$

$$ M_2 = { \Sigma (X_i - \mu)^2 \over N } $$

$$ M_3 = { \Sigma (X_i - \mu)^3 \over N } $$

$$ M_4 = { \Sigma (X_i - \mu)^4 \over N } $$

$$ M_r = { \Sigma (X_i - \mu)^r \over N } $$

Frekans Serilerinde

$$ M_1 = { \Sigma f_i (X_i - \mu) \over \Sigma f_i } $$

$$ M_2 = { \Sigma f_i (X_i - \mu)^2 \over \Sigma f_i } $$

$$ M_3 = { \Sigma f_i (X_i - \mu)^3 \over \Sigma f_i } $$

$$ M_4 = { \Sigma f_i (X_i - \mu)^4 \over \Sigma f_i } $$

$$ M_r = { \Sigma f_i (X_i - \mu)^r \over \Sigma f_i } $$

Gruplandırılmış Serilerde

$$ M_1 = { \Sigma f_i (m_i - \mu) \over \Sigma f_i } $$

$$ M_2 = { \Sigma f_i (m_i - \mu)^2 \over \Sigma f_i } $$

$$ M_3 = { \Sigma f_i (m_i - \mu)^3 \over \Sigma f_i } $$

$$ M_4 = { \Sigma f_i (m_i - \mu)^4 \over \Sigma f_i } $$

$$ M_r = { \Sigma f_i (m_i - \mu)^r \over \Sigma f_i } $$

<br>

<div align="center">Örneklem Aritmetik Ortalamaya Göre Momentleri</div>

Basit Serilerde

$$ M_1 = { \Sigma (x_i - \bar x) \over n } $$

$$ M_2 = { \Sigma (x_i - \bar x)^2 \over n } $$

$$ M_3 = { \Sigma (x_i - \bar x)^3 \over n } $$

$$ M_4 = { \Sigma (x_i - \bar x)^4 \over n } $$

$$ M_r = { \Sigma (x_i - \bar x)^r \over n } $$

Frekans Serilerinde

$$ M_1 = { \Sigma f_i (x_i - \bar x) \over \Sigma f_i } $$

$$ M_2 = { \Sigma f_i (x_i - \bar x)^2 \over \Sigma f_i } $$

$$ M_3 = { \Sigma f_i (x_i - \bar x)^3 \over \Sigma f_i } $$

$$ M_4 = { \Sigma f_i (x_i - \bar x)^4 \over \Sigma f_i } $$

$$ M_r = { \Sigma f_i (x_i - \bar x)^r \over \Sigma f_i } $$

Gruplandırılmış Serilerde

$$ M_1 = { \Sigma f_i (m_i - \bar x) \over \Sigma f_i } $$

$$ M_2 = { \Sigma f_i (m_i - \bar x)^2 \over \Sigma f_i } $$

$$ M_3 = { \Sigma f_i (m_i - \bar x)^3 \over \Sigma f_i } $$

$$ M_4 = { \Sigma f_i (m_i - \bar x)^4 \over \Sigma f_i } $$

$$ M_r = { \Sigma f_i (m_i - \bar x)^r \over \Sigma f_i } $$

<br>

m: Sınıf Orta Sayısı, f: Frekans

M<sub>1</sub>: 1. Dereceden Moment, M<sub>4</sub>: 4. Dereceden Moment, M<sub>r</sub>: r. Dereceden Moment

<br>

<span id="konig"></span>

---

## König Teoremi

Sıfıra göre momentler biliniyorsa, aritmetik ortalamaya göre momentler kolaylıkla hesaplanabilir. König Teoremi adı verilen momentler arasındaki ilişki şu şekildedir:

$$ \mu_2 = M_2 - M_1^2 $$

$$ \mu_3 = M_3 - 3M_1M_2 + 2M_1^3 $$

$$ \mu_4 = M_4 - 4M_1M_3 + 6M_1^2M_2 - 3M_1^3 $$

<br>

<strong>Uygulama</strong>: Aşağıda 7 değerden oluşan x serisi verilmiştir.

$$ x = 10, 12, 14, 14, 16, 18, 20 $$

Serinin 1’den 4. Dereceye kadar olan momentlerini sıfıra, aritmetik ortalamaya ve König Teoremine göre bulunuz.

<br>

Sıfıra göre momentler:

<table align="center">
  <tr>
    <th></th>
    <th>(x<sub>i</sub>)</th>
    <th>(x<sub>i</sub>)<sup>2</sup></th>
    <th>(x<sub>i</sub>)<sup>3</sup></th>
    <th>(x<sub>i</sub>)<sup>4</sup></th>
  </tr>
  <tr align="center">
    <td></td>
    <td>10</td>
    <td>100</td>
    <td>1000</td>
    <td>10000</td>
  </tr>
  <tr align="center">
    <td></td>
    <td>12</td>
    <td>144</td>
    <td>1728</td>
    <td>20736</td>
  </tr>
  <tr align="center">
    <td></td>
    <td>14</td>
    <td>196</td>
    <td>2744</td>
    <td>38416</td>
  </tr>
  <tr align="center">
    <td></td>
    <td>14</td>
    <td>196</td>
    <td>2744</td>
    <td>38416</td>
  </tr>
  <tr align="center">
    <td></td>
    <td>16</td>
    <td>256</td>
    <td>4096</td>
    <td>65536</td>
  </tr>
  <tr align="center">
    <td></td>
    <td>18</td>
    <td>324</td>
    <td>5832</td>
    <td>104976</td>
  </tr>
  <tr align="center">
    <td></td>
    <td>20</td>
    <td>400</td>
    <td>8000</td>
    <td>160000</td>
  </tr>
  <tr align="center">
    <td>Toplam (Σ)</td>
    <td>104</td>
    <td>1616</td>
    <td>26144</td>
    <td>438080</td>
  </tr>
</table>

$$ M_1 = { \Sigma x_i \over n } = { 104 \over 7 } = 14.86 $$

$$ M_2 = { \Sigma x_i^2 \over n } = { 1616 \over 7 } = 230.86 $$

$$ M_3 = { \Sigma x_i^3 \over n } = { 26144 \over 7 } = 3734.86 $$

$$ M_4 = { \Sigma x_i^4 \over n } = { 438080 \over 7 } = 62582.86 $$

<br>

Aritmetik ortalamaya göre momentler:

x̄ = 15

<table align="center">
  <tr>
    <th></th>
    <th>(x<sub>i</sub> - x̄)</th>
    <th>(x<sub>i</sub> - x̄)<sup>2</sup></th>
    <th>(x<sub>i</sub> - x̄)<sup>3</sup></th>
    <th>(x<sub>i</sub> - x̄)<sup>4</sup></th>
  </tr>
  <tr align="center">
    <td></td>
    <td>(10 – 15)</td>
    <td>(10 – 15)<sup>2</sup></td>
    <td>(10 – 15)<sup>3</sup></td>
    <td>(10 – 15)<sup>4</sup></td>
  </tr>
  <tr align="center">
    <td></td>
    <td>(12 – 15)</td>
    <td>(12 – 15)<sup>2</sup></td>
    <td>(12 – 15)<sup>3</sup></td>
    <td>(12 – 15)<sup>4</sup></td>
  </tr>
  <tr align="center">
    <td></td>
    <td>(14 – 15)</td>
    <td>(14 – 15)<sup>2</sup></td>
    <td>(14 – 15)<sup>3</sup></td>
    <td>(14 – 15)<sup>4</sup></td>
  </tr>
  <tr align="center">
    <td></td>
    <td>(14 – 15)</td>
    <td>(14 – 15)<sup>2</sup></td>
    <td>(14 – 15)<sup>3</sup></td>
    <td>(14 – 15)<sup>4</sup></td>
  </tr>
  <tr align="center">
    <td></td>
    <td>(16 – 15)</td>
    <td>(16 – 15)<sup>2</sup></td>
    <td>(16 – 15)<sup>3</sup></td>
    <td>(16 – 15)<sup>4</sup></td>
  </tr>
  <tr align="center">
    <td></td>
    <td>(18 – 15)</td>
    <td>(18 – 15)<sup>2</sup></td>
    <td>(18 – 15)<sup>3</sup></td>
    <td>(18 – 15)<sup>4</sup></td>
  </tr>
  <tr align="center">
    <td></td>
    <td>(20 – 15)</td>
    <td>(20 – 15)<sup>2</sup></td>
    <td>(20 – 15)<sup>3</sup></td>
    <td>(20 – 15)<sup>4</sup></td>
  </tr>
  <tr align="center">
    <td>Toplam (Σ)</td>
    <td>-1</td>
    <td>71</td>
    <td>-1</td>
    <td>1415</td>
  </tr>
</table>

$$ M_1 = { \Sigma (x_i - \bar x) \over n } = { -1 \over 7 } = -0.14 $$

$$ M_2 = { \Sigma (x_i - \bar x)^2 \over n } = { 71 \over 7 } = 10.14 $$

$$ M_3 = { \Sigma (x_i - \bar x)^3 \over n } = { -1 \over 7 } = -0.14 $$

$$ M_4 = { \Sigma (x_i - \bar x)^4 \over n } = { 1415 \over 7 } = 202.14 $$

<br>

König Teoremine göre momentler:

$$ \mu_2 = M_2 - M_1^2 = 230.86 - 14.86^2 = 10.04 $$

$$ \mu_3 = M_3 - 3M_1M_2 + 2M_1^3 = 3734.86 - 3(14.86)(230.86) + 2(14.86)^3 = 5.88 $$

$$ \mu_4 = M_4 - 4M_1M_3 + 6M_1^2M_2 - 3M_1^3 $$

$$ \mu_4 = 62582.86-4(14.86)(3734.86)+6(14.86)^2 (230.86)-3(14.86)^4 $$

$$ \mu_4 = 169.37 $$

<br>

<span id="carpiklik"></span>

---

## Çarpıklık

Asimetri ya da Çarpıklık (Skewness) seri değerlerinin başta mı yoksa sonda mı yoğunlaştığını tespit etmemize yarayan istatistik ölçüsüdür.

Serileri incelediğimizde her seri aynı özelliğe sahip olmayabilir. Örneğin ortalaması ve standart sapması eşit olan iki seriden birindeki değerler başlangıç değerleri etrafında yoğunlaşırken ikinci serideki değerler son değerler etrafında yoğunlaşabilir. Bu şekilde serilerin simetrik dağılıp dağılmadığına bakarız. Seriler simetrik dağılmadığında adına asimetrik dağılım (skewed distribution, asymmetrical distribution) deriz.[^2]

<p align="center">
  <img src="https://zinzinzibidi.com/img/istatistik/simetrik-dagilim.png" style="width: 600px;"/>
</p>

Simetrik dağılımlarda Mod = Medyan = Ortalama birbirine eşittir. Normal dağılım, simetrik dağılıma en iyi örnektir.

<p align="center">
  <img src="https://zinzinzibidi.com/img/istatistik/pozitif-asimetrik-dagilim.png" style="width: 600px;"/>
</p>

Pozitif asimetrik dağılımlarda Mod > Medyan > Ortalama ilişkisi vardır. Bu dağılımlar aynı zamanda “sağa çarpık” olarak adlandırılır.

<p align="center">
  <img src="https://zinzinzibidi.com/img/istatistik/negatif-asimetrik-dagilim.png" style="width: 600px;"/>
</p>

Negatif asimetrik dağılımlarda Ortalama > Medyan > Mod ilişkisi vardır. Bu dağılımlar aynı zamanda “sola çarpık” olarak adlandırılır.

Tam simetrik ya da tam simetriğe yakın serilerde şu ilişki vardır:

$$ \bar x - Mod = 3(\bar x - \tilde x) $$

x̄: Aritmetik Ortalama, x̃: Medyan

<br>

### Çarpıklık (Asimetri) Ölçüleri

Çarpıklık ölçüleri

* Ortalamaya Dayanan Asimetri Ölçüsü (Pearson Asimetri Ölçüsü)
* Kartillere Dayanan Asimetri Ölçüsü (Bowley Asimetri Ölçüsü)[^3]
* Momentlere Dayanan Asimetri Ölçüsü

olmak üzere 3’e ayrılır.

#### Pearson Asimetri Ölçüsü

$$ AS_P = { { 3(\bar x - \tilde x) } \over s } $$

x̄: Aritmetik Ortalama, x̃: Medyan, s: Standart Sapma

Ortalamaya dayanan asimetri ölçüsüdür. -3 ve +3 arasında değer alır. 0’ın altında olduğu durumlarda sola çarpık negatif asimetrik dağılımdan, 0’ın üzerinde olduğu durumlarda ise sağa çarpık pozitif asimetrik dağılımlardan söz edilir. Tam simetri durumunda 0 değerini verir.

#### Bowley Asimetri Ölçüsü

$$ AS_B = { { (Q_3 - Q_2) - (Q_2 - Q_1) } \over { (Q_3 - Q_2) + (Q_2 - Q_1) } } $$

Kartillere dayanan asimetri ölçüsüdür. -1 ve +1 arasında değer alır. 0’ın altında olduğu durumlarda sola çarpık negatif asimetrik dağılımdan, 0’ın üzerinde olduğu durumlarda ise sağa çarpık pozitif asimetrik dağılımlardan söz edilir. Tam simetri durumunda 0 değerini verir.

#### Momentlere Dayanan Asimetri Ölçüsü

$$ \alpha_3 = { M_3 \over \sigma^3 } = { M_3 \over \sqrt{M_2^3} } $$

Momentler yardımıyla hesaplanan bu çarpıklık ölçüsünde sonuç 0’dan küçükse sola çarpık negatif asimetrik dağılımdan, 0’dan büyükse sağa çarpık pozitif asimetrik dağılımdan söz edilir. Tam simetri durumunda 0 değerini verir.

Aritmetik ortalamaya göre 3. dereceden moment asimetri ölçüsü olarak bilinir. Bu sebeple α<sub>3</sub> ile gösterilir.

<br>

<strong>Uygulama</strong>: Aşağıda 12 değerden oluşan x serisi verilmiştir.

$$ x = 10, 10, 11, 12, 12, 12, 12, 12, 12, 14, 16, 20 $$

Serinin çarpıklığını Pearson, Bowley ve Momentlere Dayanan Asimetri ölçülerine göre yorumlayınız.

<br>

Pearson Asimetri Ölçüsüne göre öncelikle ortalama ve medyan değerleri bulunmalıdır.

$$ \bar x = { \Sigma x_i \over n } = { 153 \over 12 } = 12.75 $$

$$ \tilde x = { { x_{n \over 2} + x_{ {n \over 2} + 1 } } \over 2 } = { { x_6 + x_7 } \over 2 } = { { 12 + 12 } \over 2 } = 12.00 $$

$$ s = \sqrt{ { \Sigma (x_i - \bar x)^2 } \over n - 1 } = \sqrt{ 86.25 \over 11 } = \sqrt{ 7.1875 } = 2.80 $$

$$ AS_P = { { 3(\bar x - \tilde x) } \over s } = { { 3(12.75 - 12.00) } \over 2.80 } = 0.80 $$

1.00’a yakın pozitif bir asimetri ölçüsü söz konusudur. Bu sebeple hafif sağa çarpık pozitif asimetrik dağılımdan söz edilebilir.

<br>

Bowley Asimetri Ölçüsüne göre Q<sub>4</sub> dışında tüm kartil değerleri bulunmalıdır.

$$ Q_1 = x_{ {n+2} \over 4} = x_{ 12+2 \over 4} = x_{3.50} = { {x_3 + x_4} \over 2 } = { { 11 + 12 } \over 2 } = 11.50 $$

$$ Q_2 = \tilde x ={ { x_{ {n} \over 2} } + { x_{ { {n} \over 2} + 1 } } \over 2 } =  12.00 $$

$$ Q_3 = x_{ {3n+2} \over 4} = x_{ 38 \over 4 } = x_{9.50} = { {x_9 + x_{10}} \over 2 } = { { 12 + 14 } \over 2 } = 13.00 $$

$$  AS_B = { { (Q_3 - Q_2) - (Q_2 - Q_1) } \over { (Q_3 - Q_2) + (Q_2 - Q_1) } } = { { (13 - 12) - (12 - 11.50) } \over { (13 - 12) + (12 - 11.50) } } = 0.33 $$

Pearson Asimetri ölçüsünde olduğu gibi 1.00’a yakın pozitif asimetri söz konusudur. Bu sebeple hafif sağa çarpık pozitif asimetrik dağılımdan söz edilebilir.

<br>

Momentlere Dayanan Asimetri Ölçüsüne göre serinin 3. dereceden momentini bulmamız yeterlidir. Standart sapmayı Pearson Asimetri Ölçüsünde hesaplamıştık.

$$ M_3 = { \Sigma (x_i - \bar x)^3 \over n } = { 367.88 \over 12 } = 30.66 $$

$$ \alpha_3 = { M_3 \over \sigma^3 } = { 30.66 \over 2.80^3 } = { 30.66 \over 21.96 } = 1.40 $$

Bulunan asimetri ölçüsü 0’ın üzerinde olduğu için sağa çarpık pozitif asimetrik dağılımdan söz edilir. 3 asimetri ölçüsünde de seri değerlerinin pozitif asimetrik dağıldığı ve dağılım sağa çarpık olduğu sonucuna varılmıştır.

<br>

<span id="basiklik"></span>

---

## Basıklık











$$ $$

$$ $$

$$ $$

$$ $$

$$ $$








[^1]: İngilizce adı da momenttir.

[^2]: Dağılım, simetrikse ve aykırı değerler yoksa aritmetik ortalama, asimetrikse ve aykırı değerler varsa medyan kullanımı tercih edilir.

[^3]: Galton Asimetri Ölçüsü olarak da bilinir.
