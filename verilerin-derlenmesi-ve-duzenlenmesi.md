# Verilerin Derlenmesi ve Düzenlenmesi

Araştırmaya başlanılmadan önce edinilen ham verilerin kirli verilerden temizlenmesi konusuna değinmiştik. Ham veriler kirli veriler içermese bile veri setini okunaklı hâle getirmek için bazı düzenlemelere ihtiyaç duyarız.

Veri modellemesinde “Verilerin Toplanması” (Collecting Data) aşamasının ardından “Verilerin Derlenmesi ve Düzenlenmesi” (Compiling & Organizing Data) aşamalarına geçilir. Veriler türlerine göre derlendikten sonra veri setini “sınıflama ve gruplama metodları” ile özet tablolara dönüştürürüz.

## Verilerin Toplanması

Elimizde 122 öğrencinin istatistik sınav notlarını temsil edecek 44 öğrenciye ait 4 farklı sınıfın verisi olsun.

$$ x_1 = 48, 45, 48, 64, 50, 24, 04, 12, 88, 71, 64 $$

$$ x_2 = 24, 12, 25, 33, 44, 45, 64, 48, 55, 64, 88 $$

$$ x_3 = 12, 24, 25, 48, 64, 88, 88, 71, 48, 55, 50 $$

$$ x_4 = 74, 48, 64, 88, 24, 12, 04, 71, 55, 48, 50 $$

## Verilerin Derlenmesi ve Özetlenmesi

Tek bir veri setinde tüm verileri küçükten büyüğe sıralarsak aşağıdaki seriyi elde ederiz.

$$ x = 04, 04, 12, 12, 12, 12, 24, 24, 24, 24, 25, 25, 33, 44, 45, 45, 48, 48, 48, 48, 48, 48, 48, 50, 50, 50, 55, 55, 55, 64, 64, 64, 64, 64, 64, 71, 71, 71, 74, 88, 88, 88, 88, 88 $$

Serinin az sayıda birimden oluşmasından ve tek bir değişken içermesinden dolayı derleme aşaması tamamlanmıştır.

Dikkatli bakıldığında veri setinin tekrar eden sayılardan oluştuğu görülebilir. Hangi sayıların hangi sıklıkla tekrar edildiğini görebilmek için birimleri sınıflandırabiliriz.

<br>

<table align="center">
  <tr>
    <th>x</th>
    <th>f (tekrar sayısı)</th>
  </tr>
  <tr align="center">
    <td>04</td>
    <td>2</td>
  </tr>
  <tr align="center">
    <td>12</td>
    <td>4</td>
  </tr>
  <tr align="center">
    <td>24</td>
    <td align="center">4</td>
  </tr>
  <tr align="center">
    <td>25</td>
    <td align="center">2</td>
  </tr>
  <tr align="center">
    <td>33</td>
    <td align="center">1</td>
  </tr>
  <tr align="center">
    <td>44</td>
    <td align="center">1</td>
  </tr>
  <tr align="center">
    <td>45</td>
    <td align="center">2</td>
  </tr>
  <tr align="center">
    <td>48</td>
    <td align="center">7</td>
  </tr>
  <tr align="center">
    <td>50</td>
    <td align="center">3</td>
  </tr>
  <tr align="center">
    <td>55</td>
    <td align="center">3</td>
  </tr>
  <tr align="center">
    <td>64</td>
    <td align="center">6</td>
  </tr>
  <tr align="center">
    <td>71</td>
    <td align="center">3</td>
  </tr>
  <tr align="center">
    <td>74</td>
    <td align="center">1</td>
  </tr>
  <tr align="center">
    <td>88</td>
    <td align="center">5</td>
  </tr>
  <tr align="center">
    <td>Toplam (Σ)</td>
    <td align="center">44</td>
  </tr>
</table>

<br>

Bu noktada sınavda 48, 64 ve 88 not alan öğrencilerin çoğunlukta olduğu sonucuna varabiliriz. Yaptığımız işleme “sınıflama” (statistical classification) denilmektedir. f notasyonu[^1], birimlerin veri setinde hangi sıklıkla tekrar edildiğini belirtmektedir.

Tabloyu biraz daha özet hâle getirelim.

<table align="center">
  <tr>
    <th>Sınıf Aralığı</th>
    <th>Frekans (f)</th>
  </tr>
  <tr align="center">
    <td>00 - 25</td>
    <td>12</td>
  </tr>
  <tr align="center">
    <td>26 - 50</td>
    <td>14</td>
  </tr>
  <tr align="center">
    <td>51 - 75</td>
    <td>13</td>
  </tr>
  <tr align="center">
    <td>76 - 100</td>
    <td>5</td>
  </tr>
  <tr align="center">
    <td>Toplam (Σ)</td>
    <td>44</td>
  </tr>
</table>

<br>

Bu işleme ise gruplandırma ya da gruplama (statistical grouping) denilmektedir. Gruplandırma, sınıf dağılımlarının özet tablolara dönüştürülmesi işlemidir. Örnekte istatistik dersinden alınan notların 0 ve 75 arasında yoğunlaştığı görülebilir.

## Verilerin Grafikleştirilmesi

<p align="center">
  <img src="https://zinzinzibidi.com/img/istatistik/verilerin-grafiklestirilmesi.png" style="width: 480px;"/>
</p>

Yoğunlaşmayı net görebilmek için histogram grafikleri kullanırız. (Yukarıdaki grafik histogram grafiğidir.)

Bu tür basit örneklerde sınıf aralığı ve birim sayısının az olmasından dolayı grafik kullanmamıza bile gerek bulunmamaktadır. Buna rağmen çok fazla verinin ve sınıf aralığının olduğu veri setlerinde grafik kullanılması yoğunlaşmanın nerede olduğunu anlamamızda tablolara göre daha fazla esneklik sağlayacaktır.

## Gruplandırmada Sınıf Aralığı Uzunluğunun Belirlenmesi

İstatistik sınav notları örneğinde sınıf aralığını 25 notluk dilimlere ayırarak 4 farklı dilimde belirledik. Sınıfları aralıklandırmayı, diğer bir ifade ile gruplandırmayı tamamen kendi yöntemlerimizle gerçekleştirdik.

İstatistik standartlarına uygun gruplandırma yapmak istersek sınıf aralığını aşağıdaki formül ile belirleriz.

$$ Sınıf Aralığı = [x_{max} - x_{min}]/[1+3.3log(n)] $$

$$  Sınıf Aralığı = \text{Sınıf Uzunluğu (Range)}/\text{Sınıf Sayısı} $$








[^1]: frekans (frequency)
