---
layout: default
title: "LCD Rehberi: Temel Yapı, Panel Tipleri ve Tüm Detaylar"
date: 2026-09-24
categories: [Paneller, LCD]
---

# LCD Rehberi

Selamlar, rastgele şeyler hakkında rastgele rehberler yayımlamak adlı bir hedefim vardı ve bugün paneller ile başlayacağız. Eğer zamanım olursa ve ilgi de artarsa OLED ve diğer paneller için de gelecek. Sonradan diğer donanım kollarında da bilgilendirmek isterim.

Rehberimizde amacımız üstünkörü panelleri anlatmak değil; neyin ne olduğunu, neyin neyi etkileyip değiştirdiğini ve en çok sorulan soruların çoğunu yanıtlamaya ve anlamayanlar için anlatmaya çalışacağım. Temel ama biraz klişe bilgilerle başlasak da bu bilgiler bilmeyenler için bir rota olacak, geri kalan yerlerde ise neyin ne olduğunu çözümleyeceğiz. Şimdiden iyi okumalar, okuduğunuz ve okuyacağınız için teşekkürler.

## Giriş

Daha konuya başlamadığımız için 0 yazdım. Bundan yıllar öncesini biliyorsunuz, tüplüler vardı. Buraları anlatmama gerek yok; insanlar ince ekran istiyordu ama o zaman yoktu. LCD ilk meyvelerini 2000'lerin sonrasında verse de 1968'de ilk kez laboratuvarda üretilen bir teknolojidir ama yaygınlaşamadı. LCD'nin isminden de anlaşılacağı üzere sıvı kristaller ise 1888'de bulunmuştur. Bulan kişi de süper zeki bir mühendis değil, Avusturyalı botanikçi Friedrich Reinitzer; kolesterol türevlerini incelerken bulmuş ama önemsememiştir. 1968'de de ilk prototip çıkmıştır. İlk çıkan panel de TN olup Sharp'ın EL-805 modelinde kullanılan hesap makinesidir ama renksizdir. İlk renkli TN ise 1988'de çıkan 14" bir Sharp monitördür ama yaygınlaşamadı çünkü fiyatlar Elon Musk'ın bile alamayacağı seviyedeydi. Ayrıca şu an dünyanın en yaygın ekranı olan LCD'yi bulan adamın da tekrar hatırlatalım: süper zeka değil, botanikçi olduğunu. Kendinizi üzmeyin.

## 1) Temel LCD Yapısı

LCD dediğimiz ekran teknolojisi OLED, CRT veya Micro-LED veya plazma gibi kendinden ışımalı değil, arka ışımalıdır. Görüntü için arka ışık gerekir. Günümüzde çok ucuzdur ve üretim verimi %95 seviyelerine kadar çıkmıştır. Birkaç basit katmandan oluştuğu için maliyeti düşüktür. LCD'leri asıl çalıştıran şey sıvı kristal dediğimiz yapılardır; voltaj ile garip davranışlar sergilerler.

Kimyasal formülü = C₁₈H₁₉N
Yapısı = C₅H₁₁—C₆H₄—C₆H₄—CN
Telaffuz = 4-pentil-4'-siyanobifenil (5CB)

LCD'de arka ışıktan çıkan fotonlar önce arka polarizöre çarpar. Burada tek açıya indirgenen fotonlar sıvı kristallerden belirli açılar ve güçlerle geçerek renk filtresinden geçer. Ardından son olarak ön polarizörden de açı uygunluğuna göre geçerek/geçemeyerek renk oluştururlar. Temel mantıkları budur.

### LCD'de 6 Katman Bulunur

1. Arka ışık
2. Arka polarizör
3. TFT katman
4. Sıvı kristal
5. Renk filtresi
6. Ön polarizör

#### Arka Işık

Işığı sağlayan tabakadır, farklı türleri vardır. Biz en çok kullanılan tür olan WLED'i baz alacağız. Renk kalitesi, kontrast, parlaklık ve daha onlarca şeyi etkiler; bundan da ileride bahsedeceğiz. Işığı üretir ancak buradan çıkan ışık saçaklı, titreşimli ve dağınıktır. LCD için dümdüz, titreşimsiz ve saçaksız ışık gerekir; bu yüzden arka polarizöre ihtiyaç duyarız. Işığın üretim yeri burasıdır. Arka ışıkta difüzör ve kılavuz plaka adlı noktalar vardır ama bunları anlatmamıza gerek yok, kafa karıştırmayalım.

#### Arka Polarizör

Arka ışıktan çıkan saçaklı, titreşimli ve dağınık ışığı alarak ışığı ve titreşimi tek bir düzleme döker. Arka polarizör üzerine gelen ışıktan sadece belli açıdakileri geçirip geri kalanları bloklayarak bu işlemi yapar; böylece ışık hazır ve tek bir açıya indirgenmiştir. Arka polarizör ile ön polarizör birbirine 90° açıyla yerleştirilmiştir.

#### TFT Katman

Thin Film Transistor demektir, yani ince film transistör. İçinde bildiğimiz transistörler vardır; ona gelen emri voltaja dönüştürerek emrindeki sıvı kristale basar ve onun açısını değiştirerek temel işi yapar. Çok ince ve film şeklindedir ve şeffaftır. Sayısı hesaplanabilir: Bir piksel 3 alt pikselden oluştuğu için her pikselin 3 transistörü vardır. 1920x1080 ekranda 2.073.600 piksel vardır, yani toplam 6.220.800 transistörlük bir TFT katman vardır ekranda.

#### Sıvı Kristal

Sıvı kristal katman ışığı belli açılarda bükerek/değiştirerek renk filtresine ulaştırır, görüntüyü oluşturan katmandır. Tam sıvı değil, tam da katı değildir; normalde sıvı olsa da elektrik alanına karşı yön değiştirir. Bu yüzden voltaj uygulanınca konumunu fiziksel olarak değiştirir, bu da ışığı kontrol etmemizi ve renk oluşturabilmemizi sağlar. TN ve IPS/VA panellerde farklı şekilde panele enjekte edilir ve farklı şekilde çalışırlar. Bunu ileride anlatacağız ama şu anlık kafanız karışmasın diye temel geçiyoruz.

