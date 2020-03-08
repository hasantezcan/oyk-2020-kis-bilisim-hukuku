#### `Özgür Yazılım Kış Kampı '20`

### `Bilişim Hukuku - GÜN 2 - 2020.01.26`

---

## RFC - Requests for comment
> [**wikipedia.org/Request_for_Comments**](https://en.wikipedia.org/wiki/Request_for_Comments)
> [**What Is Internet Request for Comments (RFC)?**](https://www.lifewire.com/what-is-internet-request-for-comments-rfc-4092366)

RFC belgeleri, İnternet topluluğu tarafından yeni standartları tanımlamak ve teknik bilgileri paylaşmak için 40 yılı aşkın bir süredir kullanılmaktadır.

Üniversitelerden ve şirketlerden araştırmacılar, internet teknolojileri hakkında en iyi uygulamaları sunmak ve geri bildirim almak için bu belgeleri yayınlamaktadır.

RFC'ler bugün [**IETF**](https://www.ietf.org/) adı verilen dünya çapında bir kuruluş tarafından yönetilmektedir.

### RFC'lerin Tarihçesi
RFC 1 dahil olmak üzere ilk RFC'ler 1969'da yayınlandı.

RFC 1 de tartışılan **"host software"** teknolojisi günümüzde kullanılmıyor olsa da RFC belgeleri arasında halen durması bilgisayar ağlarının ilk günlerine ilginç bir bakış sunar.

Bugün bile, RFC'nin düz metin biçimi başlangıçtan beri olduğu gibi kalmaktadır.

<p align="center">
	<img alt="rfc2460" src="/images/day2/rfc.png" width="800">
</p>

> #### [**`rfc2460`**](https://tools.ietf.org/html/rfc2460), [**`rfc8200`**](https://tools.ietf.org/html/rfc8200)
- daha okunur bir alternatifi [`rfc-editor.org/info/rfc8200`](https://www.rfc-editor.org/info/rfc8200)

---
## Shannan - Information Theory
> [**wikipedia/information_theory**](https://en.wikipedia.org/wiki/Entropy_(information_theory))

- [**Information and Entropy** - *MIT Course 2008*](https://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-050j-information-and-entropy-spring-2008/#)

- [**Information and Entropy** [Türkçe] - Yaşar Safkan](https://www.youtube.com/watch?v=TYqtEelODkQ&list=PL8bY8chu6YPrb_MNULaBId1jnrw5R4a68)

- [**What is entropy?** - *Jeff Phillips*](https://www.youtube.com/watch?v=YM-uykVfq_E)

- [**Information entropy** | *Journey into information theory*](https://www.youtube.com/watch?v=2s3aJfRr9gE)	 	

- **Entropi kavramı** - *Lise müfredatı* [**[0]**](https://www.youtube.com/watch?v=ZsY4WcQOrfk), [**[1]**](https://www.youtube.com/watch?v=Ah2NqzT99JE)

***Information nasıl ölçülür?***
- Bit ile.
	- Peki, Bit Nedir?

	..
	..
	..

---

## Encoding, Encryption, Compression

#### 1- Encoding
`veri boyutu büyür.`
- veri değişmiyor

#### 2- Encryption
`veri boyutu aynı kalır.`
- veri değişmiyor

#### 3- Compression
`veri boyutu küçüklür.`
> [https://www.makeuseof.com/tag/how-does-file-compression-work/](https://www.makeuseof.com/tag/how-does-file-compression-work/)

1. **Kayıplı sıkıştırma *(Lossy Compression)***
> [wikipedia.org/Lossy_compression](https://en.wikipedia.org/wiki/Lossy_compression)

	En yüksek seviyede sıkıştırma işleminin gerçekleştirilebilmesi için verinin bir kısmından fedakarlık edilerek gerçekleştirilen sıkıştırılma işlemidir. Kayıplı sıkıştırma işlemi sıklıkla grafik ve ses dosyalarının boyutunu düşürmek için kullanılan bir yöntemdir. Örn: *mp3, jpeg, png*

  #### `veri kaybı olur.`

	***Hukuki açıdan bakıldığında;***
	#### Kayıplı sıkıştırma veri ile oynanmış demek değil midir?

	Evet. Görüntü, kayıplı sıkıştırıldığı için veri kaybı söz konusu olur. Bu da eksik veri ile karar alma durmu yaratır. Bu sebeplerden ham veri mevcutsa o veri ile değerlendirme yapamak daha doğru sonuç verecektir.

2. **Kaypısız sıkıştırma**
>[wikipedia.org/Lossy_compression](https://en.wikipedia.org/wiki/Lossy_compression)

	Dosyanın kalite kaybı olmadan sıkıştırılması ve ayıklandığında tekrardan çalışabilir hale getirilebilmesi işlemidir.

  #### `veri kaybı olmaz.`

---

#### **Encoding ile Encryption arasındaki fark nedir?**
Base 64 bir şifreleme değildir. Bir kodlama yöntemidir.

CTF yarışmalarında bunu şifreleme soruları olarak sorarlar.

..
..
..
..


#### Önce sıkıştırıp sonra şifrelemek mi? Önce şifrelemek sonra sıkıştırmak mı?

Önce sıkıştırcaz sonra şifreliycez.

Sıkıştırma direk olarak örüntüler ile ilgilenir. Amacı örüntüleri değerlendirip bunlardan faydalanarak en optimal düzeni oluşturmaktır. Ardından asimetri ile yani düzensizlik ile beslenen Encoding'e başvururuz. Şifrelerken zaten amaç tüm örüntüyü bozmaktır. Şifrelemekte amaç geriye örüntü bırakmamaktır.

Bu sebeple önce sıkıştırıp sonra şifrelemek daha verimlidir.

---

### `- MD5: b8e20611dcc4105286bcf56de754f7a3`

### `- SHA1: 9f34ac74f28e6ee9f0ad76d7b39d615722822b4f`

#### Bu ifadeler nedir?
- Bu ifadeler birer hexadecimal sayıdır.

## Hash Nedir?
> [**wikipedia.org/Cryptographic_hash_function**](https://en.wikipedia.org/wiki/Cryptographic_hash_function)
> [**gokhansengun/kriptografik_hash_fonksiyonu_nedir**](https://medium.com/@gokhansengun/kriptografik-hash-fonksiyonu-nedir-ve-hangi-ama%C3%A7larla-kullan%C4%B1l%C4%B1r-94bdee56fa93)

**md5**, **sha1** bunlar şifreleme algoritması değildir. Bu adlandırma yanlıştır.

**Kriptografik Hash fonksiyonları** aldıkları girdinin boyutundan bağımsız olarak belirli (örneğin 20 bayt) uzunluğa sahip bir çıktı üretirler. Üretilen çıktı verilen girdiye özeldir. Aynı girdi ile sürekli aynı çıktı oluşur ve iki farklı girdinin çıktısı ile birbiriyle aynı olamaz.(Collision olmaması durumunda)

Hashleri anlamadan önce fonksiyonları anlamak gerekir.

> **Temel fonksiyon bilgisi** - [**[0]**](https://www.khanacademy.org/math/algebra/x2f8bb11595b61c86:functions/x2f8bb11595b61c86:evaluating-functions/v/what-is-a-function), [**[1]**](https://www.matematikkolay.net/konu-anlatimi/fonksiyon)

Hash fonksiyonları da birer fonksiyondur. Ve onları bu şekilde düşünmek bazı yanlış düşünceleri aklıcı şekilde uzaklaştıracaktır.

Fonkisiyonlar bize belli sayıda çıktı verirler. Bazı fonkiyonlar bir adet çıktı verir. Siz girdi olarak ne veriseniz verin size vereceği çıktı sabittir. Bu fonskiyonlara **sabit fonksiyon** adını veririz.

<p align="center">
<img alt="rfunction-x" src="/images/day2/function-x.png" width="350">
</p>

<p align="center">
<img alt="rfunction-x-exp" src="/images/day2/function-x-exp.png" width="300">
</p>

- **f(x) fonksiyonunun** girdi sayısı sınırsız çıktı sayısı bir adetir.
- **md5 fonkisiyonun** girdi sayısı sınırsız çıktı sayısı 2^128 tanedir. **Çıktı sayısı sınırsız değildir.**

#### Gelin şimdi **”Collision”** kavramını irdeleyelim..

Aynı çıktıyı oluşturan iki farklı girdi **”Collision”** bulunduğu anda Hash fonksiyonu “kırılmış”tır ve kriptografik olarak güçlü değildir. SHA-1 için 2017'de 6610 yıl işlemci zamanı kullanılarak bir “Collusion” tespit edilmiştir, MD5'ta ise 2005'ten beri “Collusion”’lar vardır. Tespit edilen “Collusion”’lardan dolayı MD5 ve SHA-1 Hash fonksiyonları günümüzde kriptografik olarak yeterince güçlü kabul edilmemektedir.

Yani hash fonksiyonlarında birebirlik esastır. Bu sağladığı sürece sıkıntı yoktur. Fakat bunun bozulması beraberinde collisionu da dağrumuş olur.

##### `Yani hash fonskiyonları ebedi değildirler. Doğarlar, yaşarlar ve ölürler.`

### [`We're doing math here, not magic!` ](https://www.linkedin.com/pulse/were-doing-math-here-magic-eng%C3%BCr-r%C4%B1za-pi%CC%87%C5%9Fi%CC%87ri%CC%87ci%CC%87/)

---

[**adlibilisimuzmani.com**](https://www.adlibilisimuzmani.com/adli-bilisim-kavramlari/)

bu sitede bulunan hash ile ilgili tanım yanlışıtır.

`Hash değeri, hash’i hesaplanan veriye özel ve parmak izi gibi benzersiz bir değerdir.`

Bu ifade yanlıştır. Çünkü her fonskiyonun belirli bir çıktı değeri vardır ve **"hesaplanan veriye"** yani girdiye eşsiz sonuç çıkaratamayabilir. Bknz [**Collision**](#)

### `Yetkinliğinden emin olmadığınız bilgileri sırtlanmayınız.`

---

Tabiki hash fonksiyonlarını kullanırken mutlak güven içinde olmayız. Kullandığımız hash fonksiyonunun collision'a uğrama ihtimalini hep var sayarız. **Taviz veririz.**

Tabiki collision tespti yapılmış hash fonskiyonlarını da kullan**mamak** gerekir. Bu fonksiyonlar artık zafiyetlidir ve güvenli sayılmazlar.

Fakat günümüzde bu collisionlardan bihaber birçok kullancı mevcuttur. Hayatın olağan akışı içinde farkına varmamış olabilir ve artık güvenli sayılmayan bir hash fonskiyonunu kullanıyor olabiriz. Kendimizi bu durumda bulammak için bu fonksiyonların güveniriliğini takip etmemiz gerekir.

> hash fonksiyonları ile ilgili haberleri buradan takip edebilirsiniz: [**src.nist.gov/hash-functions/news**](https://csrc.nist.gov/Projects/Hash-Functions/news)

Bu arada bir hash fonksiyonun collisionu çıkmamış görünebilir. Fakat kimileri bu açığı çoktan bulmuş ve kimseye açık etmeden kötüye kullanıyor olabilir. Zaten bir collision tespit edildikten sonra birden fazla firma peş peşe bunu nasıl tespit etiklerini anlatan duyurular yaparlar. Bu durum bize burada bir bit yeniği olduğunu gösterebilir.

Bugün adliyeden bir dosya kopyası aldığımızda bu dosyanın doğruluğunu adliyeler **md5 hash fonskiyonu** ile kontrol etmektedirler. Md5 2005'te collision'a uğramış olmasına rağmen adliyelerin hala bu hash fonksiyonunu kullanıyor olmaları dosyaların birebirliğini ölçmede güvenili bir yöntem kullanmadıklarını gösterir.

> İlgilisine başlık;
	- [**what-are-bitcoin-hash-functions?**](https://newscryptonews.com/bitcoin/what-are-bitcoin-hash-functions/)

## Elektronik İmza
> [**btk.gov.tr/elektronik-imza-mevzuati**](https://www.btk.gov.tr/elektronik-imza-mevzuati)

[**5070 sayılı kanuna**](https://mevzuat.gov.tr/MevzuatMetin/1.5.5070.pdf) göre Elektronik İmza elle atılan imza ile eş değer olarak kabul edilmiştir. E-imza şeklinde de anılan bu kavram bilgisayar ortamındaki imza olarak tanımlanmaktadır. E-devlet projesi kapsamında bir çok projede kullanılması zorunlu olması ile birlikte iş ve işlemlerin daha hızlı ve kolay bir şekilde yapılmasına da olanak sağlamaktadır

<p align="center">
	<img alt="e-imza" src="/images/day2/e-imza.jpg" width="450">
	<br>
	<em> elektronik imza </em>
</p>

E-imza çalışma şekli ise; bilgisayara usb olarak bağlanan ve fiziksel yapısı flashdisk şeklinde olup buna akıllı kart veya token denilmektedir. Token içerisinde kişiye özgü bilgilerin bulunduğu şifrelenmiş bir sertifika bulunmaktadır.

> [**Elektronik imza temin etmek için..**](https://eimza.gen.tr/)

Elektronik imza kullanımıda esas olan iki öge vardır. Bunlar;
- E-imza çubuğu
- E-imza pin'i

Elektronik imza pinlerinin sadece ait olduğu vatandaş tarafından bildindiği varsayılır. Bu sebeple pin'inizi kimseye söylememeniz gerekmektedir.

Fakat buna rağmen gündelik kullanımlarda pek çok kişi hem e-imza cihazlarını hem de e-imza pinlerini başkaları ile paylaşmakta. Fakat bu durum çok büyük risk barındırıyor. Devlet pin'i sadece sizin bildiğinizi kabul ederek. E-imza ile yapılan işlemlerin siz tarafıdan yapıldığını kabul ediyor. Ve yapılan işlemler geri alnamıyor ve bu durumlarda maduriyet oluşma ihtimali hayli fazla.

Bu konu hakkında duyulan bir örenğe göre bir kişi alım satım işlerini idare etsin diye e imza bilgilerini bir katip'e veriyor. Katip de ona verilmiş olan  e-imza bilgilerini kullanarak vatandaşın iki evini satıp kayıplara karışıyor.

---

..
..
..
..
..
..
..
..
..
..
..
..
..
..
..
..
..
..
..
..
..
..
..
..
..
..
..
..
..
..
..
..
..
..
..

..
..
..
..
..
..
..
..
..
..
..
..
..
..
..
..
..
..

---

## Kaynakça
