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

<br>

$$ x = 04, 04, 12, 12, 12, 12, 24, 24, 24, 24, 25, 25, 33, 44, 45, 45, 48, 48, 48, 48, 48, 48, 48, 50, 50, 50, 55, 55, 55, 64, 64, 64, 64, 64, 64, 71, 71, 71, 74, 88, 88, 88, 88, 88 $$

* x<sub>max</sub>: En yüksek değer
* x<sub>min</sub>: En düşük değer
* n: Birim sayısı

Formülü x serisine uyguladığımızda

$$ Sınıf Aralığı = [x_{max} - x_{min}]/[1+3.3log(n)] $$

$$ Sınıf Aralığı = [88 - 04]/[1+3.3log(44)] $$

$$ Sınıf Aralığı \approx 13.08 \approx 13 $$

<table align="center">
  <tr>
    <th>Sınıf Aralığı</th>
    <th>Frekans (f)</th>
  </tr>
  <tr align="center">
    <td>04 ≤ x < 17</td>
    <td>6</td>
  </tr>
  <tr align="center">
    <td>17 ≤ x < 30</td>
    <td>6</td>
  </tr>
  <tr align="center">
    <td>30 ≤ x < 43</td>
    <td>1</td>
  </tr>
  <tr align="center">
    <td>43 ≤ x < 56</td>
    <td>16</td>
  </tr>
    <tr align="center">
    <td>56 ≤ x < 69</td>
    <td>6</td>
  </tr>
  <tr align="center">
    <td>69 ≤ x < 82</td>
    <td>4</td>
  </tr>
  <tr align="center">
    <td>82 ≤ x < 95</td>
    <td>5</td>
  </tr>
  <tr align="center">
    <td>Toplam (Σ)</td>
    <td>44</td>
  </tr>
</table>

<br>

Dikkat edilirse ilk aralığımız olan 04 ≤ x < 17 aralığının uzunluğu
17 – 04 = 13’tür. “Sınıf aralığı” ifadesi buradan gelmektedir.

<p align="center">
  <img src="https://zinzinzibidi.com/img/istatistik/sinav-notlari-dagilimi.png" style="width: 480px;"/>
</p>

Bir önceki histogram grafiğinden farklı olarak sınav notlarının 43 ve 56 aralığında yoğunlaştığını rahatlıkla söyleyebilir, “44 öğrencinin 16’sı
43 ≤ x < 56 aralığında not almıştır” sonucuna varabiliriz.

## Göreceli ve Birikimli Frekans

<b>Göreceli Frekans (Relatif Frekans, Relative Frequency)</b>: Frekans dağılımının yüzdesel gösterimidir.

<b>Birikimli Frekans (Kümülatif Frekans, Cumulative Frequency)</b>: Frekans dağılımının birikimli gösterimidir.

<table align="center">
  <tr>
    <th>Sınıf Aralığı</th>
    <th>Frekans (f)</th>
    <th>Gör. Frekans (%)</th>
    <th>Bir. Frekans (Σf)</th>
    <th>Gör. Bir. Fre. (%Σf)</th>
  </tr>
  <tr align="center">
    <td>04 ≤ x < 17</td>
    <td>6</td>
    <td>%13.64</td>
    <td>6</td>
    <td>%13.64</td>
  </tr>
  <tr align="center">
    <td>17 ≤ x < 30</td>
    <td>6</td>
    <td>%13.64</td>
    <td>12</td>
    <td>%27.27</td>
  </tr>
  <tr align="center">
    <td>30 ≤ x < 43</td>
    <td>1</td>
    <td>%2.27</td>
    <td>13</td>
    <td>%29.55</td>
  </tr>
  <tr align="center">
    <td>43 ≤ x < 56</td>
    <td>16</td>
    <td>%36.36</td>
    <td>29</td>
    <td>%65.91</td>
  </tr>
  <tr align="center">
    <td>56 ≤ x < 69</td>
    <td>6</td>
    <td>%13.64</td>
    <td>35</td>
    <td>%79.55</td>
  </tr>
  <tr align="center">
    <td>69 ≤ x < 82</td>
    <td>4</td>
    <td>%9.09</td>
    <td>39</td>
    <td>%88.64</td>
  </tr>
  <tr align="center">
    <td>82 ≤ x < 95</td>
    <td>5</td>
    <td>%11.36</td>
    <td>44</td>
    <td>%100</td>
  </tr>
  <tr align="center">
    <td>Toplam (Σ)</td>
    <td>44</td>
    <td>%100</td>
    <td>-</td>
    <td>-</td>
  </tr>
</table>

<br>

04 ≤ x < 17 aralığının göreceli frekansı hesaplanırken frekans sayısı frekans toplamına bölünür ve % (yüzde) ifadesi ile gösterilir.
(6/44 = 0.1364 = %13.64)

