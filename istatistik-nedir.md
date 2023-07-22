# İstatistik Nedir?

> "İstatistiklerle yalan söylemek kolaydır. Ama onlarsız doğruyu söylemek çok daha zordur."
> Frederick Mosteller

Verilerin toplanması ve derlenmesi sonrası yapılan sayısal analiz ve nicel yorumlama tekniklerinin tümünü ifade eden bilim dalıdır. Dilimizde tam karşılığı olmamakla birlikte “say” kökünden türetilen “sayıtım”, “sayımlama”, “sayım bilimi” gibi terimler istatistik için kullanılan sözcüklerden birkaçıdır. Etimolojisinden de anlaşılacağı üzere “sayılar” istatistiğin temelini oluşturur.

<img src="https://zinzinzibidi.com/img/istatistik/dolar2.png" align="left" style="width:96px;"/> Günlük hayatta sayıların olduğu hemen her yerde istatistik vardır. Arabaya bindiğimizde hız göstergesinin 0’dan 240 km/saate kadar olması bize o taşıtın saatte minimum 0, maksimum 240 km ile gidebileceği bilgisini verir. Dört ay boyunca sırasıyla 600, 800, 1200, 1400 TL tutarlı elektronik eşya satın alan müşteri hakkında toplamda 4000, aylık ortalama 1000 TL elektronik eşya harcaması olduğu sonucuna ulaşabiliriz. Müşterinin her ay harcama tutarını artırdığı çıkarsamasında bulunabiliriz. EURUSD kurunun 1.20 olduğu döviz piyasasında 1 euro’nun 1.20 ABD doları olduğunu söyleyebilir, oranlar yardımıyla 960 doların 800 euro’ya denk geldiğini hesaplayabiliriz. Toplamları, minimumları, maksimumları, ortalamaları ve oranları gördüğümüz birçok alanda aynı zamanda birer istatistik okuyucusuyuzdur. Toplamlar ve ortalamalar istatistiğin görünür hâlidir. Standart sapma, medyan, basıklık ve çarpıklık derecesi, değişim katsayısı gibi ilk bakışta göremeyeceğimiz, fakat yapacağımız analizleri daha anlamlı kılacak birtakım istatiksel kavramlara da gereksinim duyarız. Bu sebeple istatistiğe “anlamlı sonuçlara ulaşmak için kullandığımız matematiksel yöntemler bütünü” de diyebiliriz.

<img src="https://zinzinzibidi.com/img/istatistik/line-chart.png" align="right" style="width:96px;"/> Yıllar sürecek veri bilimi ve veri analizi çalışmalarımızın ve uğraşlarımızın büyük bölümü “karşılaştırmalar” (comparisons) üzerine olacaktır. Günlük hayatta ev ararken kiraya çıkmak istediğimiz konutun diğer mülklere göre büyüklüğünü, konumunu ve fiyatını kıyaslarız. Araba alırken teknik değerlerinin diğer arabalara, hatta önceki arabamıza göre daha iyi olup olmadığına bakarız. Telefon satın alırken markasını, ekran genişliğini, şarj kapasitesini diğer telefonlar ile karşılaştırırız. Veri bilimi adına yaptığımız çalışmalarımız da günlük hayattakinden farklı olmayacak, biraz daha fazla bilgi birikimi gerektiren karşılaştırmalar yapacağız.

Haftada 400, 600, 500, 200, 800 müşteri işlemi yapan A şubesi ile 450, 550, 500, 400, 600 işlem yapan B şubesini karşılaştırdığımızda iki şubenin de günlük ortalama 500 işleme sahip olduğunu söyleyebiliriz. “Bir sonraki iş günü en az 450 müşteri işlemi yapma olasılığı daha fazla olan şube hangisidir?” sorusu sorulduğunda ortalamalar bize anlam ifade etmeyecektir. İstatistikçilerin seri karşılaştırmalarında sıkça kullandığı standart sapma ve değişim katsayısı bu gibi durumlarda kurtarıcımız olacaktır. A şubesinin standart sapması ve değişim katsayısı sırasıyla 224 ve 45, B şubesinin 79 ve 16’dır. Sayıları yorumlamasını bilen istatistikçi bu gibi bir örnekte standart sapması ve değişim katsayısı daha düşük olan B şubesinin günler itibariyle daha istikrarlı işlem yaptığını görebilecek, bir sonraki iş günü B şubesinin en az 450 işlem yapma olasılığının A şubesine göre daha yüksek olduğu sonucuna ulaşabilecektir. Özetle istatistik, veri karşılaştırmalarında bize büyük kolaylık sağlayacaktır.

Karşılaştırmalar en az iki farklı olgu üzerine olabileceği gibi tek bir konu üzerine de olabilir. Bir önceki örnekte iki farklı şubenin karşılaştırmasını yaptık. Sadece A şubesinin bir önceki yıl işlem adetleri ile cari yıl işlem adetleri üzerine karşılaştırma da yapabiliriz.

## İstatistik Kullanım Alanları

Veri bilimi gibi istatistik de disiplinler arası alandır. Astronomide astroistatistik, iktisatta ekonometri, kimyada kemometri, biyolojide biyoistatistik, psikolojide psikometri, sosyolojide sosyometri gibi bilim dallarının oluşmasını sağlamıştır. Günlük hayatta istatistiği görünür hâli ile kullandığımız gibi uzmanlık alanı gerektiren alanlarda istatistiğe daha fazla ihtiyaç duyarız. İstatistik elde ettiğimiz bulguları açıklamamıza, veriler yardımıyla genel ve özel sonuçlara ulaşmamıza yardımcı olur. Çok büyük bir veri seti üzerinde çalışılıyorsa yapılan örneklemeler ile zaman ve maliyet tasarrufu sağlanır.

## İstatistiğin Yöntemleri

<p align="center">
<img src="https://zinzinzibidi.com/img/istatistik/istatistik-yontemleri2.png" style="width:480px; border-radius: 48px;"/>
</p>

<b>Betimsel İstatistik (descriptive statistics)</b>: Verilerin ortalamalar, standart sapmalar, grafikler ile özetlendiği, geçmişe yönelik yorumlandığı istatistik yöntemidir.

<b>Çıkarımsal İstatistik (statistical inference)</b>: Verilerin hipotez testleri, varyans analizi, korelasyon analizi, regresyon analizi gibi tekniklerle hem geçmişe hem de geleceğe yönelik yorumlandığı istatistik yöntemidir.

İki yöntemin yanında az bilinen bir yöntem daha vardır. “Keşifsel Veri Analizi” adıyla tanımlanan bu metodda betimsel ve çıkarımsal istatistikte kullanılan tekniklerin grafikler yardımıyla özetlenmesi esastır. 1960’larda John Tukey tarafından literatüre kazandırılmıştır.
