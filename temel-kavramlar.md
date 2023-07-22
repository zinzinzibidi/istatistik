# Temel Kavramlar

> Veriler tek başına anlam ifade etmezler. Anlam ifade ettikleri zaman adına 'bilgi' deriz.

Bu bölümde istatistikte sıkça kullanılan temel kavramlara değinilecektir. İlerleyen bölümlerde anlatılan kavramların daha net anlaşılabilmesi için mutlaka okunmalıdır.

<b>Veri (Data)</b>: Analiz için elde edilen gözlem değerlerinin tamamı

* <b>Ham Veri (Raw Data, Primary Data)</b>: Verinin işlenmemiş hâli
* <b>İşlenmiş Veri (Processed Data, Secondary Data)</b>: Verinin işlenmiş hâli
* <b>Kirli Veri (Dirty Data)</b>: Ham verinin, veri yazılımlarının işleyemeyeceği derecede hatalı, formatı bozuk ya da boş veri birimleri içermesidir.

<b>Veri Birimi (Data Point)</b>: Veri seti içindeki her bir hücre

<b>Veri Seti (Data Set, Dataset)</b>: Verilerin bütün hâlde depolandığı tablolar

<b>Veri Tabanı (Database)</b>: Veri setlerinin ham veriler içerecek şekilde saklandığı, gerektiğinde istenilen veriye ya da veri setine ulaşılabilen ortam

<b>Değişken (Variable, Var)</b>: Belirli nitelikleri ile farklılık gösteren istatistiksel varlık

<b>Seri (Serie)</b>: Değişkenlere ait değerlerin büyükten küçüğe, küçükten büyüğe, en yakın zamandan en uzak zamana, en uzak zamandan en yakın zamana ya da alfabetik sıralanması

<p align="center">
  <img src="https://zinzinzibidi.com/img/istatistik/temel-kavramlar-excel.png" style="width: 360px;"/>
</p>

Yukarıdaki Excel tablosu, ürünlere ait uzunluk, genişlik ve yükseklik değerlerini içeren basit bir veri setidir. Eğer tabloyu veri tabanından edinirsek adına ham veri diyebiliriz. Ham veriler işlenmemiş verileri içeren tablolardan oluşur. Beyaz hücreler içerisinde gösterilen uzunluk, genişlik ve yükseklik değerleri aynı zamanda birer veri birimidir. Ürün adları mavi alanda gösterilmesine rağmen ürün adları da birer “veri birimi”dir.

Değişkenler “Ürün Adı”, “Uzunluk”, “Genişlik”, “Yükseklik”tir. Her biri farklı özelliğe sahiptir. Ürün adları uzunluk, genişlik ve yükseklik değerlerine göre belirlendiği için, diğer bir ifade ile ürünler uzunluk, genişlik ve yükseklik değerlerine bağlı olduğu için “Ürün Adı” aynı zamanda <b>bağımlı değişken</b>dir. “Uzunluk”, “Genişlik”, “Yükseklik” değişkenleri herhangi bir değer alabilir ve yeni bir ürün adı oluşturabilir. Herhangi bir değer alabilmesi, diğer değişkenlerden etkilenmemesi nedeniyle uzunluk, genişlik ve yükseklik değişkenleri <b>bağımsız değişken</b> olarak ifade edilir. Bağımlı, bağımsız değişken farkını özetleyecek olursak... Ürün4’ün Ürün4 olabilmesi için uzunluk, genişlik ve yükseklik değerleri sırasıyla 20, 15, 15 olmalıdır. Ürün Adı tamamen bu üç değere bağlıdır. Bu sebeple Ürün Adı bağımlı değişkendir. Uzunluk, yükseklik ve genişlik değişkenleri herhangi bir değer alabilir. Diğer değişkenlere bağlı değildir. Bu nedenle bağımsız değişken olarak adlandırılır.

