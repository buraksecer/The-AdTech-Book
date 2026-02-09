---
layout: default
title: "Bölüm 08: İzlenim, Tıklama ve Dönüşüm Takibi"
---

# Bölüm 08: İzlenim, Tıklama ve Dönüşüm Takibi

Bu kitabın önceki bölümlerinde, reklamverenlerin ve yayıncıların (publishers) kampanyalarını kurmak ve yürütmek için AdTech platformlarını nasıl kullandıklarına baktık.

Bu bölümde ise AdTech platformlarının verileri nasıl topladığını; böylece reklamverenlerin ve yayıncıların kampanyalarının performansına ilişkin ayrıntılı raporları nasıl takip edip görüntüleyebildiklerini inceleyeceğiz.

Bu bölümdeki açıklamaların ve örneklerin çoğu, hem **publisher’ın (yayıncının)** hem de **advertiser’ın (reklamverenin)** ad server’larında takip (tracking) ve raporlamanın nasıl çalıştığını göstermektedir. Ancak DSP’ler ve SSP’ler gibi birçok başka platform da bu işlevleri içerir.

---

## 🎯 Gösterim (Impression), Tıklama (Click) ve Dönüşüm (Conversion) Takibi

Takip (tracking), bir AdTech platformunun önemli bir parçasıdır ve bir reklam kampanyasının performansını anlamanın ve temel metrikleri ölçmenin ilk adımıdır.

Özetle tracking, bir reklam kampanyasına ait verilerin toplanmasını ifade eder.

AdTech platformlarının takip ettiği birçok alan vardır. Bunlar arasında gösterim (impression), tıklama (click) ve dönüşüm (conversion) gibi temel metriklerin yanı sıra **viewability (görünebilirlik)** ve **reklama maruz kalma süresi (ad-exposure time)** gibi metrikler de yer alır. Ayrıca video reklamlar için **gösterim (plays)**, **tamamlama oranları (completion rates)** ve **ortalama izlenme süresi (average time played)** gibi metrikler de takip edilebilir.

---

## 👁️ Gösterim (Impression) Takibi

Gösterim takibi, en basit haliyle her bir reklamın kaç kez gösterildiğinin takip edilmesidir.

Bir reklam her kullanıcıya gösterildiğinde bir gösterim olarak sayılır.

Örneğin, bir kullanıcı bir web sayfasını ziyaret eder, bir reklam görür, ardından sayfayı yeniler ve aynı reklamı tekrar görürse, iki gösterim sayılmış olur.

Bir gösterimi saymanın en yaygın yöntemi, ad server’a bir gösterim gerçekleştiğini bildiren **1×1 boyutunda şeffaf bir görsel** sunmaktır. Buna **impression tracker** (veya **impression pixel**) denir.

Ad server, tarayıcı reklamı render ettiğinde (görüntülediğinde) gösterimi saymak için reklamın HTML markup’ı içine bu pikseli ekler. Bu yöntem, reklam sunucusunun reklamı seçtiği anda değil, reklamın gerçekten tarayıcıda yüklendiği anda sayım yapılmasını sağlar.

Bu sayede reklam gösterimi, tarayıcı kreatifi yüklediği anda sayılmış olur.

Aşağıda Google Ad Manager ad server’ından (eski adıyla DoubleClick for Publishers) bir **impression tracker** örneği yer almaktadır:

Ad server, gösterimi birden fazla sistemde sayabilmek için reklam markup’ına üçüncü taraf AdTech platformlarına ait ek pikseller ekleyebilir.
Örneğin yalnızca ölçüm amacıyla kullanılan üçüncü taraf bir ad server ya da bir **ad verification (reklam doğrulama)** platformu buna örnek olabilir.

Reklam markup’ı içinde başka tag’lerin veya piksellerin yüklenmesi ve diğer platformlara çağrı yapılması süreci **piggybacking** olarak adlandırılır.

Hem publisher’ın hem de advertiser’ın ad server’larında bir gösterimi saymanın iki temel yöntemi vardır:

---

### Yöntem 1: Reklam Markup’ına İki Pixel Eklemek

Publisher’ın ad server’ı, reklam markup’ı içine iki adet **1×1 piksel** ekler.

* İlk piksel, **publisher’ın ad server’ına** bir istek (request) gönderir ve gösterimi sayar.
* İkinci piksel ise **advertiser’ın ad server’ına** bir istek gönderir ve o da gösterimi sayar.

Her iki piksel de kendi ad server’larına **aynı anda** gönderilir.

(Şekil: *Impression tracking – Method 1*)

---

### Yöntem 2: Ad Server Request Bazlı Sayım

Hem publisher’ın hem de advertiser’ın ad server’ları, **yalnızca kendi ad server’larına reklam için bir istek ulaştığında** gösterimi sayar.

**Gösterim Takibi: Yöntem 2**