Birikimli frekansta bir önceki sınıf aralığının frekans sayısı toplanır ve sonraki sınıf aralığına geçilir.

0 + 6 = 6

6 + 6 = 12

12 + 1 = 13

...

Göreceli birikimli frekans, birikimli frekansın oransal gösterimidir.
43 ≤ x < 56 aralığının göreceli birikimli hesaplanırken birikimli frekans değeri frekans toplamına bölünür. Göreceli frekansta olduğu gibi % ifadesi ile gösterilir. (29/44 = %65.91)

Yorumlanmaları şu şekildedir:

* 44 öğrencinin %9’u 69 ≤ x < 82 aralığında not almıştır. (göreceli frekans)
* 04 ≤ x < 82 aralığında not alanların sayısı 39’dur. (birikimli frekans)
* 04 ≤ x < 82 aralığında not alanların örneklem içindeki payı %89’dur. (göreceli birikimli frekans)

Hatırlarsanız 122 öğrenciden 44 öğrenciyi örnekleme amacıyla seçmiştik. Bu sebeple “örneklem içindeki payı %89’dur” yorumlaması yerine “tüm öğrenciler içindeki payı %89’dur” sonucuna varmak istatistiksel olarak anlamlı olmazdı.

> Herhangi bir istatistiksel kaynakta “göreceli” ya da “relatif” ifadeleri geçiyorsa “oransal” (nispî, proportional) değerlerden söz ediliyordur. Göreceli değerler çoğunlukla oransal (yüzdesel) artışları veya azalışları göstermek için kullanılır.

## Yüzde (%) Gösterimleri ve Yuvarlamalar

% (yüzde) ifadeleri kendi notasyonu ile gösterilse de 0.1424 şeklinde ondalıklı da gösterilebilir. Kimi zaman ondalıklı değerler 100 ile çarpılır ve 14.24 gösterimleri tercih edilir. “Çarpı 100” gösterimlerinin tercih edilmesi durumunda sütun başlıklarında ifadenin oransal değer olduğu mutlaka belirtilmelidir. Sütun başlığının “Pay” yerine “Pay (%)” olması gibi …

İstatistikte 0 değeri sayıların başlangıcında kullanılmayabilir. Örneğin; “0.1424” oranını “.1424” şeklinde gösterebiliriz. “Nokta Sayı” gösterimleri noktadan önce 0 (sıfır) kullanıldığını belirtir.

Hesap makinenizde <b>.1424 x 2</b> işlemini yaptığınızda sonucun <b>0.2848</b> olduğunu görebilirsiniz.

Yuvarlamalar (rounding) ondalık basamakların azaltılmasında kullanılan ve sayı okunurluğunu artıran özelliklerden biridir. Yuvarlamalarda son ondalığın 5 veya 5’ten yukarı olup olmadığına bakılır. 5 veya 5’ten yukarı ise bir üst sayıya tamamlanır. Değilse soldaki ondalıkta değişiklik yapılmaz.

0.14245732<b>9</b> = 0.1424573<b>3</b> = 0.142457<b>3</b> = 0.14245<b>7</b> = 0.1424<b>6</b> = 0.142<b>5</b> = 0.14<b>3</b> = 0.1<b>4</b> = 0.<b>1</b>

---

## Sıra Sizde

<b>Uygulama</b>: x = 10, 10, 10, 11, 11, 16, 18, 20, 22, 22, 24 serisinin sınıf uzunluğu ve sınıf aralığı kaçtır?

A) Sınıf Uzunluğu: 10 | Sınıf Aralığı: 5 <br>
B) Sınıf Uzunluğu: 14 | Sınıf Aralığı: 3 <br>
C) Sınıf Uzunluğu: 10 | Sınıf Aralığı: 5 <br>
D) Sınıf Uzunluğu: 14 | Sınıf Aralığı: 3 

<b>Yanıt</b>: 

$$ Sınıf Aralığı = [x_{max} - x_{min}]/[1+3.3log(n)] $$

$$ Sınıf Aralığı = [24 - 10]/[1+3.3log(11)] $$

$$ Sınıf Aralığı \approx 3.1556 \approx 3 $$

Bu şekilde sınıf aralığını 3 buluruz. Sınıf uzunluğu 24 - 10 = 14'tür.

<br>

<table align="center">
  <tr>
    <td colspan="3" align="center">Navigasyon</td>
  </tr>
  <tr>
    <td><a href="https://github.com/zinzinzibidi/istatistik/blob/main/temel-kavramlar.md">&#60;&#60;&#60; Önceki Konu &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</a></td>
     <td><a href="https://github.com/zinzinzibidi/istatistik/blob/main/README.md">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;İçindekiler&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</a></td>
     <td><a href="https://github.com/zinzinzibidi/istatistik/blob/main/merkezi-egilim-olculeri.md">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Sonraki Konu &#62;&#62;&#62;</a></td>
  </tr>
</table>

[^1]: frekans (frequency)
