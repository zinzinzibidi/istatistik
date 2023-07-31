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











$$ $$

$$ $$

$$ $$

$$ $$

$$ $$








[^1]: İngilizce adı da momenttir.