(Şekilde gösterildiği gibi süreç şu adımlarla ilerler:)

1. Tarayıcı, web sitesini yüklemek için **publisher’ın web server’ına** bağlanır.
2. Publisher’ın web server’ı, reklam alanının (ad slot) kodunu içeren web sitesinin HTML’ini döner.
3. Reklam alanının kodu, tarayıcının **publisher’ın ad server’ına** bir istek göndermesini tetikler.
4. Publisher’ın ad server’ı:

   * Gösterimi sayar
   * Advertiser’ın ad server’ına işaret eden ad tag’ini döner
5. Advertiser’ın ad tag’i, tarayıcının **advertiser’ın (3. taraf) ad server’ına** bir istek göndermesini tetikler.
6. Advertiser’ın ad server’ı:

   * Gösterimi sayar
   * CDN üzerindeki kreatife link içeren ad markup’ı döner
7. Tarayıcı, kreatifi yüklemek için **Content Delivery Network (CDN)**’e istek gönderir.
8. Kreatif geri döner ve ad markup tarafından reklam alanında render edilir.

---

## 🖱️ Tıklama (Click) Takibi

Bir reklamın aldığı tıklama sayısının takibi genellikle bir **click tracker** aracılığıyla yapılır.

Click tracker, ad server’ın **redirect (yönlendirme) servisine ait URL’dir**. Bu servis tıklamayı sayar ve ziyaretçiyi kampanyanın nihai açılış sayfasına (final landing page) yönlendirir.

Ad server, ziyaretçi nihai açılış sayfasına yönlendirilmeden önce tıklamanın sayılabilmesi için click tracker URL’sini reklam markup’ı içinde döner.

Aşağıda Google Ad Manager ad server’ından bir **click tracker** örneği yer almaktadır.

---

**Bir click tracker’ın nasıl çalıştığına dair temel akış aşağıdaki gibidir:**

**Bir publisher’ın ad server’ında tıklama takibinin nasıl çalıştığı**

(Şekildeki akış şu şekildedir:)

0. Kreatif, ad tag tarafından reklam alanına yüklenir ve render edilir.
1. Kullanıcı reklama tıklar ve **publisher’ın ad server’ına** yönlendirilir; ad server bu noktada tıklamayı sayar.
2. Publisher’ın ad server’ı, **advertiser’ın landing page’ine** yönlendiren bir **HTTP 302 redirect** döner.
3. Tarayıcı bu yönlendirmeyi takip eder ve advertiser’ın landing page’ini yükler.

---

Yukarıdaki diyagram, bir **publisher’ın ad server’ı** ile tıklama takibinin nasıl çalıştığını göstermektedir.
Peki advertiser da tıklamayı takip etmek isterse ne olur?

Bunu sağlamak için, **publisher’ın ad server’ından advertiser’ın ad server’ına** bir **click redirect** eklenmesi gerekir; ardından kullanıcı landing page’e yönlendirilir.

**Publisher ve Advertiser ad server’larında tıklama takibinin nasıl çalıştığı**

(Şekildeki akış aşağıdaki gibidir:)

0. Kreatif ad tag tarafından reklam alanına yüklenir ve render edilir.
1. Kullanıcı reklama tıklar ve **publisher’ın ad server’ına** yönlendirilir; publisher ad server bu noktada tıklamayı sayar.
2. Publisher’ın ad server’ı bir **HTTP 302 redirect** döner.
3. Tarayıcı bu yönlendirmeyi takip ederek **advertiser’ın ad server’ına** gider ve advertiser ad server tıklamayı sayar.
4. Advertiser’ın ad server’ı bir **HTTP redirect** döner ve kullanıcıyı **advertiser’ın landing page’ine** yönlendirir.
5. Tarayıcı advertiser’ın landing page’ini yükler.

---

Advertiser’ın ad server’ının aynı tıklamayı ve gösterimi de saymasının nedeni, publisher tarafından sağlanan raporları doğrulamak (impression ve click sayılarının karşılaştırılması) ve tüm kampanya verisini tek bir sistemde (yani advertiser’ın ad server’ında) toplamak istemesidir.

Daha fazla işlem gerçekleştirmek için redirect zincirine ek yönlendirmeler eklemek mümkündür. Örneğin:

* **Ad verification**: Görülebilir gösterimleri (viewable impressions), botları ve sahte aktiviteleri tespit etmek.
* **Aracı sistemlerde tıklama takibi**: Örneğin ad network’ler gibi.

---

### 🔗 Click URL Makroları

Click tracker’lar, hedef URL’nin bir parametre olarak iletilmesini destekleyebilir (ör. `redir_url=`).
Bu özellik, redirect zincirine birden fazla click tracker eklemek ve bir sonraki yönlendirmenin URL’sini dinamik olarak click tracker’a geçirmek için gereklidir.

