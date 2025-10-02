# Bölüm 01: Giriş

## 📖 Genel Bakış

Web sitelerinde ve mobil uygulamalarda gördüğünüz reklamlardaki perdenin arkasını kaldırabilseydiniz, sahnelerin arkasında neler olup bittiğine şaşırırdınız. Çevrimiçi reklamcılık ekosistemi; şirketlerden, teknoloji sistemlerinden ve karmaşık teknik süreçlerden oluşur ve tümü birlikte çalışarak internet üzerindeki çevrimiçi kullanıcılara reklam sunar.

Çevrimiçi reklamcılık beraberinde birçok olumlu yön de getirmiştir. Öncelikle, içerik üreticilerine bir gelir kaynağı sağlayarak içeriklerini çevrimiçi kullanıcılara ücretsiz sunmalarına olanak tanımıştır. Ayrıca, mevcut ve yeni medya ile teknoloji şirketlerinin büyümesine ve gelişmesine de katkı sağlamıştır.

Ancak, çevrimiçi reklamcılık sektörü birçok iniş ve çıkış yaşamış olsa da, birçok düşüş de olmuştur. Bazı önemli örnekler arasında 1990'ların sonu / 2000'lerin başındaki dot-com balonunun patlaması, ve daha yakın zamanda gizlilik yasalarının (örneğin GDPR) ve tarayıcılardaki gizlilik ayarlarının (örneğin Safari'nin Intelligent Track Prevention özelliği) yürürlüğe girmesi yer almaktadır. Bu durum reklamverenleri, AdTech şirketlerini ve yayıncıları olumsuz yönde etkilemiştir.

---

## 🤔 Bu Kitabı Neden Yazdık?

12 yılı aşkın süredir reklam ve pazarlama teknolojisi tasarlayıp geliştirirken 2 şey fark ettik:

1. **AdTech'i oluşturan platformlar ve süreçler son derece karmaşıktır.**
2. **Çevrimiçi reklamcılığın hem temel hem de teknik açıdan nasıl çalıştığını kolay anlaşılır ve şeffaf bir şekilde açıklayan çok az kaynak vardır.**

Fark ettik ki aslında başkalarıyla paylaşabileceğimiz adeta bir bilgi hazinesinin üzerinde oturuyorduk.

Ve işte **The AdTech Book** böyle doğdu.

---

## 👥 The AdTech Book Kimin İçin Yazıldı?

**The AdTech Book**, çevrimiçi reklamcılığın tarihini öğrenmek ve dijital reklam teknolojisi ekosisteminin farklı unsurlarının nasıl çalıştığını, rollerinin ne olduğunu ve sektördeki taraflar arasındaki ilişkileri anlamak isteyen herkes için idealdir.

Kitap çok teknik ve detaylı açıklamalar içerse de, biz The AdTech Book'u herkesin okuyup anlayabileceği en basit şekilde yazmaya çalıştık.

### 🎯 Hedef Kitle

Daha spesifik olarak, bu kitap şu kişilere büyük fayda sağlayacaktır:

- **Reklam ve pazarlama şirketlerindeki üst düzey yöneticiler ve kurucular**
- **Reklam verenler ve reklam ajanslarında ya da şirket içinde çalışan pazarlama uzmanları**
- **Reklam ve pazarlama teknolojisi geliştiren teknik ekipler**
- **İçeriklerini reklam yoluyla paraya dönüştüren (veya dönüştürmek isteyen) yayıncılar ve içerik üreticiler**
- **Çevrimiçi reklamcılığın nasıl çalıştığını öğrenmek isteyen düzenli internet kullanıcıları**

---

## 📋 Genel Varsayımlar

Bu kitap, reklamların web sitelerini gelir elde etmek için nasıl kullanıldığını ve ürün/hizmetlerin nasıl tanıtıldığını anladığınızı varsayar. 

Bu kitap, platformların ve süreçlerin nasıl çalıştığı konusunda herhangi bir teknik bilgiye sahip olduğunuzu **varsaymaz**. Ancak böyle bir bilginiz varsa, kitapta yer alan teknik açıklamaları anlamanın çok daha kolay olduğunu göreceksiniz.

---

## 📚 Bu Kitap Nasıl Düzenlendi?

Kitabın ilk birkaç bölümü çevrimiçi reklamcılığın tarihini tanıtarak sonraki bölümler için zemin hazırlar. Dijital reklamcılığın temellerini ele alıyor ve ardından yavaş yavaş platformları, aracılar ile teknik süreçleri tanıtmaya başlıyoruz.

---

## 🔤 Bu Kitapta Kullanılan Kurallar

### **Kalın**

Belirli terimleri vurgular.

> **Örnek:** Marka farkındalığı (diğer adıyla markalaşma): Ana hedef geniş bir tüketici kitlesine ulaşmak, onlarla etkileşim kurmak ve markaya maruz kaldıkları süreyi en üst düzeye çıkarmaktır.

### *İtalik*

Bir cümlenin içindeki belirli bir terimi vurgulamak için kullanılır.

> **Örnek:** Bir *yayıncı*, bir kitleyi çeken içerik üreten herhangi bir şirket olarak tanımlanabilir.

### ***Kalın ve İtalik***

Yeni terimleri belirtir.

> **Örnek:** ***Reklam Teknolojisi*** (Ad Tech, AdTech, adtech, ad tech, ad technology); çevrimiçi medya kampanyalarını oluşturmak, yürütmek, yönetmek, ölçmek ve optimize etmek için kullanılan yazılım ve araçları ifade eder.

### ***İtalik, Altı Çizili ve Kalın***

İleri okumalar için bölümlere atıfta bulunurken kullanılır.

> **Örnek:** Şu bölüme bakın: *The Main Digital Advertising Mediums and Channels* — farklı dijital reklam türleri hakkında daha fazla bilgi için.

---

## 💡 Açık Gri Kutular

Bu kitap boyunca bunun gibi açık gri kutular göreceksiniz. Bu kutuların 2 amacı vardır:

1. Çevresindeki metinde geçen belirli terimleri açıklamak
2. Tartışılan konularla ilgili ilginç bilgiler sunmak

---

## 💻 Kod Örnekleri

Bu kitapta yer alan kod örnekleri yalnızca açıklama amaçlıdır. Aksi belirtilmedikçe kopyalanıp kullanılmak üzere tasarlanmamıştır.

```html
<a href="https://www.advertisers-landing-page.com">
  <img src="http://advertisement1.jpg">
</a>
```

---

## 🎨 Teknik Çizimler, Açıklamalar ve Örnekler

Bu kitap boyunca, bir teknik konuyu (örneğin sunucu taraflı video header bidding süreci) resmettiğimizde, açıkladığımızda veya örnek verdiğimizde, kavramın kafa karışıklığında kaybolmaması için en yaygın ya da en anlaşılır yolu tercih ediyoruz.

Ayrıca, bu kitapta bahsedilen teknik süreçlerin genellikle birden fazla şekilde uygulanabileceğini de belirtmek gerekir.

> *Sunucu taraflı video header bidding'in nasıl çalıştığını gösteren bir illüstrasyon.*

---

## 📝 Kitapta Kullanılan Terminoloji

Bu kitapta, aynı şeyden farklı isimlerle bahsettiğimizi fark edeceksiniz. Örneğin:

> ***Envanter*** (Inventory), diğer adıyla ***reklam alanı*** (ad space) veya ***çevrimiçi medya*** (online media), bir yayıncının sitesinde ya da uygulamasında kullanıma sunduğu alandır.

Bu durum çevrimiçi reklamcılık sektöründe yaygındır, ancak kafa karışıklığını önlemek için kitap boyunca mümkün olduğunca tek bir terim kullanmaya çalışacağız.

**Tek istisna:** ***Çevrimiçi reklamcılık*** (online advertising) ve ***dijital reklamcılık*** (digital advertising) terimleridir. Bu terimler tam anlamıyla eşanlamlı olmasa da, kitap boyunca çok sınırlı bir şekilde, aynı şeyi ifade etmek için kullanılacaktır: yani internet veya dijital cihazlarda sunulan ve görüntülenen reklamlar.

Popüler terimlerin bir listesini AdTech sözlüğümüzde bulabilirsiniz.

---

## 📬 Sizden Haber Almak İsteriz

Bu kitabı sizin için yazdık. Eğer ekleyebileceğimizi düşündüğünüz ya da geliştirmemizi istediğiniz bir şey varsa, lütfen bizimle iletişime geçin ve bize bildirin.

---

<div align="center">

[⬅️ Ana Sayfa](../README.md) | [➡️ Bölüm 02: Reklamcılığın Temelleri](02-reklamciligin-temelleri.md)

</div>
