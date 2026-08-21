---
layout: default
title: "IJP OLED Rehberi: Üretim Teknolojisi ve Geleceği"
date: 2026-08-21
categories: [Paneller, OLED]
---

# IJP OLED Rehberi

Selamlar, bugün OLED için belki devrim olabilecek ve OLED'in geleceğini tayin edebilecek bir teknolojiden kısaca bahsedeceğiz. CSOT'un (TCL yan kuruluşu) gen 8.6 IJP OLED fabrikasını açması ile tost basar gibi üretim yapması tabii ki de dikkat çekti. Bu ilk revizyondan MSI ise nasibini aldı ve (Türkiye hariç) ilk IJP OLED monitörlerini çıkardı. Bugün bu konumuzda IJP OLED'e değineceğiz ve bunun ne olduğunu anlatacağız.

## IJP OLED nedir?

IJP OLED, bir panel teknolojisinden çok OLED'in kronik üretim sorunlarını ve verimsizliğini çözmek için çıkmış bir üretim teknolojisidir. Bu teknolojide OLED klasik VTE üretim tarzı yerine inkjet printing yani mürekkep püskürtmeli baskı ile üretim yapılır. Böylece bir baskı makinesine OLED hammaddesi yüklenir ve baskı makinesi tek alt piksellere mürekkebi basar. Bu yüzden de hiç madde israfı olmaz. OLED'in alt piksellerini oluşturan organik madde çok pahalıdır ve VTE üretimde %70'e yakını israf olur. IJP'de ise %100'e yakını israf olmadan kullanılır. Ayrıca pahalı vakum odaları ve çok pahalı olan hizalama maskesi (fine metal mask, FMM) gerektirmediği için çok daha ucuzdur.

## Nasıl çalışır?

Aslında temel mantık evdeki bildiğimiz yazıcılar gibi çalışır ama bu milimetrik mikron hassasiyetinde yapılır. Bir ultra hassas uçlu mürekkep püskürtme makinesine organik madde yüklenir ve makine bunu OLED'deki boşluklara çok hızlı basmaya başlar. Gelişmiş makineler saniyede 30.000 piksel basabilir.

## Üretim

Önce normal OLED'de olduğu gibi cam ve esnek bir tabaka alınır. Bu tabakaya pikselleri kontrol edecek ince film transistör (TFT) katmanı işlenir.

Mürekkebin doğru yerde durması için TFT tabakaya "bank" dediğimiz mikroskobik setler örülür.

IJP makinesi gelir ve nozzle'ı (başlık) istenilen piksel boyutu için takılır (yüksek PPI için daha ince, düşük PPI için daha kalın başlıklar).

IJP makinesi bir oda boyutundadır. Makineye özel solvent içinde çözülmüş organik madde doldurulur.

Makine başlar ve inanılmaz bir hızla ve hiçbir madde israf etmeden mürekkebi tek tek pentile (RGBG) veya RGB şeklinde dizerek fışkırtır.

Doldurulan panel fırına yollanır ve mürekkep kurutulur. Kuruyan mürekkep ince, pürüzsüz ve homojenik bir film halini alır. İşte bu katmanda OLED'dir.

En son olarak panelin üstüne katot elektrot filmi eklenir, oksijen ve nemden korumak için kapsüllenir.

## Faydaları nedir?

En büyük faydası büyük ekranlar içindir. VTE üretim yöntemi büyük ekranlarda mümkün değildir (buharlaşma sorunları). IJP ile 115" ve ötesine kadar her türlü panel doldurulabilir ve üretilebilir.

Çıkan paneller gerçek OLED'dir. Günümüzde büyük ekranlarda OLED üretmek maliyetli ve zordur. Bu yüzden WOLED veya QD-OLED kullanmak zorunda kalırız. Bunların da kendine has problemleri mevcuttur. IJP OLED yönteminde ise gerçek pentile (RGBG) veya RGB OLED basılabilir.

- Organik madde israfı neredeyse olmaz.
- Dev vakum odalarına veya vakum pompalarına gerek kalmaz.
- Pahalı ve sürekli kirlenen FMM maskesine gerek kalmaz.
- Üretim maliyetini ciddi şekilde düşürür.

Ama kendine ait sorunları da vardır.

## Sorunlar

- Mürekkebin, "mürekkep olabilmesi için" solvent içinde çözünmesi gerekir. Bu solvent pikselin ömrünü azaltır. Bu yüzden özel organik maddeler geliştiriliyor. Ayrıca daha kısa ömürlü oldukları için yüksek parlaklıklara çıkmaları daha zordur.

- Mürekkep homojen dağılamaz. Bu yüzden "kahve lekesi etkisi" denen bir soruna neden olur. Mürekkep kenarlarda birikip merkezde incelebilir. Bu da piksellerin eşit homojenlikte olmamasına ve parlaklık farklılığı sorununa neden olabilir. Bu sorun için de özel organik maddeler geliştiriliyor.

- Yüksek PPI veya keskinliklerde uygun değildir. Belli bir PPI üzerinde VTE kullanılmalıdır.

- Yatırım maliyeti şu anlık yüksektir. Fabrika kurmakta zordur. Daha emekleme aşamasında fabrikalar kendini amorti edene kadar zaman geçmesi gerekir.

- Zamanla nozzle tıkanır ve temizlenmesi gerekir.

- IJP'ye özel organik madde üretimi az ve zordur.

## Sonuç

IJP OLED'in öncülerinden CSOT seri üretime yeni başladı. MSI ilk partiden monitör üretmeye başladı. Sorunları ve avantajlarını yakında göreceğiz. Ayrıca geçen seneye kıyasla OLED pazarı %23.6 büyüdüğü için şu an yükseliyor. IJP OLED pazara tamamen hakim olduğunda (2027 sonuna doğru) OLED fiyatları feci şekilde düşecektir. Ancak hala önümüzde aşmamız gereken sorunlar mevcut.

Okuduğunuz için teşekkür ederim. 💜