Genellikle ad server’a bir click tracker eklerken, zincirdeki bir sonraki click tracker’ın URL’sini genişletmek için **click URL macro** kullanılır.

Örnek:

```
https://ad.example.org/click?ad_id=123456&redir_url=%%click_url%%
```

Ad server, `%%CLICK_URL%%` yer tutucusunu zincirdeki bir sonraki click tracker ile otomatik olarak genişletir (yani kendi click tracker’ı ile).

## 🎯 Dönüşüm (Conversion) Takibi

Bir **conversion (dönüşüm)**, bir kullanıcı reklamverenin veya pazarlamacının belirlediği bir hedefi her tamamladığında kaydedilir.

Bu hedef; bir ürün satın almak, bir dosya indirmek ya da bir landing page üzerindeki iletişim formunu doldurmak olabilir. Kullanıcı bu aksiyonlardan herhangi birini her gerçekleştirdiğinde bir dönüşüm kaydı oluşur.

Online reklamcılık ve pazarlamada dönüşüm takibi, kampanya performansını raporlamak için kullanılır. Ayrıca **CPA (cost-per-action)** modelinde de kullanılır; bu modelde publisher’lar ve affiliate reklamverenler/pazarlamacılar **yalnızca bir dönüşüm gerçekleştiğinde** ödeme alırlar.

İki temel dönüşüm türü vardır:
**Click-through conversion** ve **View-through conversion**.

---

### Click-through Conversion

Bir kullanıcı **reklama tıklamış** ve ardından **dönüşüm gerçekleştirmişse** buna click-through conversion denir.

Click-through conversion oranını (**CTC**) hesaplamak için, dönüşüm sayısı reklamın aldığı tıklama sayısına bölünür:

**CTC % = (dönüşümler ÷ tıklamalar) × 100**

---

### View-through Conversion

Bir kullanıcı **reklamı görmüş**, **tıklamamış**, ancak daha sonra **dönüşüm gerçekleştirmişse** buna view-through conversion denir.

Örneğin, kullanıcı bir ayakkabı reklamını görür; reklama tıklamadan doğrudan web sitesine gider ve ürünü satın alır.

View-through conversion oranını (**VTC**) hesaplamak için, dönüşüm sayısı reklamın aldığı gösterim sayısına bölünür:

**VTC % = (dönüşümler ÷ gösterimler) × 100**

CTC ve VTC oranları, reklamverenden reklamverene ciddi şekilde değişebilir. Bunun nedeni; tanıtılan ürün veya hizmet, hedef kitle ve reklam maruziyeti gibi birçok faktörün etkili olmasıdır.

---

### Attribution Window (Atıf Penceresi) Nedir?

Her iki dönüşüm modelinde de **attribution window (atıf penceresi)** adı verilen bir kavram vardır. Bu, kullanıcının reklamı ilk gördüğü veya tıkladığı an ile dönüşümü gerçekleştirdiği an arasındaki süreyi ifade eder.

Atıf penceresi reklamverenden reklamverene değişir; genellikle **24 saat ile 30 gün** arasında olabilir.

Doğru atıf penceresini belirlemek zor olabilir. Çünkü atıf penceresi uzadıkça, atfın doğruluğu azalır.

Örneğin, bir kullanıcının dönüşüm gerçekleştirmesinin nedeni 30 gün önce gördüğü bir reklam mıydı, yoksa başka bir pazarlama kanalının etkisi mi olduğunu anlamak zorlaşır.

Benzer şekilde, atıf penceresi **çok kısa** tutulursa, reklamı görüp onun etkisiyle dönüşüm yapan bazı kullanıcılar kapsam dışı kalabilir. Bu durum yalnızca reklamverenin atıf raporlarını değil, publisher’ın potansiyel gelirini de etkiler.

---

### Click-through ve View-through Conversion Karşılaştırması

**Click-through conversion – Avantajlar**

* Tıklamaların dönüşümlere daha doğru şekilde atfedilmesini sağlar.
* Yanlış raporlama için çok az veya hiç alan bırakmaz.

**Click-through conversion – Dezavantajlar**

* Dezavantajların çoğu, dönüşüm türünden ziyade kullanılan **attribution modeli** ile ilgilidir.
* Örneğin first-click veya last-click attribution kullanıldığında, dönüşümü gerçekten tetikleyen etkileşimin hangisi olduğunu anlamak zor olabilir.

**View-through conversion – Avantajlar**

* Ürün veya hizmete bağlı olarak, özellikle **middle-funnel** ve **top-funnel** kampanyalarda click-through conversion’a göre daha iyi çalışabilir.

**View-through conversion – Dezavantajlar**