Kısa çalışma diyagramı: Diyelim pikselin 133-156-100 renginde yanması gerek, bu renk isteniyor. Sıvı kristal voltaj yiyerek kırmızı (R) alt pikseli 133 seviyesi kadar parlak yakar, yeşil alt pikseli 156 seviyesi kadar parlak yakar (G) ve mavi alt pikseli 100 seviyesi kadar parlak yakar (B). Böylece bu renkler beynimizde karışarak sanki tek bir renkmiş gibi gözümüze çarpar. Parlaklık değeri 8-bit renk derinlikli bir panel için 0-255 arasında değer alabilir, 6-bit için 0-63, 10-bit için 0-1023 gibi. Bunu da ileride anlatacağız.

#### Renk Filtresi

Az önce anlattığımız gibi rengi oluşturan merkezdir. Bir pikseli 3x3 birim bir kare olarak düşünürsek kırmızı alt piksel (R) 1x3 birim, yeşil alt piksel (G) 1x3 birim, mavi alt piksel (B) 1x3 birim yer kaplar ve tam bir kare piksel oluştururlar. Piksellerin etrafındaki siyah kısma ise ızgara yani "Grid" denir.

#### Ön Polarizör

Işığın uğradığı son noktadır. Gerçek siyah oluşumu burada olur. Sadece onunla uyumlu derecedeki ışığı geçirir, geri kalan ışığı bloklar ve siyaha dönüştürür. Arka polarizöre 90° dik olarak yerleştirilir. Biraz karmaşık olduğu için ileride detaylı anlatacağız.

## 2) 3 Temel Panel ve Davranışları

3 temel panel olduğunu biliyoruz ama neden 3 ve bunlar gerçekten ne? Amacımız burada bunları öğrenmek. Klişe bilgiler de olacak pek bilinmeyen bilgiler de ama biz herkese hitap ediyoruz; her şeyi yazmamız gerekli.

### Neden Sadece 3 Temel Panel?

Çünkü sıvı kristaller voltaja karşı en fazla 3 pozisyona geçebilir, doğalarında sadece 3 temel tepki vardır:

- TN → Voltaj alınca dikleşir
- VA → Voltaj alınca yana yatar
- IPS → Voltaj alınca kendi düzleminde döner

Bu yüzden 3'ten fazla panel üretmek mümkün değildir. Ne yaparsak yapalım sıvı kristaller bu üç hareketten birini yapacaktır, burada fizik bizi tokatlar. Geri kalan yan paneller bu temel panellerin çakması ve hafif iyileştirilmiş versiyonlarıdır.

### İlk Temel Panel - TN

İlk üyesi ve LCD'nin babasıdır. 1972'de ilk kez prototip olarak çıktı. Üretimi iyice bitse de hâlâ hayatımızda; verimi en yüksek panel ve maliyeti en düşük paneldir. IPS ve VA'dan farklı olarak normalde beyaz bir paneldir. Voltaj verildiğinde ve verilmediğinde farklı davranışlar sergiler.

**Voltaj verilmediğinde:** Sıvı kristal molekülleri iki cam sandviç arasında 90° heliks yani spiral ve bükülmüş şekilde enjekte edilir. Böylece arkadan gelen ışığı voltaj yokken tam 90° büker, böylece ışık ön polarizörle tam uyumlu hale geçerek beyaz rengi oluşturur. TN bu yüzden normalde beyazdır.

**Voltaj verildiğinde:** Sıvı kristaller elektrik alanının etkisi ile spiral yapıyı terk ederek dikleşir. Işık bükülmez, ön polarizöre gelen ışık bloke olur; böylece piksel siyah olur. Siyah renk için voltaj uygulanması gerekir.

**Panelin Genel Özellikleri:** TN'deki sıvı kristallerin hareket edeceği yol çok çok kısa olduğu için hızlılardır, düşük voltajda bile çok hızlı hareket edebilirler çünkü yolları kısadır.

Ama moleküller tam dikleşmediği için yandan bakınca renkler sapar ve negatife döner. Yandan bakınca bozulmanın sebebi budur, görüş açısı 45°/45°/45°/45° civarındadır.

Renk ve kontrast performansları da epey kötüdür. Bunun nedeni yine sıvı kristalin tam dikleşememesidir, ışığı kaçırırlar. Hem ışık kaçtığı için siyah performansları düşer hem de renkler olduğu gibi olmaz. Ayrıca genelde maliyet ve e-spor odaklı paneller olduğu için zaten renk amaçlanmaz. TFT katmanları ise ucuz olur ve genelde 6-bit olurlar. En ucuz paneldir.

### İkinci Temel Panel - VA

İkinci gelen üyesi, ilk prototipler 1990'larda çıkmıştır. Üretimi hâlâ vardır; özellikle QLED VA paneller TV'lerde, mini-LED VA paneller bazı laptoplarda kullanılmaktadır. Rapid VA ismiyle hızlandırılmış versiyonları hâlâ oyuncu monitörlerinde sinematik oyun odaklı olarak satılır, e-spor için pek uygun değildir. Kontrast oranları epey güzeldir.

**Voltaj verilmediğinde:** TN'den farklı olarak normalde siyah bir paneldir. Sıvı kristaller iki cam sandviç arasına dikey olarak enjekte edilir, böylece bu konumda ışık hiç bükülmez ve ön polarizörle uyumsuz olduğu için engellenir. Voltaj yokken siyahtır. Tam dik olduğu için ışığı mükemmel engelleyebilir ve mükemmel kontrast oranlarına sahiptir.

**Voltaj verildiğinde:** Elektriksel alanın etkisi ile dik duran moleküller yana doğru yatmaya başlar ve yatmaya başladıkça ışık bükülür. Voltajı arttırdıkça ışık daha da bükülür ve ön polarizörle uyumlu hale gelir, böylece beyaz oluşur. Ama VA panellerde sıvı kristalin yolu aşırı uzun olduğu için oldukça yavaştırlar. Buna VA Smearing denir.