Veri birimlerinin (hücrelerin) bir kısmı #YOK ve benzeri ifadeler içerirse, toplama, ortalama alma gibi işlemler yapılamamakta, veri analistinin işi de zorlaşmaktadır. Bu tür veri setleri “kirli veri seti” olarak adlandırılır. Çok büyük veriler içeren tablolarda kirli verileri görebilmesi zor ve zahmetlidir. Hatalı verilerin nedeni bulunamazsa kirli veriler, veri setinden silinmez. 0 (sıfır) değeri ile değiştirildikten sonra analize devam edilir. Kirli veriler temizlendikten sonra elde edilen verilere işlenmiş veri denir.

İşlenmiş verilerin elde edilmesi için her zaman kirli verilerin temizlenmesi şartı yoktur. Ham veriler kirli veriler içermese bile ondalıklı formatta gösterilen 124,000.56 benzeri değerlerin 124,001 tamsayı formatında gösterilmesi durumunda da veri işlenmiş sayılır ve işlenmiş veri seti oluşturulabilir.

Serilerde değişkenlerden biri mutlaka nümerik ya da alfabetik sıralanmalıdır. Ürün adları alfabetik sıralandığı için bu veri setini aynı zamanda “ürün serisi” olarak adlandırabiliriz.

<p align="center">
  <img src="https://zinzinzibidi.com/img/istatistik/veri-turleri2.png" style="width: 480px;"/>
</p>

Veri türleri (data types) ya da değişken türleri (types of variables) istatistikte modellemeye başlanılmadan önce bilinmesi gereken en önemli konudur. Bu sebeple tam olarak öğrenilmeden analize devam edilmemeli, modelleme aşamasından önce tereddütte kalınması durumunda anlamları tekrar gözden geçirilmelidir.

Veriler genel olarak nitel (qualitative) ve nicel (quantitative) olmak üzere ikiye ayrılır. Nitel veriler saç rengi, cinsiyet, öğrenim durumu gibi sayısal ifadeler içermeyen değişkenlerden oluşur. Nicel veriler sayılabilirdir. Toplama, ortalama alma gibi temel istatistik işlemleri uygulanabilir.

Nitel verilerin tamamı kategorik değişkenlerden elde edilir. Adından da anlaşılacağı gibi üzerlerinde temel sayısal ölçümler yapılamadığı için kategorilendirilir.

> Nominal kelime anlamıyla “görünür”, ordinal ise “sıralı” demektir.

<img src="https://zinzinzibidi.com/img/istatistik/cinsiyet.png" align="right" style="width: 64px;"/> 

<b>Nominal Veri (Nominal Data)</b>: Sayısal olmayan, kendi içinde sıralanamayan değişkenlerden oluşan kategorik veri türüdür.

Saç rengimiz, çalıştığımız kurum, okuduğumuz okul, cinsiyetimiz birer nominal değişkendir.

<img src="https://zinzinzibidi.com/img/istatistik/mezuniyet.png" align="right" style="width: 64px;"/> 

<b>Ordinal Veri (Ordinal Data)</b>: Sayısal olmayan, kendi içinde hiyerarşik olarak sıralanabilen değişkenlerden oluşan kategorik veri türüdür.

Eğitim düzeyi (ilkokul – lise – üniversite), futbol saha mevkileri (defans – orta saha – forvet), “kesinlikle katılmıyorum – katılmıyorum – kararsızım – katılıyorum – kesinlikle kalıyorum” yanıtlarından oluşan anket sorularında kullanılan likert ölçekleri (likert scale) gibi sayısal veriler içermeyen fakat kendi içinde sıralanabilen değişkenlerden oluşur.

<img src="https://zinzinzibidi.com/img/istatistik/sayilar.png" align="right" style="width: 64px;"/> 

<b>Aralıklı Veri (Discrete Data)</b>: 0, 1, 2, 3… gibi tamsayılardan oluşan, ondalıklı sayılar içermeyen nümerik veri türüdür.