* Reklam kullanıcıya gösterilmiş olabilir ama kullanıcı onu gerçekten görmemiş olabilir (örneğin reklam viewport içinde olmayabilir).
* Kampanyaya gerçekte olduğundan fazla dönüşüm atfedilmesi mümkündür.
* Kullanıcı reklamı gördükten sonra dönüşümden önce çerezlerini silerse, dönüşüm atfı kaybolabilir.
* Bu yöntem dolandırıcılığa daha açıktır. Örneğin kreatif gösterilmeden piksel tetiklenebilir. Bu durumda kullanıcı dönüşüm yaparsa, reklamı hiç görmemiş olsa bile view-through conversion olarak kaydedilebilir.

Bu iki dönüşüm türü, kullanıcının bir marka veya reklamla olan farklı etkileşimlerini dikkate alan daha geniş bir alan olan **attribution (atıf)** kavramının parçasıdır.

---

### 🧩 Pixel Yöntemi (The Pixel Method)

**Click-through conversion takibi** için kullanılan pixel yöntemi şu şekilde çalışır:

Pixel yönteminde kullanıcı bir web sitesini ziyaret eder, bir reklam görür ve reklama tıklar. Ardından advertiser’ın landing page’ine yönlendirilir ve dönüşümü gerçekleştirir. Kullanıcı reklama tıkladığında, advertiser’ın **conversion pixel’i** tetiklenir ve kullanıcının **cookie ID’sini** advertiser’ın ad server’ına kaydeder.

Genellikle ad server, ilgili cookie ID için **son tıklamanın** (last click) dönüşümü oluşturduğunu varsayar.

(Şekil: Pixel yöntemiyle click-through conversion takibi)

Bu şekilde dönüşüm, **belirli bir reklam**, **line item** ve **kampanya** ile ilişkilendirilebilir (click ID, kullanıcının hangi reklama tıkladığına dair bilgiyi saklar).

---

### 👁️ View-through Tracking için Pixel Yöntemi

View-through dönüşümler için pixel yöntemi şu şekilde çalışır:

Bu yöntemde kullanıcı bir reklamı **görür ancak tıklamaz**, publisher’ın web sitesinden ayrılır, daha sonra **başka bir kanal üzerinden** (örneğin Google aramasıyla) advertiser’ın web sitesine geri döner ve dönüşüm gerçekleştirir.

Advertiser, publisher’ın sitesinde reklam gösterildiği anda oluşturulan **cookie ID** ile, başarı (success) sayfasında conversion pixel tetiklendiğinde okunan cookie ID’yi karşılaştırarak dönüşümü publisher’daki reklama atfedebilir.

---

### 🖧 Server-Side Yöntem

Server-side yöntem, pixel yöntemine benzer şekilde çalışır; ancak burada pixel tetiklenip kullanıcının cookie ID’si ad server’a gönderilmek yerine, cookie ID **sayfadan ad server’a server-to-server (sunucudan sunucuya) bir çağrı** ile iletilir.

Bu yöntem, özellikle **affiliate reklamcılığı ve pazarlaması** alanında yaygın olarak kullanılır. Bunun nedeni, verinin doğru olması ve dönüşümlerin güvenilir şekilde takip edilmesinin kritik önemde olmasıdır; çünkü publisher’lar (affiliate’ler) **yalnızca dönüşüm gerçekleştiğinde ödeme alırlar**.

Aşağıda server-side yöntemi açıklamak için iki örnek verilmiştir:

---

### Örnek 1: Affiliate olarak sigorta satışı

Affiliate reklamverenler ve pazarlamacılar **CPA (cost-per-action / acquisition)** modeliyle ödeme alırlar. Bu da, kullanıcının dönüşüm gerçekleştirmesi durumunda — sabit bir komisyon ya da satış tutarının belli bir yüzdesi şeklinde — ödeme aldıkları anlamına gelir.

Ancak, bir kullanıcının publisher’ın sitesinde sigorta reklamını görmesi ile gerçekten dönüşüm yapması (sigorta poliçesini satın alması) arasında **saatler, günler hatta haftalar** geçebilir.

Bu nedenle advertiser tarafındaki sistemin, **click ID’yi takip etmesi** ve dönüşüm doğrulandıktan sonra (örneğin başvuru başarıyla işlendiğinde veya ödeme alındığında) affiliate ad network’ünü (veya ad server’ı) başarılı dönüşüm hakkında bilgilendirmesi gerekir.

---

### Örnek 2: Uygulama (App) yüklemeleri

Bir uygulama yüklemesinin dönüşümünü bir publisher’a veya affiliate’e atfetmek, tarayıcı tabanlı dönüşümlere kıyasla farklıdır. Bunun nedeni; web ve mobil tarayıcıların aksine, **mobil uygulamalarda pixel tetiklenememesidir**.

Bu nedenle dönüşüm gibi **Event**’leri takip edebilmek için, uygulama içindeki **SDK (software development kit)** ad server’a yükleme bilgisini bildirir. Bu yükleme daha sonra partner tarafından oluşturulan **app store yönlendirmesine** (publisher veya affiliate) atfedilir.