**Panelin Genel Özellikleri:** Kontrast oranı 3000:1'den başlayarak 6000:1 hatta ötesine kadar çıkar. Tam dikleşebildiği için ışığı hiç kaçırmaz, renk doğruluğu da kabul edilebilir bir seviyedir. Görüş açısı 89°/89°/89°/89° olsa da yandan bakılınca hafif bozulur ama yine de çok geniştir. Sinematik oyunlar oynamak isteyip OLED'e parası yetmeyenler için önerilir. Ancak hızlı anlarda sıvı kristalin gitmesi gereken yol çok uzun olduğu için yavaştırlar. TN'den pahalı, IPS'ten ucuzdur.

### Üçüncü Temel Panel - IPS

En sevilen ve kral sayılan paneldir. Renk ve geniş açı şampiyonu olsa da kontrastı ortalamadır. İlk prototip 1996'da çıktı. En çok üretilen LCD paneldir; Fast IPS monitörlerde, QLED IPS TV'lerde, mini-LED IPS profesyonel laptoplarda kullanılır ve buna benzer türevleri vardır. Her şeyde ortalama bir panel desek yanlış olmaz. Aynı VA gibi normalde siyah bir paneldir.

**Voltaj verilmediğinde:** Sıvı kristal molekülleri iki cam sandviç arasına yatay olarak enjekte edilir. Ne dik ne heliks şekilde, sadece dümdüz yatay; böylece kendi eksenlerinde dönerler. Yolları kısa olduğu için hızlıdırlar. Voltaj yokken ışığı hiç bükmezler, böylece olduğu gibi geçen ışık ön polarizör ile tersleşir ve bloke edilir. Böylece normalde siyah bir paneldir, voltaj yokken siyahtır.

**Voltaj verildiğinde:** Elektriksel alan ile bulundukları eksende dönmeye başlarlar. Voltaj arttıkça daha da çok dönerler, böylece ışığı bükerler ve ön polarizör ile uyumlu hale getirirler. Voltaj verildiğinde beyazlardır.

**Panelin Genel Özellikleri:** Moleküller sürekli yatay kaldığı için gerçek 89°/89°/89°/89° izleme açılarına sahiptir, hiçbir şekilde yandan bakınca bozulmazlar. Renk doğruluğu da oldukça iyidir. Ancak pikseller ışığı biraz kaçırdığı için kontrast oranları düşüktür; genelde 1000:1'den başlar, en fazla 2000:1'e kadar çıkarlar. Kontrast düşüklüğü IPS glow dediğimiz soruna yol açar. OLED'in çakma kuzeni sayılır, VA ve TN'den pahalıdır.

## 3) Yan Paneller

PLS, AHVA, IGZO, MVA, SVA, PVA... Bunlar tam bir panel değildir. Fizik kanunları katıdır; sıvı kristal panelleri temelde sadece 3 şekilde olabilir. Bunlar patent ihlalinden kaçmak için uydurulan ve "biz yaptık" demek için çıkan şeylerdir.

### PLS

Samsung'un IPS patent parası ödememek için uydurduğu şeydir, IPS ile aynıdır. Açılımı Plane-to-Line Switching demektir, küçük parlaklık farkı vardır. MSI'ın IPS-level yazan panelleri de PLS'dir; IPS ve PLS isim hakkı vergisi ödememek için IPS-level yazarlar.

### AHVA

Çinli üretici AUO'nun IPS patent parası ödememek için uydurduğu paneldir, aslında IPS'dir, VA değil. Açılımı Advanced High Viewing Angle'dır, IPS'ten farkı yoktur.

### IGZO

Panel bile değildir ama panel gibi yazılır, bu yanlıştır. IGZO, Sharp'ın patentlediği bir TFT teknolojisidir. IGZO denen bir maddeyi kullanarak daha dinamik, daha hızlı ve daha verimli anahtarlama yapan bir TFT materyalidir. Açılımı Indium Gallium Zinc Oxide'dir.

### ATW

IPS'e eklenen özel bir polarizör ile kontrastı 2000:1'e kadar çıkarıp IPS Glow'u neredeyse yok eden bir teknolojidir, LG patentlemiştir, panel değildir.

### MVA

Fujitsu'nun patentten kaçmak için yaptığı çakma paneldir, VA'dır aslında. Açılımı Multi-Domain VA'dır; her pikseli bir sürü bölgeye ayırarak gerçek 89°/89°/89°/89° açı sunduğunu beyan eder.

### PVA ve SVA

Yine aynı dava, Samsung'un VA panelleridir. Açılımları Super ve Patterned Vertical Alignment demektir.

### WVA

BOE'nin çakma VA teknolojisidir, açılımı Wide Viewing Angle'dır.

## 4) Arka Işık Tipleri

LCD arkadan ışımalıdır, bu yüzden arka ışıkları da bilmek gerekir. Arka ışığın türü ve saflığı her şeyi değiştirir. Günümüzde piyasa kendini genelde WLED, QLED ve mini-LED'e bıraktı.

### Arka Işığın Etkilediği Birimler

- Parlaklık
- Kontrast
- Renk gamutu
- Kalınlık ve tasarım
- Ekran homojenliği
- Işık sızması
- Güç tüketimi
- Titreşim
- Ömür

Görüldüğü üzere her şey burada bitiyor.

### CCFL

Cold-Cathode Fluorescent Lamp demektir. LCD'nin ilk dönemlerinde kullanılmıştır. Işıklandırmada bir sürü minik floresan lamba vardır. Evlerdeki floresan lambalar gibi içindeki cıva buharı elektrikle uyarılır ve UV ışık yayar; bu UV ışık floresan kaplamaya çarparak beyaz ışık olur. Çok geniş renk gamutları sunabilir, oldukça homojen şekilde ışığı yayar. Ancak oldukça kalındır, aşırı ısınır; zamanla parlaklığı düşer, sararır. Cıva çevreye çok zararlıdır. Zamanla parlaklığı artar, maksimum parlaklık için birkaç dakika beklemek gerekir, hemen sönmez. Durum: Öldü.

### WLED

