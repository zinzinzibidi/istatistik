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
  <img src="https://zinzinzibidi.com/img/istatistik/veri-turleri.png" style="width: 480px;"/>
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

<img src="https://zinzinzibidi.com/img/istatistik/kimlik.png" align="left" style="width: 64px;"/> 

Nitel verilerin birer kategorik değişken, nicel (sayısal) verilerin ise nümerik değişkenler olduğunu öğrendik. Kategorik değişkenler çoğunlukla metinsel değerlerden oluşmakla birlikte aralarında hiyerarşik düzen olup olmaması, kategorik değişkenin alt türünü belirlemektedir. Hiyerarşik sıralamanın olması durumunda ordinal, olmaması durumunda nominal veri ayrımını yapabiliriz. Nümerik değişkenler ise tamamen sayısal verilerden oluşur. Veriler ondalıklı ise sürekli, değilse aralıklı (kesikli) olduğunu söyleyebiliriz.