Başarılı bir yükleme gerçekleştiğinde, publisher’a veya affiliate’e bir **postback bildirimi** gönderilir; bu da CPA komisyonunun kazanıldığı anlamına gelir.

---

## Affiliate Kampanyalarını Doğru Atfetmenin Önemi

Tahmin edebileceğiniz gibi, **CPA kampanyalarında güven** sıkça karşılaşılan bir problemdir.

Reklamverenlerin publisher’lara ve affiliate’lere komisyon ödememek için başvurabilecekleri bazı yollar vardır; ancak bu durum uzun vadede hem reklamverene hem de publisher/affiliate’e zarar verir.

Açıklayalım.

Affiliate, CPA ve revenue-share dünyasında publisher’lar genellikle tanıtacakları **yüzlerce teklif (offer)** arasından seçim yapabilir.

Publisher’ın ve affiliate’in amacı, tanıttıkları teklifler üzerinden **en yüksek geliri** elde etmektir. Bu nedenle teklifleri genellikle trafiğin küçük bir kısmıyla test eder, ardından en çok gelir getirenleri bulmak için optimizasyon yaparlar.

Eğer teklifler iyi performans göstermezse (örneğin hedef kitleye uygun olmaması gibi nedenlerle), publisher bu teklifleri sitesinden kaldırır ve tanıtmayı bırakır. Bu durumda reklamveren de bu tekliflerden **hiç dönüşüm alamaz**.

Bu da sürecin tüm amacını ortadan kaldırır.

---

## 📊 Raporlama (Reporting)

Bir AdTech platformunun raporlama fonksiyonu, kampanyanın birçok farklı alanına ait metrikleri göstermekten sorumludur.

Raporlar hem advertiser’lar hem de publisher’lar için son derece değerlidir; çünkü kampanya performansı ve reklamlara tıklayan kullanıcılar hakkında net içgörüler sunar.

Her gösterim (impression) için AdTech platformu aşağıdaki bilgileri içeren bir kayıt saklar:

* Zaman damgası (impression, click, conversion)
* IP adresi
* Kampanya ID
* Line item ID
* Reklam / kreatif ID
* Coğrafi konum
* Tarayıcı
* İşletim sistemi (OS)
* Publisher domain’i
* Publisher placement
* … ve diğerleri

Benzer bilgiler her tıklama ve dönüşüm için de saklanır.

---

## 📈 Metrikler (Metrics)

Bir **metric**, genel kampanya için ya da belirli bir dimension değerine karşılık gelen veriler için hesaplanan **sayısal bir değerdir**.

Bazı metrikler diğerlerinden türetilebilir. Örneğin **CTR**, toplam tıklama sayısının toplam gösterim sayısına bölünmesiyle hesaplanır:

**CTR = (tıklamalar ÷ gösterimler) × 100**

### Örnek metrikler:

* **Impressions (Gösterimler):** Bir reklamın kaç kez gösterildiği
* **Clicks (Tıklamalar):** Reklamın kaç kez tıklandığı
* **Conversions (Dönüşümler):** Kullanıcının gerçekleştirdiği hedef aksiyon sayısı (ör. form doldurma, satın alma)
* **Reach:** Kampanyanın ulaştığı tekil ziyaretçi / cihaz sayısı
* **Click-through rate (CTR):** Tıklamalar / Gösterimler × 100
* **Cost per mille (CPM):** 1.000 gösterim başına maliyet
* **Cost per click (CPC):** Bir tıklamanın maliyeti
* **Cost per action / acquisition (CPA):** Bir aksiyonun, edinimin veya dönüşümün maliyeti (özellikle affiliate marketing’de kullanılır)
* **Conversion rate (CVR):** Dönüşümler / Tıklamalar × 100
  (Genellikle click-through conversion’lar için kullanılır)

---

* **Amount spent (cost):** İlgili gösterimler, tıklamalar ve dönüşümler için harcanan toplam para miktarı.
* **Revenue (total conversion value):** Dönüşümlerden elde edilen toplam gelir.

---

## 🧮 Effective Cost Per Mille, Click ve Action (eCPM, eCPC, eCPA)

Çoğu raporda başında **“e”** harfi bulunan metrikler görürsünüz.

Buradaki **e**, *effective* (etkin) anlamına gelir ve belirli bir fiyatlandırma modelinin fiilen ne kadar gelir ürettiğini hesaplamak için kullanılır (ör. eCPM).

**Effective CPM, CPC ve CPA**, herhangi bir kampanya için hesaplanabilir ve aşağıdaki formüllerle bulunur:

* **Effective cost per click (eCPC)** = harcanan bütçe / tıklama sayısı
* **Effective cost per action/acquisition (eCPA)** = harcanan bütçe / dönüşüm sayısı
* **Effective cost per mille (eCPM)** = (harcanan bütçe / gösterim sayısı) × 1000