Açılımı beyaz LED olsa da beyaz LED diye bir şey yoktur, bu LED'ler bildiğimiz LED de değildir; özel olarak üretilmiş SMD LED'lerdir. WLED mavi bir LED'in üstüne sarı fosfor kaplanarak oluşur, ikisi karışarak beyaz oluşur. Çok ince, çok hafif ve çok verimlidir. Çevreye zararsızdır, hemen yüksek parlaklığa ulaşır, oldukça uzun ömürlüdür. Ancak beyaz ışıkta olsa da mavi ışık ağırlıklıdır, bu yüzden kırmızı ve yeşil tonlar biraz sönük kalabilir. Renk gamutu olarak CCFL'den kötüdür. Ucuz olduğu için en yaygın arka ışık türüdür.

### RGB-LED

WLED'in renk sorununu çözmek için çıkmıştır, üst seviye ve pahalıdır. WLED yerine tek tek kırmızı, mavi ve yeşil LED'ler kullanılır. Bunlar saf renktir ve karışarak saf beyazı oluştururlar. Çok çok geniş renk gamutu sunarlar, renk doğruluğu üst düzeydir. Ama oldukça pahalıdır ve çok yer kaplar, aşırı ısınır, zamanla renkler kayar. Durum: Öldü.

### GB-R LED

RGB-LED çok pahalı olduğu için çıkmıştır. Maliyeti WLED'den çok olsa da RGB-LED'den daha düşüktür. Yeşil ve mavi LED'ler üstüne kırmızı fosfor kaplanır. Neredeyse RGB-LED kadar renk gamutu sunar, çok daha düşük maliyetle üretilir ama verimi düşüktür. Durum: Öldü.

### QLED

WLED'in sorununu çözen bir teknolojidir. Arka ışık klasik WLED olsa da panele Quantum Dot filmi eklenir. Işık bu nano kristallere çarpınca saf mavi ve saf yeşile dönüşür. WLED'in maliyet ve verimlilik avantajı korunurken RGB-LED kadar geniş renk gamutu elde edilir. WLED'den hafif pahalıdır ama iyice maliyetleri düştü. Özellikle QLED IPS ve QLED VA türevleri TV'lerde kullanılır, oyuncu monitörlerinde de kullanılır.

### Mini-LED

OLED katili olarak adlandırılan bir teknolojidir. Geleneksel devasa WLED'ler yerine minnak binlerce (2000+) WLED kullanılır. Böylece bölgesel karartma yapılarak 1.000.000:1'e kadar dinamik kontrast elde edilir. Ayrıca bir sürü aydınlatma bölgesi sayesinde 1.000 cd/m² üstü parlaklıklar elde edilir, en gerçek HDR deneyimi burada yaşanır. Ama fiyatları epey pahalıdır, OLED'i öldürecek kadar ucuz değillerdir. Etrafı siyah ortası parlak nesnelerde Halo etkisi olur. Mini-LED IPS ve mini-LED VA popülerdir, üst düzey TV ve laptoplarda kullanılır.

## 4.5) Arka Işık Yerleşim Tipleri

3 adet arka ışık yerleşim tipi vardır. Arka ışığın kendisi kadar yerleşimi de önemlidir.

### Edge-lit

LED'ler panelin sadece kenarlarına yerleştirilir, genelde alt-üst ya da sağ-sol. Işık bir kılavuz plaka ile komple ekrana yayılır. Aşırı ince ve hafif paneller Edge-lit sayesinde olur, böylece ultra ince ekran ve laptoplar ortaya çıkmıştır. Maliyeti çok daha düşük ve üretimi çok daha kolaydır ama çok ciddi ışık sızması olur, ışık homojen yayılmaz, parlaklık köşelerde toplanır.

### Direct-lit

LED'ler panelin arkasına yaydırılarak yerleştirilir, böylece homojenlik artar ve ışık sızması düşer. Ama panel oldukça kalın olur, bütçe çözümüdür.

### Full-Array-lit

LED'ler panelin arkasına yüzlerce veya binlerce olacak şekilde yerleştirilir, mini-LED'in çalışma mantığı budur. Local dimming yapılarak karanlık olması gereken bölgedeki LED'ler tamamen kapanarak OLED-vari siyahlar sunar. Dimming bölgeleri zone denen bölgelere ayrılır. Ancak panel kalınlığı yine artar, maliyet çok yüksektir ve ısınırlar, pek de verimsizdirler.

## 6) Ekran Kaplamaları

Panel üretimden çıktığı zaman üstüne bir kaplama yapılır, burada iyi kötü yoktur, herkesin tercihine göre değişir.

### Glossy (Parlak) Kaplama

Yüzeyi pürüzsüzdür, böylece ışığı hiç dağıtmaz ve olduğu gibi gösterir. %8 civarı yansıma yapar. Keskinlik kaybı, renk kayması, parlaklık düşmesi ve kumlu görüntü olmaz; ama dışarıdan gelen en küçük ışıkta ekran aşırı parlar ve görülmez. Çok fazla parmak izi ve toz tutar.

### Mat Kaplama

Yüzeyi ışığı dağıtması için kumlandırılmış ve pürüzleştirilmiştir. Böylece dışarıdan gelen ışığı dağıtır ve geri yansıtarak görünürlüğü arttırır, parmak izi ve toz tutmaz. Ancak ekrandan gelen ışığı da dağıtır, kumlanma yapabilir; renkler biraz kayar, parlaklık düşer, keskinlik azalır. Işığın %2 civarını geri yansıtır.

### Yarı-Mat Kaplama

Yarı yarıya bir çözümdür, ikisinden de azar azar bir şeyler alır. Işığın %4 civarını geri yansıtır. Yansıma Glossy'e göre az, Mat'a göre fazladır. Renkler daha az kayar, parlaklık daha az düşer, kumlanma etkisi azdır.

### Gorilla Armor Türevleri (Ekstra Bilgi)

Özel bir nano kaplama kullanarak ışığın sadece %1'ini geri yansıtır ama hiçbir şekilde ekran kalitesini bozmaz; bu TFOC denen nano kaplama ile olur. Dışarıdan gelen ışıklar özel katmanlar ile birbirine çarpıştırılır ve yok olur. Büyük ekranlarda olmaz, maliyeti çok yüksektir; sadece bazı S Ultra serilerinde var.