Yaş, aralıklı veriye en iyi örnektir. Bir kimsenin yaşını sorduğumuzda “24.9 yaşındayım” yanıtını almayız. 25’ine birkaç hafta kalmasına rağmen “24 yaşındayım.” yanıtını alırız. Somut bir örnek vermek gerekirse tenis kortunda bulunan tenis toplarının sayısı aralıklı veridir. “Sahada 4.6 tenis topu var.” şeklinde sayımlar yapamayacağız gibi bulacağımız toplam değeri daima tamsayı (integer) olacaktır. “Sahada 5 tenis topu var.” gibi…

<img src="https://zinzinzibidi.com/img/istatistik/termostat.png" align="right" style="width: 64px;"/> 

<b>Sürekli Veri (Continuous Data)</b>: 1.24, 2.43 gibi ondalıklı (float) değerler alan nümerik veri türüdür. Bu veri türündeki değerler tamsayı da olabilir. Önemli olan ölçümün ondalıklı sayılarla yapılıp yapılmadığıdır.

Sürekli verilere en iyi örnek bugün kullandığımız termometrelerdir. Sıcaklık değerleri 18, 25, 30 gibi derecelerle gösterilebildiği gibi 17.8, 25.4, 30.2 gibi ondalıklı sayılarla da ölçülebilmektedir.

<p align="center">
  <img src="https://zinzinzibidi.com/img/istatistik/isin.png" style="width: 240px;"/>
</p>

Sürekli verileri matematikteki ışına benzetebiliriz. Işın üzerindeki herhangi bir nokta, verinin sürekli bir değişkene bağlı olduğunu gösterecektir.

<p align="center">
  <img src="https://zinzinzibidi.com/img/istatistik/kesikli-isin.png" style="width: 240px;"/>
</p>

Işını tamsayılara denk gelecek şekilde eşit parçalara böldüğümüzde (eşit aralıklarla kestiğimizde) aralıklı veriler elde ederiz. Aralıklı verilerle oluşturulan değişkenlere aynı zamanda “kesikli değişken” adı verilmesinin sebebi budur.

## Veri Türlerinde Dikkat Edilmesi Gerekenler

<img src="https://zinzinzibidi.com/img/istatistik/kimlik.png" align="left" style="width: 96px;"/> 

Nitel verilerin birer kategorik değişken, nicel (sayısal) verilerin ise nümerik değişkenler olduğunu öğrendik. Kategorik değişkenler çoğunlukla metinsel değerlerden oluşmakla birlikte aralarında hiyerarşik düzen olup olmaması, kategorik değişkenin alt türünü belirlemektedir. Hiyerarşik sıralamanın olması durumunda ordinal, olmaması durumunda nominal veri ayrımını yapabiliriz. Nümerik değişkenler ise tamamen sayısal verilerden oluşur. Veriler ondalıklı ise sürekli, değilse aralıklı (kesikli) olduğunu söyleyebiliriz.

<img src="https://zinzinzibidi.com/img/istatistik/anket.png" align="right" style="width: 96px;"/> 

Nitel verilerin birer kategorik değişken, nicel (sayısal) verilerin ise nümerik değişkenler olduğunu öğrendik. Kategorik değişkenler çoğunlukla metinsel değerlerden oluşmakla birlikte aralarında hiyerarşik düzen olup olmaması, kategorik değişkenin alt türünü belirlemektedir. Hiyerarşik sıralamanın olması durumunda ordinal, olmaması durumunda nominal veri ayrımını yapabiliriz. Nümerik değişkenler ise tamamen sayısal verilerden oluşur. Veriler ondalıklı ise sürekli, değilse aralıklı (kesikli) olduğunu söyleyebiliriz.

Aynı şekilde anket sorularındaki 1’den 3’e kadar olan seçeneklere verilen yanıtları analiz etmek istediğimizde, istatistik yazılımında veri türünü “aralıklı veri” (discrete data) belirlememeliyiz. Anket soruları 1’den 3’e kadar “katılmıyorum - kararsızım - katılıyorum” değerlerinden oluşan, kendi içerisinde hiyerarşik düzeni olan verilerdir. Bu sebeple bu tür anketler ordinal veri türü ile oluşturulur, ordinal veri türüne ait istatiksel yöntemler uygulanır.