Advertiser’lar ve publisher’lar kampanya başlamadan önce bir fiyatlandırma modeli seçtikleri için, bu metrikler onlara **başka bir model kullanılsaydı sonuçların ne olacağını** gösterir.

Çok sık olarak advertiser’lar, kampanyalarını farklı fiyatlandırma modelleriyle hesaplayarak performanslarını karşılaştırırlar.

Publisher tarafında ise, CPM kampanyaları için **eCPC** veya **eCPA** hesaplanarak, bu kampanyaların farklı bir fiyatlandırma modeliyle daha fazla gelir getirip getirmeyeceği analiz edilir.

---

### Örnek Kampanyalar

#### Kampanya #1: CPM

* Gösterimler: 1.000.000
* Tıklamalar: 1.500
* Dönüşümler: 10
* Toplam maliyet: $4.000
* CPM: $4
* eCPC: $2,67
* eCPA: $400

---

#### Kampanya #2: CPC

* Gösterimler: 1.000.000
* Tıklamalar: 2.000
* Dönüşümler: 50
* Toplam maliyet: $10.000
* eCPM: $10
* CPC: $5
* eCPA: $200

---

#### Kampanya #3: CPA

* Gösterimler: 1.000.000
* Tıklamalar: 2.500
* Dönüşümler: 80
* Toplam maliyet: $15.000
* eCPM: $15
* eCPC: $6
* CPA: $187,50

Yukarıdaki tablolar, üç kampanya için **eCPM, eCPC ve eCPA** değerlerini göstermektedir.

---

## 💰 ROI (Return on Investment)

Performans bazlı reklamcılıkta advertiser’lar, kampanya ve trafik kaynağı bazında **ROI**’ye bakarlar. Bu metrik, reklam bütçesinin ne kadar verimli kullanıldığını ölçer.

**ROI şu şekilde hesaplanır:**

**ROI = (toplam dönüşüm değeri − harcanan tutar) / harcanan tutar × 100**

* ROI **pozitifse**, advertiser para kazanıyordur.
* ROI **negatifse**, advertiser zarar ediyordur.

### Örnek:

* **Kampanya 1:**

  * Dönüşüm değeri: $1.200
  * Harcama: $1.000
  * ROI: +%20 → Harcanan her 1 dolar için 20 cent kazanılır

* **Kampanya 2:**

  * Dönüşüm değeri: $900
  * Harcama: $1.000
  * ROI: −%10 → Harcanan her 1 dolar için 10 cent kaybedilir

> Not: Bu hesaplama, ürün veya hizmet teslimiyle ilgili sabit/değişken maliyetleri hesaba katmaz. Bu nedenle %20 ROI her zaman gerçek kâr anlamına gelmeyebilir. Ancak marjinal maliyeti çok düşük olan dijital ürünlerde oldukça sağlıklı bir metriktir.

---

## 🧩 Dimension ve Subdimension’lar

Bir **dimension**, bir raporu parçalamak için kullanılan veri özelliği veya değişkendir.

### Örnek dimension’lar:

* Country
* Device type
* Browser type
* Günün saati
* Campaign
* Line item
* Creative
* Tarih / haftanın günü
* Publisher URL / domain
* OS ve OS versiyonu
* Geolocation

**Subdimension’lar** (drill-down), bir dimension’ın başka bir dimension’a göre kırılımını görmemizi sağlar.
Örneğin:
**Country → Carrier → Line item → Ad**

---

## 🔎 Filtering (Filtreleme)

**Filtering (segmentasyon)**, rapor üzerinde çalışılan veri setini daraltmayı sağlar.

Yaygın filtreler:

* Tarih aralığı
* Advertiser → Insertion Order → Line Item → Ad

Ayrıca herhangi bir dimension için **include / exclude** filtreleri uygulanabilir. Örneğin:

* Country = Poland OR Germany OR United Kingdom
* Device type = Tablet
* Day of week = Monday–Friday

---

## 🛠️ Raporlamada Teknik Hususlar

### Gecikmeler (Delays)

Bir **Event**’in sisteme ulaşması ile raporlara yansıması arasında genellikle bir gecikme vardır.
Çoğu zaman bu birkaç dakikadır, ancak bazen birkaç saate kadar çıkabilir.

En güncel veriler genellikle **yaklaşık (approximate)** olur; **kesin raporlar** biraz zaman sonra hazır olur.
Faturalama için genellikle **kesin raporlar** kullanılmalıdır.

**Örnek:**

* İlk 15 dakika içinde yaklaşık veri
* En geç 24 saat içinde kesin rapor

---

### Raporlama Zaman Dilimi (Time Zone)

Farklı sistemlerden gelen raporlar karşılaştırılırken:

* Aynı zaman diliminin kullanıldığından
* Yaklaşık değil, **kesin verilerin** karşılaştırıldığından
  emin olunmalıdır.