## 7) Renk Gamutu ve Renk Derinliği

İki kavram birbirine yakın olsa da farklıdır birbirinden.

### Renk Gamutu

Ekranın gösterebildiği tüm renk aralığıdır. Ne kadar genişse o kadar canlı ve doğru renkler gösterebilir. Renk gamutu standartları iç içe geçmiş haldedir. "Hangi renkler?" sorusunun cevabı bu olur, arka ışık kalitesine bağlıdır.

### Renk Derinliği

O renk aralığındaki ton sayısıdır, bit üzerinden değer alır. TFT tabakasının kalitesine bağlıdır. Ne kadar gelişmiş TFT katmanı ve hassas voltajlama, o kadar geniş ton. "Kaç farklı ton?" sorusunun cevabıdır.

### Renk Gamutları

İnsan gözünün görebildiği tüm renkler CIE 1931 adlı bir uzaydır ama teknoloji insandan geri :) Bu yüzden farklı sınırlar vardır:

**sRGB:** Dünyanın en çok kullanılan ve standartlaşmış bir gamutudur, bu yüzden çoğu içeriğe uyumludur ve yeterlidir. %100 sRGB ekranlar idealdir. Bütçenizi ayırıp laptop almadan önce ilk bakacağınız şey GPU veya CPU'dan önce ekranın tipi ve renk gamutu olsun. %45 NTSC çöp ekranlarla hiçbir şeyin zevki çıkmayacaktır. Laptop şirketleri de insanlar bilgisiz diye hâlâ bize bu çöp %45 NTSC panelleri reva görürler; biz almazsak üretmezler. O yüzden en az %100 sRGB monitörlere bakalım, kimse RDR 2'de manzara izlerken renkleri çamaşır suyu ile yıkanmış şekilde görmek istemez.

**Adobe RGB:** Profesyonel fotoğrafçılar kullanır, özellikle baskı işlerinde standart bir renk gamutudur. sRGB'ye göre mavi ve yeşil tonlarda çok daha geniş, kırmızı tonlarda biraz daha geniştir. Kabaca %100 sRGB, %75 civarı Adobe RGB eder.

**DCI-P3:** Sinema endüstrisi standardıdır. sRGB'den özellikle kırmızı tonlarda çok daha geniştir. Kabaca %100 sRGB, %80 civarı DCI-P3 eder.

**BT.2020 (Rec. 2020):** En geniş renk uzayıdır ama şimdilik hiçbir profesyonel monitör %100 BT.2020 gamutuna ulaşamamıştır; şu an için en fazla %85 BT.2020'ye ulaşabildik, geleceğin gamutudur. %100 sRGB kabaca %58 BT.2020 eder.

**NTSC:** Tüplü TV standardıdır ama çok eski kaldı artık, 1953'te ABD'de standartlaştı. %100 sRGB kabaca %72 NTSC eder. Ultra ucuz panellerde gördüğümüz %45 NTSC ibaresi kabaca %62.5 sRGB eder.

### Renk Derinliği Değerleri

Her bir alt pikselin kaç seviyeye kadar tonlama yapabildiğini gösteren değerdir, bit üzerinden hesaplanır. TFT kalitesine bağlı olan bu değer, her bir pikselin ne kadar yumuşak tonlamalar yapabileceğini gösterir. TFT ne kadar kaliteli ise o kadar hassas voltajlama yaparak o kadar çok ton gösterir. FRC (Frame Rate Control) denen teknoloji ile ucuza renk derinliği sahte olarak arttırılabilir. Düşük renk derinliğinde bantlanma dediğimiz sorun olur.

**6-bit paneller:** Alt piksel başına 64 kanal ton gösterebilir ama artık günümüzde ultra ucuz TN'ler harici kalmamıştır; olan panellerde ise en azından FRC vardır. Bir alt piksel 0 seviyesinden 63 seviyesine kadar çıkabilir, toplam 18 kanal renk sunar (6+6+6). Bu da ekranın 262.144 adet ton üretebildiğini gösterir, bantlanma sorunu olur.

**8-bit paneller:** Alt piksel başına 256 kanal ton gösterebilir; günümüzün standardı ve en yaygınıdır. Üst düzeylerde 8-bit+FRC ile 10-bit taklidi de olur. Alt piksel 0 seviyesinden 255 seviyesine kadar çıkabilir, toplam 24 kanal renk sunar. Bu da bize 16.777.216 ton demektir, bantlanma biraz olur.

**10-bit ve 12-bit paneller:** Pahalı olduğu için pek görmeyiz. 10-bit paneller alt piksel başına 1024, 12-bit paneller 4096 kanal ton gösterir; yani alt pikseller 10-bit için 0'dan 1023'e, 12-bit için 0'dan 4095'e kadar çıkabilir. Toplamda 30 kanal ve 36 kanal renk sunarlar. 10-bit paneller 1.073.741.824 ton, 12-bit paneller 68.719.476.736 ton sunar. 10-bit'te banding oluşmaz, 12-bitte mümkün değildir. İnsan gözüne en yakın 10-bit panellerdir ama fark edilmesi yine de çok zordur.

Renk derinliği arttıkça HDMI/DP/eDP bant genişliğini oldukça doldurur, maliyeti yüksektir.

Her zaman geniş renk gamutu iyi bir şey değildir. Çoğu oyun, web sitesi ve video %100 sRGB'ye göre yapıldığı için renkler biraz fazla canlı ve doğallıktan uzak olabilir; buna oversaturating denir (gereksiz doygunluk). Ten rengi yerine kırmızıya kayması, çimlerin yeşil yerine fosfor yeşili olması gibi. Çoğu zaman sorun olmaz ama renk yönetimi kötü uygulamalarda göze çarpabilir.

### FRC

Bu teknoloji 6-bit veya genelde 8-bit panellerde kullanılır. Yazılımsal sahtekarlık ile 2-bit daha fazla kanal eklenir; bunun için piksel iki ton arasında inanılmaz hızlı titreşir ve beynimizi kandırır. Tonlar neredeyse düzgün olsa da gerçek haz olmaz; dikkatli bakarsanız kumlanma etkisi olurken flicker yaydığı için gözleri özellikle düşük ışıkta yorar.