İstatistikte veri türleri başta kafamızı karıştırabilir. Tam olarak anlaşılması zaman almaktadır. Net olarak görülmemesine rağmen birbirlerinden kesin çizgilerle ayrılmışlardır. İstatistiksel modellemelere başlanılmadan önce veri türlerinin sisteme doğru tanıtılması analizlerimizin de doğru sonuçlanmasını sağlayacaktır. Hatalı veri türü ile yapılan modellemeler ve analizler hatalı sonuçlar doğuracaktır. Veri türleri bu yüzden başlangıç aşamasında kritik öneme sahiptir.

<br>

<table align="center">
  <tr>
    <td align="center">Veri Türleri ile ilgili YouTube videosu</td>
  </tr>
  <tr>
    <td><a href="https://www.youtube.com/watch?v=kyjlxsLW1Is" target="_blank">Teach me STATISTICS in half an hour!</a></td>
  </tr>
</table>

<br>

<p align="center">
  <img src="https://zinzinzibidi.com/img/istatistik/anakutle-ve-orneklem.png" style="width: 480px;"/>
</p>

## Anakütle ve Örneklem

<b>Anakütle (Population)</b>: Araştırma konusu tüm veri birimlerini içeren küme

Kimi kaynaklarda “anakitle”, “popülasyon”, “yığın”, “evren” terimleriyle ifade edilir.

Toplam nüfus, 2020 yılında üniversite okuyan öğrencilerin sayısı, 2021 yılında tüm banka çalışanlarının sayısı anakütleye örnektir.

<b>Örneklem (Sample)</b>: Araştırma konusu anakütleden belirli sayıda veri birimi seçilerek oluşturulan küme

2021 yılında tüm banka çalışanların sayısını anakütle olarak göstermiştik. Türkiye Bankalar Birliğinin verilerine göre Haziran 2021’de toplam 180,019 mevduat bankası çalışanı bulunmaktadır.1 Çalışanların 61,268’i kamu bankalarında, 118,751’i özel bankalarda çalışmaktadır. Kamu ve Özel Bankalarda aynı pozisyonda çalışanların maaş ortalamalarını karşılaştırmak istediğimizde 180,019 birim içerisinde araştırma konusu pozisyonda çalışan tüm personellerin maaşlarını tespit etmek neredeyse imkânsızdır. Bu sebeple her iki kümeden de belirli sayıda örnek seçip ortalamaları hesaplamak gerçeğe en yakın sonucu verecektir. Kamu bankalarında uzman pozisyonunda çalışan 120, özel bankalarda eşdeğer pozisyonda çalışan diğer 120 personelden oluşan 2 örneklem kümesi seçtiğimizde yaptığımız seçime örnekleme deriz. Hem kamu hem de özel bankalarda çalışanların maaş ortalamalarını incelediğimizde ortalama, standart sapma, medyan gibi önemli göstergelere ulaşabilir, anakütleye ait parametreleri doğru tahmin edebiliriz.

### İstatistik ve Parametre Arasındaki Fark Nedir?

Parametre (parameter), anakütleden elde edilen ortalama, standart sapma ve benzeri göstergelerdir. İstatistik (statistic), örneklemden elde edilen aynı göstergelerin parametreyi tahmin etmek amacıyla kullanılmasıdır. Merkezî Eğilim Ölçüleri bölümünde konu detaylı olarak incelenecektir. Şimdilik sadece istatistik denilince aklımıza örneklem’in (sample), parametre denilince de anakütle’nin (population) gelmesi yeterlidir.

### İstatistikçiler Neden Örneklem Seçimi Yapar?

<img src="https://zinzinzibidi.com/img/istatistik/durbun.png" align="left" style="width: 96px;"/>