---

### Data Retention (Veri Saklama)

Bazı raporlama sistemleri, veri büyüdükçe belirli bir süreden eski **Event**’leri siler (ör. 6 ay veya 1 yıl).

Alternatif olarak, zaman geçtikçe raporların **granülerliği düşürülür**:

* Son 1 ay: saatlik detay
* 1 ay – 1 yıl: günlük toplamlar
* 1 yıldan eski: yalnızca kampanya toplamları

---

## ⚠️ Discrepancies (Uyuşmazlıklar): Trust, But Verify

Online reklamcılıkta **discrepancy**, iki farklı AdTech platformunda raporlanan veriler arasındaki farktır
(ör. publisher ad server’ı ile advertiser ad server’ı arasındaki farklar).

Bu konu çok hassastır; çünkü bu veriler **faturalama** için kullanılır ve sık sık publisher’lar, advertiser’lar ve AdTech vendor’ları arasında anlaşmazlıklara yol açar.

Discrepancy’lerin birçok nedeni olabilir; ancak çoğu **teknik hatalardan** kaynaklanır.

AdTech platformlarının büyük çoğunluğu, **client-side tracking** (tarayıcılar, mobil SDK’lar, embedded cihazlar) kullanır. Bu yöntem, gösterim, tıklama ve dönüşüm gibi **Event**’leri yakalamada **hata yapmaya açıktır**.

Bu bölümde şu sorular ele alınır:

* Raporların doğru olduğu nasıl doğrulanır?
* Discrepancy’ler neden kaçınılmazdır?
* En yaygın discrepancy nedenleri nelerdir?
* Kabul edilebilir discrepancy seviyesi nedir?

---

### 1. Gösterim Takibi Sırasında Olası Discrepancy

Şekilde görüldüğü gibi:

Publisher’ın ad tag’i yüklenir ve gösterim publisher tarafında sayılır; ancak herhangi bir nedenle tarayıcı, advertiser’ın ad tag’ini veya impression pixel’ini yüklemez.

Bu durumda publisher ve advertiser raporları arasında **gösterim farkı** oluşur.


---

### 2. Tıklama sayılırken (When counting the click)

Bir **discrepancy (uyuşmazlık)**, redirect zinciri kırılırsa oluşabilir. Bu durumda advertiser’ın ad server’ı tıklama bilgisini alamaz ve kullanıcı nihai landing page’e yönlendirilmez.

Yukarıdaki diyagramlarda görüldüğü gibi, çoğu uyuşmazlık **publisher’ın ad server’ı ad tag’i yükledikten sonra** meydana gelir. Bu nedenle advertiser’lar genellikle publisher’lara kıyasla **daha düşük sayılar** raporlar.

---

### Discrepancies ve Yaygın Nedenleri

Aşağıda uyuşmazlıkların neden oluşabileceğine dair bazı olası sebepler yer almaktadır.

### İnsan Kaynaklı ve Implementasyon Hataları

AdOps ekipleri genellikle yoğun ad trafficking işleri ve son dakika değişiklikleriyle uğraşır. Kampanya yayına girmeden hemen önce ajansların tag göndermesi veya değiştirmesi oldukça yaygındır.

Her kampanya için yapılması gereken manuel işler de buna eklenince, özellikle junior ya da aşırı yük altındaki AdOps ekip üyelerinin hata yapması kolaylaşır.

Yaygın hatalar şunlardır:

* **Eksik impression tracking pixel’ı eklemek:**
  Tam ID içermeyen bir pixel advertiser’ın ad server’ına istek gönderir ancak eksik ad veya kampanya kimliği nedeniyle impression sayılmaz.

* **Yanlış impression pixel’ı kullanmak:**
  Örneğin, pastebin’de kalan Campaign ABC pixel’ının yanlışlıkla Campaign 123’e yapıştırılması.

* **Yanlış macro kullanımı:**
  Cache buster eklenmemesi, pixel’ın tarayıcı tarafından cache’lenmesine ve aynı kullanıcıda sonraki gösterimlerin raporlanmamasına yol açabilir.

* **Run date farkları veya kampanyanın ad server’lardan birinde eksik kurulması:**
  Kampanya bir ad server’da başlamış olabilir ancak diğerinde aktif değildir. Bu da reklamın gösterilmemesine neden olur.

Örneğin advertiser tarafındaki tag’ler doğru kurulmamış, publisher tarafında doğru kurulmuşsa; publisher boş reklamın impression’larını saymaya devam eder.

---

### Konfigürasyon Kaynaklı Problemler

Farklı AdTech platformları arasındaki raporlama konfigürasyonları da uyuşmazlıklara neden olabilir:

* **Zaman dilimi (Time zone):**
  Bir platform Central Time (CT), diğeri Pacific Time (PT) kullanıyorsa günlük ve saatlik raporlarda farklar oluşur.