## 8) Parlaklık

Ekranın ne kadar ışık üretebildiğidir, bizzat arka ışık sorumludur. Ne kadar güçlü arka ışık = o kadar yüksek parlaklık. Birimi nit veya cd/m²'dir, ikisi eşit birimdir. HDR ile direkt bağlantısı vardır. En parlak paneller mini-LED IPS panellerdir. Genelde en az 300 cd/m² isteriz, ideal parlaklık için 350-400 arası yeterlidir laptop ve monitörlerde. Karşılaştırma için güneş 1.600.000.000 cd/m²'dir :) Parlaklık canlılık ile de dolaylı yoldan bağlantılıdır; parlaklık arttıkça beyin algısı yüzünden canlılık da artar. OLED ekranlarda ise gerçekten canlılık parlaklıkla artar.

### Tepe Parlaklık

Tepe parlaklık ekranın güneşte (telefon için) veya HDR içeriklerde kısa süreli olarak kendi kapasitesinin çok üstüne çıkabilmesidir. Ancak uzun süremez çünkü ısınır. Genelde buna HBM denir (High Brightness Mode). En çok OLED telefonlarda ve mini-LED IPS/VA monitörlerde görürüz.

### Sürdürülebilir Parlaklık

Ekranın manuel modda %100 parlaklıktayken ısınma olmadığı sürece uzun süre koruduğu en fazla parlaklıktır, üstüne çıkamazsınız. Ekran tamamen beyaz yapılarak ölçülür. Pazarlamada etkileyici gözükmesi için tepe parlaklık bol bol şişirilir.

### HDR

HDR, VESA'nın bir standardıdır. Uyumlu videolarda etkileyiciliği arttırmak için ekranın parlaklığını geçici olarak arttırır ve sürükleyicilik yaratır. Bazı sertifikaları vardır (ayrıca VESA, DP standardını bulan şirkettir aynı zamanda). HDR ekranlar genelde sadece OLED veya mini-LED ekranlarda cidden etkileyici olur:

- **DisplayHDR 400:** En az 400 cd/m² ekranlar alabilir. Pek bir etkisi olmaz, pazarlama gazının ta kendisidir, Ahmet'tir.
- **DisplayHDR 500:** En az 500 cd/m² ekranlar alabilir. HDR 400'ün gereksiz kardeşidir, tam bir Mehmet'tir.
- **DisplayHDR 600:** En az 600 cd/m² ekranlar alabilir. Etkisi yavaş yavaş hissedilir ama yine de pek etki etmez.
- **DisplayHDR 1000:** En az 1000 cd/m² ekranlar alabilir. Gerçek HDR deneyimi burada başlar, çoğu amiral gemisi telefonda bu vardır, kaliteli mini-LED monitörlerde de bulunur.
- **HDR 1000+/1400:** 1000 cd/m² üstü ekranlar alır, zirve noktasıdır. Her babayiğidin harcı değildir ama azalan getiri olur. HDR 1000 yeterli iken 1400 gereksiz ama iyi seviyesindedir.
- **HDR Ready:** Panelin HDR ile alakası yoktur, sadece HDR sinyalini alabilir ama panel işleyemez demektir. Pazarlama gazının kralıdır. HDR Ready yazan monitörlerden pek bir tat alamazsınız HDR açısından çünkü HDR yoktur; bu monitörlere itibar etmeyiniz.

## 9) Kontrast

Kontrast en parlak beyaz ile en karanlık siyah arasındaki potansiyel farktır. Ne kadar yüksekse beyazlar o kadar canlı, siyahlar o kadar derin ve karanlık olur. Düşük kontrastlı ekranlarda siyahlar çamaşır suyuyla yıkanmış ve gri gibi gözükür. İki türü vardır: Biri gerçek kontrast (statik), diğeri ise panelin türüne göre kolpa kontrast (dinamik).

### Statik Kontrast

Az önce anlattığımız gibi gerçek kontrasttır. En beyaz ile en siyah arasındaki potansiyel farktır. Mesela 1000:1 kontrast, en karanlık siyahın en aydınlık beyazdan 1000 kat daha karanlık olması demektir. Düşük kontrast sadece siyahları çamaşır suyu gibi yıkanmış göstermez, daha da kötüsü siyah sahnelerde tüm atmosferi ve heyecanı bozar; çünkü renkler iyi olsa bile kontrast kötü olduğu için birbirine bulanır ekran.

### Dinamik Kontrast

Siyah olması gereken yerlerde monitör algoritması bakar ve "bu siyah olması gerek" der, ardından oradaki WLED'i kapatır. Ancak mini-LED gibi binlerce LED yerine normal ekranda birkaç on/yüz LED olur. Bu yüzden hassas kontrastlama (dimming) yapılamaz, Halo etkisi çok belirgindir ve pazarlamada bolca şişirilen bir maddedir. Yeni monitör alınca ilk işiniz OSD'den bunu kapatmak olsun. Özellikle TV'lerde çok kullanılır bu taktik.

LCD'de parlaklık düştükçe kontrast düşer; çünkü siyah seviyesi aynı kalsa da beyaz seviyesi düşer ve potansiyel fark azalır.

## 10) Piksel Yoğunluğu ve Izgara Etkisi

Ekranın genel keskinliğini belirleyen şey piksel yoğunluğudur ama "piksel yoğunluğu yüksek = kesinlikle keskin ekran" diye bir tez yoktur; burada panelin kalitesi ve ızgara inceliği de önemlidir.

Piksel yoğunluğu keskinlikte birinci baktığımız değerdir, birimi PPI'dır. Çözünürlük ve ekran boyutuna bağlıdır, bu ikisi ters orantılıdır. Çözünürlük düşüp ekran boyutu da düşerse PPI aynı kalabilir; çözünürlük yükselip ekran boyutu da aynı oranda büyürse PPI yine aynı kalır. PPI 1" alana kaç piksel sığdığını gösterir. PPI ne kadar yüksekse pikseller küçülür ve keskinleşir. Görüntü ekrana ne kadar yaklaşırsanız o kadar yüksek PPI gerekir, ne kadar uzaklaşırsanız o kadar etkisi azalır.