Örneklemdeki amaç yığın parametrelerine ulaşılmasının zahmetli, maliyetli ve çok fazla zaman almasından kaynaklanmaktadır. Eğer elimizde inceleme konusu kümenin tüm veri birimlerini içeren veri seti yoksa örneklem modellemeleri oluşturmak anakütleyi temsil etmenin en sağlıklı ve en güvenilir yoludur. Bu sebeple örneklem modellemeleri yapmak hem daha az zahmetli hem de daha az zaman alan temel istatistik yöntemdir. Anketler örneklemede en sık kullanılan araçlardır. İnceleme konusu popülasyondan seçilen belirli sayıdaki örneğe ait veri, anakütle parametrelerini tahmin etmek için kullanılır.

### Örneklem Seçiminin Doğru Yapılması Neden Önemlidir?

<img src="https://zinzinzibidi.com/img/istatistik/istanbul.png" align="left" style="width: 164px;"/>

İstanbul Yerel Seçimleri için anket çalışması yaptığımızı ve 1000 kişiden oluşan veri setimiz olduğunu varsayalım. Eğer tüm İstanbul nüfusu içerisinden sadece Beşiktaş’ta oturan 1000 kişiye anket sorularını yöneltirsek anket sonuçları hatalı olacaktır. Çünkü anket sonuçları Beşiktaş’ta kimin belediye başkanı olabileceğini doğru tahmin edebilmesine rağmen İstanbul genelinde kimin büyükşehir belediye başkanı olacağını doğru tahmin edemeyecektir. Bu sebeple 1000 birimin “nüfus yoğunluklarına göre” ilçelere bölüştürülmesi, anket sorularının bu ilçelerde oturanlara sorulması anakütle parametrelerini doğru tahmin etmemizi sağlayacaktır.

<img src="https://zinzinzibidi.com/img/istatistik/tuik.png" align="right" style="width: 186px;"/> 

Örneklem seçiminin resmî anlamda yapıldığı diğer bir örnek Türkiye İstatistik Kurumu (TÜİK) tarafından düzenli olarak hesaplanan “işsizlik oranı”dır. İşsizlik oranı hesaplanırken tüm ülke nüfusunun iş durumunu tespit etmek imkânsıza yakın olduğu için 58,560 hanehalkına2 anket soruları yöneltir. Katılımcılara son 4 haftada iş arayıp aramadıkları sorulur.3 Toplam 24,604,086 hanehalkının sadece %0.24’üne denk gelen 58,560 birimlik hanehalkı ile işsizlik oranları hesaplanır.4 Anakütlenin yüzde 1’i bile olmayan örnekleme yapılır. Biraz önce de belirttiğimiz gibi önemli olan parametrelerin doğru tahmin edilmesidir. Örneklem büyüklüğü arttıkça parametreler de gerçeğe en yakın tahmin edilebilecektir.

## Sıra Sizde

<b>Uygulama</b>: Kahverengi, sarı ve siyah değişkenlerinin veri türü nedir?

A) Nominal veri <br>
B) Ordinal veri <br>
C) Aralıklı veri <br>
D) Sürekli veri

<details>
<summary>Yanıtı Göster</summary>
<br>Saç renkleri kendi içerisinde hiyerarşik sıralanamadıkları için ve nümerik veriler olmamalarından dolayı <br>nominal veri</b> türünde değerlendirilir.
</details>

<br>

<b>Uygulama</b>: 64, 43, 50, 75 ve 80 notları ne tür bir veri türüdür?

A) Nominal veri <br>
B) Ordinal veri <br>
C) Aralıklı veri <br>
D) Sürekli veri

<details>
<summary>Yanıtı Göster</summary>
<br>Nümerik veriler ondalıklı değerler almadıkları sürece aralıklı veri türünde değerlendirilir.
</details>

<br>

<b>Uygulama</b>: Anket yanıtları "düşük", "orta" ve "yüksek" olan değişkenler hangi veri türünde değerlendirilir?

A) Nominal veri <br>
B) Ordinal veri <br>
C) Aralıklı veri <br>
D) Sürekli veri

<details>
<summary>Yanıtı Göster</summary>
<br>Anket sorularına verilen yanıtların neredeyse tamamı ordinal veri türünde değerlendirilir. Ordinal veriler, kendi içinde hiyerarşik sıralamaya sahip verilerden oluşur.
</details>

<br>