* **Traffic validation ve filtering:**
  Bazı platformlar sahte trafiği engellemek için filtreleme uygular; bu da platformlar arası fark yaratır.

* **Terminoloji ve sayım metodolojisi farkları:**
  Bir platform impression’ı pixel browser’da çalıştığında sayarken, diğeri reklam server’dan çıktığında sayabilir. İkinci durumda reklam tarayıcıda hiç yüklenmese bile impression sayılmış olur.

---

### Client-Side Kaynaklı Problemler

AdTech platformlarının çoğu client-side tracking’e dayanır ve şu teknik sorunlarla karşılaşabilir:

* Zayıf internet bağlantısı ve yüksek latency
* JavaScript hataları
* Tarayıcıda JavaScript’in kapalı olması veya `<noscript>` kullanımı
* URL maksimum uzunluğunun aşılması (redirect zincirinin kesilmesi)
* URL içindeki özel karakterlerin parse edilememesi
* Kreatif dosya boyutunun çok büyük olması veya IAB standartlarına uymaması
* Sayfadaki büyük dosyaların (ör. ağır görseller) yüklenme süresini artırması

---

### Impression Discrepancy Nasıl Hesaplanır?

İki AdTech platformu arasındaki uyuşmazlık şu formülle hesaplanır:

**Impression discrepancy**
= (publisher impression sayısı − advertiser impression sayısı)
÷ advertiser impression sayısı

Yüzdeye çevirmek için sonuç 100 ile çarpılır.

---

### Discrepancy Toleransı

IAB’e göre, publisher verileri baz alındığında **%10’a kadar discrepancy kabul edilebilir**.

Eğer discrepancy %10’un altındaysa, faturalamada genellikle **publisher’ın verileri** kullanılır.

---

### Reconciliation

**Reconciliation**, iki farklı kayıt setinin karşılaştırılarak verilerin doğru ve tutarlı olduğunun doğrulanması sürecidir.

Uyuşmazlıkların çok sayıda sebebi olabildiğinden, reconciliation çoğu zaman manuel bir süreçtir.
AdOps ekipleri platformlara giriş yapar, raporları indirir ve problemin kaynağını analiz eder.

---

## 🎓 Bölüm Özeti

Bu bölümde, AdTech platformlarında **tracking (takip)** ve **raporlama** mantığını; bunun nasıl ölçüm, optimizasyon ve faturalama süreçlerine bağlandığını öğrendik.

### **📚 Öğrendiklerimiz:**

1. **👁️ Gösterim (Impression) Takibi**: En yaygın yöntem **1×1 şeffaf görsel (impression pixel / impression tracker)** kullanmaktır; böylece reklam tarayıcıda render edildiğinde sayım yapılır.
2. **🖱️ Tıklama (Click) Takibi**: Genellikle **click tracker** (redirect URL) kullanılır; tıklama sayılır ve kullanıcı landing page’e yönlendirilir.
3. **🎯 Dönüşüm (Conversion) Takibi**: Dönüşümler pixel yöntemleri veya **server-side** yaklaşımlarla izlenebilir.
4. **🪟 Attribution Window**: Bir gösterim/tıklama ile dönüşüm arasındaki zaman aralığı, atfın doğruluğunu ve kapsama alanını doğrudan etkiler.
5. **📊 Raporlama Bileşenleri**: Raporlar; **metrics**, **dimensions** ve **filtering** kavramlarıyla analiz edilir.
6. **⚠️ Discrepancies (Uyuşmazlıklar)**: Platformlar arası sayım farkları yaygındır; teknik sebepler, konfigürasyon ve implementasyon hatalarından kaynaklanabilir.
7. **🤝 Reconciliation**: Uyuşmazlıkların kaynağını bulmak ve faturalama için “hangi sayı doğrudur?” sorusunu çözmek çoğu zaman manuel bir süreçtir.

### **🔑 Ana Çıkarımlar:**

- **Sayım metodolojisi** (pixel mi request mi?) ve **sayım anı** (render mı response mu?) değiştiğinde, raporlar arasında fark oluşması normaldir.
- Raporları karşılaştırırken **zaman dilimi**, **yaklaşık/kesin rapor ayrımı** ve **filtreleme kuralları** kontrol edilmelidir.
- Discrepancy yönetimi, yalnızca raporlama değil aynı zamanda **güven** ve **faturalama** problemidir.

---

[⬅️ Bölüm 07: Hedefleme ve Bütçe Kontrolü](/The-AdTech-Book/bolumler/07-hedefleme-ve-butce-kontrol.md) | [🏠 Ana Sayfa](/The-AdTech-Book/index.md) | [➡️ Bölüm 09: Medya Satın Alma Yöntemleri](/The-AdTech-Book/bolumler/09-medya-satin-alma-yontemleri.md)