### Izgara (Grid)

Direkt renk filtresi kalitesine bağlıdır. Ne kadar kaliteli ve sıkı bir renk filtresi varsa Grid etkisi o kadar azdır. Mesela direkt evimden gözlemledim: 55" 4K bir TV'm var ancak laptopumun ekranı kırılınca kullanmak zorunda kaldım. Laptopum da 4K'yı desteklemediği için 1080p'de kullanmak zorunda kaldım. 55" 1080p bir TV'nin PPI'ı ~40 PPI'dır. Bazen ara sıra kullandığım 32" 1080p bir TV'm daha var, ona da bir gün bağladım laptopumu ve ~69 PPI olmasına rağmen görüntü çok fazla tırmalayıcı ve kötüydü; çünkü 32" TV'min kalitesi çok kötüydü ve pikseller arası dev ızgaralar vardı. Ama 55" 1080p TV'm ~40 PPI olmasına rağmen görece daha kaliteli olduğu için pikseller arası ızgaraları yoktu ve kabul edilebilir bir keskinlik sunuyordu. O yüzden almadan önce panelin kalitesine ve ızgara kalınlığına da bakın. Düşük PPI ve kalın ızgara hem gözü aşırı yorar hem de kötü ve tırmalayıcı bir görüntü oluşturur.

## 11) Tepki Süresi

Tepki süresi denilen şey temelde bir pikselin bir renkten bir renge geçiş süresidir. Sıvı kristalin hareket etmesi gereken yol ne kadar uzun olursa o kadar yüksek olur. Gitmesi gereken yol arasındaki ilişkiyi yukarıda yazdık ama hatırlatalım:

**Gidilmesi gereken yol:** VA > IPS > TN

Ne kadar hızlı tepki süresi, o kadar net iz bırakmayan sahneler. İki türe ayrılır:

### GtG (Gray-to-Gray)

En yaygın kullanılan ölçüdür, pikselin gri tondan gri tona gidişini temsil eder.

Neden griden griye? Çoğu piksel aslında siyah veya beyaz yerine ara tonlarda gider, ölçmek için en uygun ara ton da gridir.

Aslında GtG'nin kesin bir ölçüm yöntemi yoktur; üreticiler biraz şişirme, biraz sallama, biraz hesap ve biraz da tahmin ile bir şeyler söyler.

- TN paneller genelde gerçek 1ms.
- IPS paneller 1ms (çok zordur aslında) - 4ms arası.
- VA'da 4ms - 8ms arasıdır (yine de iz bırakabilir).

GtG'nin standardı yoktur, üretici ne dediyse güvenmek zorundayız.

### MPRT

Moving Picture Response Time demektir. İnsan gözünün algıladığı bulanıklığı ölçen bir birimdir, yani "bir piksel kaç ms görünür kalır?" sorusunun cevabıdır.

Düşük MPRT = daha az bulanıklık = daha net görüntü.

MPRT'yi düşürmek için BFI denen bir teknoloji kullanılır; yani aralara siyah kare ekleyerek düşürmeye çalışmak. Bazı Sync teknolojileri bunları kullanır (DyAc, ULMB, ELMB).

### VA Smearing

Ghosting'in VA sürümüdür ama daha çok karanlık sahnelere özgüdür. Koyu ve siyah nesneler hareket ederken sanki arkasında kuyruklu yıldız gibi iz bırakır. Bunun en kronik versiyonu Samsung Odyssey G3 monitörde yaşanıyor.

Çünkü VA kristallerinin gideceği yol oldukça uzundur. VA paneller siyahtan griye geçerken dik konumdan hafif yatık konuma geçmesi gerekir ancak bunu pek de hızlı yapamazlar; bu yüzden bu problem ortaya çıkar. Ghosting silik bir izken smearing daha problemli ve siyah kuyruklu yıldız gibidir.

Rapid VA paneller bunu büyük oranda yüksek voltaj vererek çözmüştür.

### Ghosting

Hayaletlenmedir, daha çok IPS'lere özgüdür. Günümüzdeki Fast IPS paneller ile çözülmüştür. Herhangi bir hareketli nesnenin arkasında objenin silik bir kopyasının belirmesidir. Pikselin eski rengi silip yeni renge hızlıca geçememesinden oluşur, böylece bu iz olur.

### Inverse Ghosting

Ghosting'in tam tersidir. Hareketli nesnenin olması gerekenden daha parlak ve beyazımsı veya renkli bir iz bırakmasıdır. OverDrive ayarı çok agresif olursa bu sefer piksel gereğinden fazla hızlanır ve ortaya bu sorun çıkar, olması gereken renk seviyesi aşılır. Buna overshooting denir. Mesela siyahtan griye geçmesi gereken piksel yüksek voltaj yüzünden hemen gri veya beyazımsı olur, sonra bir anda dönüp tekrar gri olur; çok hızlı değişim ekranda iz bırakır.

OverDrive seviyesini ortalama değere getirmek çözer.

### OverDrive

Sıvı kristale gereğinden fazla voltaj uygulayarak pikselin daha hızlı hareket etmesi ve daha hızlı tepki vermesi için yapılır. Yüksek Hz için daha yüksek OverDrive değeri gerekir. Düşük Hz'lerde çok fazla OverDrive uygulamak çılgın inverse ghosting yapabilir; tam ortası deneme yanılma ile bulunur.

## 12) Yenileme Hızı

TFT tabakanın bir piksele saniyede kaç kez yenilenmesi gerektiğini söylemesidir. 60Hz olan ekranda TFT piksele saniyede 60 kere "renk değiş", 120Hz ve ötesinde ise TFT tabaka piksele 120 veya daha ötesi kadar "renk değiş" der. Renk değişimi daha hızlı olunca görüntü daha akıcı gelir. 240Hz üstü pek hissedilmez, 120Hz en iyi noktadır; çünkü hem yeterli akıcılık verir hem de güç tüketimi azalır. Güç tüketimini etkileyen en önemli şeylerden biridir.

Eğer piksel yenileme hızından daha geç tepki süresine sahipse ghosting oluşur.

Yenileme hızı ve kareler arası süre: Kareler arası süre panelin tepki süresinden (GtG) çok olmalıdır, yani GtG kareler arası süreden az olmalıdır.

- 60Hz = 16.7ms
- 120Hz = 8.3ms
- 144Hz = 6.9ms
- 240Hz = 4.2ms
- 360Hz = 2.8ms
- 480Hz = 2ms

Yenileme hızı arttıkça diminishing returns yani azalan getiri yasasına çarpar, fark azalır.

### VRR

Variable Refresh Rate yani değişken yenileme hızı demektir. Yenileme hızı FPS ile aynı olursa ekran yırtılması dediğimiz şey olmaz; yani FPS, yenileme hızı ile eşitlenir.

2 genel standardı ve diğer açık standartları vardır:

- **NVIDIA G-Sync:** Sadece NVIDIA kartlarla çalışan, ücretli ve kapalı kaynak bir standarttır. Monitör üreticileri G-Sync'i koymak için bir lisans ücreti ödemek zorundadır, bu yüzden sadece pahalı ve üst seviye monitörlerde bulunur.
- **AMD FreeSync:** Sadece AMD kartla çalışan, ücretsiz ve açık kaynak bir standarttır. Bedava olduğu için neredeyse her monitörde ve gelişmiş TV'lerde bile bulunur.

Ayrıca VRR'nin çalışma aralığı 48Hz'den XXX Hz'e kadardır. 48Hz'in altına düştüğünde VRR devre dışı kalır ve yırtılma geri başlar. Burada LFC (Low Frame Rate Compensation) denen bir teknoloji devreye girer ve kareyi katlayıp yapay olarak sahte kareler ile 2'ye katlar ve akıcılığı geri getirir. VRR'nin çalışması için gerçek yenileme hızının 96Hz'den fazla olması gerekir.

## 13) PWM ve DC Dimming

Daha çok OLED'e özgü bir durum olsa da LCD'de de kullanılır. Parlaklık kısılırken kullanılan 2 teknolojiden biridir.

### DC Dimming

Parlaklık kısmak için arka ışıkların voltajı düşürülerek parlaklık düşürülmüş olur. Titreşim yapmaz, göz sağlığına zararı olmaz. Düşük parlaklıkta uzun süreli kullanım için idealdir ama dediğim gibi parlaklık düştükçe renk canlılığı ve doğruluğu kayar.

### PWM Dimming

Ekran parlaklığı çok kısa sürelerle açık bırakılıp tekrardan çok hızlı kapatılır. Saniyede kaç kez aç-kapa döngüsü olduğunu PWM dimming Hz'i söyler. Gözlerimiz bu aç-kapayı anlayamaz ve tek bir parlaklıkmış gibi algılar. Düşük parlaklıkta devreye girer (genelde %45/%40 altında). Ama düşük Hz'leri gözler anlamasa da beynimiz ve sinirler anlar, bu yüzden baş ağrısı yapabilir. En az 1000Hz önerilir; renkler kaymaz ve doğruluk azalmaz ancak düşük Hz ise baş ağrıtır.

## 14) Renk Kalibrasyonu ve Delta E

Ekranda canlılık ve renklerin ne kadar patladığına baksak da profesyonel dünyada önemli olan renklerin ne kadar doğru, hatasız ve uygun olduğudur. Burada kalibrasyon ve Delta E değeri işimize yarar.

Renk kalibrasyonu 2 şekilde olur:

- **Fabrika kalibrasyonu:** Üst seviye profesyonel monitörler (EIZO, Dell UltraSharp, ASUS ProArt gibiler) fabrikada profesyonel bir şekilde kalibre edilir ve fabrikadan öyle çıkar.
- **Kullanıcı kalibrasyonu:** Bir kolorimetre ile monitör kalibre edilir ve renkler doğrulanır, kullanıcı kendi yapar.

Delta E değeri ise bir rengin olması gereken hali ile ekrandaki hali arasındaki farktır. Ne kadar düşük değer, o kadar doğru renkler demektir.

- Delta E < 1: Mükemmel ötesi, ultra profesyonel monitörler buna yakın olur.
- Delta E < 2: Muhteşem, sadece ultra keskin ve mesleki deformasyona uğramışlar fark edebilir farkı.
- Delta E < 3: Çok iyi, genel kullanıcı için yeterlidir.
- Delta E < 4: Sapma yavaş yavaş hafif fark edilebilir, iyi-orta.
- Delta E < 5+: Renkler sapmıştır, kalibrasyon şart.

Kalibrasyon hem renkleri doğrulaştırır hem de şu değerleri doğal değerine getirir:

- Beyazları gerçekten beyaz gibi yapar, sarıya kaymış olmazlar.
- Gamayı düzgün bir değere getirir ve orta tonların parlaklık eğrisi doğrulaşır, genelde 2.2 olur.
- Renk sıcaklığı 6500K yakınına döner, böylece ne sıcak ne de soğuk olur.

Genelde ev kullanıcısı için kalibrasyona gerek yoktur çünkü kalibrasyon cihazları epey pahalıdır. İllaki kalibrasyon cihazına gerek yoktur, göz ile de renk dengeleri ile oynanarak körlemesine kalibrasyon yapılabilir. Zamanla arka ışık yaşlanınca renk sıcaklığı değişse ve kalibrasyon gerekse de bunun için 5+ yıl gereklidir. Profesyonel işlerde en az yılda bir kalibrasyona ihtiyaç vardır.

## 15) Veda

Bu rehberde amacımız bilene de bilmeyene de bu işin inceliklerini anlatabilmekti ve umarım yapabilmişimdir. Bu rehberi bir insan yazdı, yani illaki küçük hatalar ve yanlışlar olacaktır/olabilir; affeyleyin forumdaşlar, hatasız kul olmaz, olmadı da. Umarım herkese hitap edecek, sıkmayacak ve akıcı bir rehber olmuştur. Okuduğunuz için çok teşekkür ederim, herkese iyi günler ve kazasız belasız yaşamlar. 💜
