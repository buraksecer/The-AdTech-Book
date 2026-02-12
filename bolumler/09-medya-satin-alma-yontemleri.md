## 09. Medya Satın Alma Yöntemleri: Programmatic, Gerçek Zamanlı Teklif (RTB), Header Bidding ve PMP

Bu kitapta daha önce ele aldığımız gibi, çevrimiçi reklamcılık sektörü; ad server’lar, DSP’ler, SSP’ler ve reklam ağları gibi birçok reklam teknolojisi platformundan oluşur.

Bu AdTech platformlarının amaçları farklıdır — bazıları reklam gösteriminden (ad serving) sorumluyken, bazıları reklam verenler ve yayıncıların online medya satın alıp satmasına yardımcı olmak üzere tasarlanmıştır.

Bu bölümde, bu AdTech platformlarını çalıştıran medya satın alma süreçlerini inceleyeceğiz.

---

## Başlıca Medya Satın Alma Süreçleri

Aşağıda bu bölümde ele alacağımız temel medya satın alma süreçlerinin genel bir özeti yer almaktadır:

* Manuel medya satın alma
* Programmatic direct
* Gerçek zamanlı teklif (RTB)
* Waterfall
* Header bidding
* Private marketplace (PMP)

Şimdi bu süreçlere daha detaylı bakalım.

---

## Manuel Medya Satın Alma

Online reklamcılığın ilk dönemlerinde, reklam verenler ile yayıncılar arasındaki reklam alım-satımı oldukça manuel bir süreçti.

Reklam verenler yayıncılarla doğrudan çalışır ve reklam etiketlerini (ad tag) doğrudan gönderirdi. Sürece herhangi bir teknolojik platform dahil olmadığı için hedefleme tanımlamak veya rapor üretmek mümkün değildi.

Neyse ki ad server’ların devreye girmesi bu sorunu çözdü ve programatik medya satın alma devrimini başlattı.

---

## Programmatic Medya Satın Alma

### Programmatic Ne Anlama Gelir?

“Programmatic” terimi farklı kişiler için farklı anlamlar taşıyabilir; ancak işte basit ve net bir tanım:

**Programmatic**, online medyanın teknoloji, algoritmalar ve veri kullanılarak otomatik bir şekilde satın alınıp satılmasını ifade eder.

Bunu, teknoloji veya algoritma kullanımını içermeyen ve insan-insana yürütülen manuel reklam satın alma yöntemiyle karşılaştırabilirsiniz.

Aşağıda, manuel satın alınan medya ile programatik olarak satın alınan medyanın yürütme süreçleri arasındaki farkı gösteren bazı örnekler yer almaktadır:

---

## Manuel Medya Satın Alma

Bir **manuel medya işleminin** yürütülmesi:

* Reklam veren ve yayıncı bir insertion order (IO) imzalar. Bu, kampanyanın uçuş tarihleri (flight dates) ve yerleşim (placement) gibi şart ve koşullarını tanımlayan bir sözleşmedir.
* Reklam veren, reklam etiketlerini (ad tag) yayıncıya gönderir. Bu ad tag’ler, yayıncının web sitesinde reklamı gösterecek HTML parçalarıdır.
* Yayıncı, reklam verenin ad tag’lerini web sitesine ekler ve kampanyayı başlatır.

---

## Programmatic Medya Satın Alma

Bir **programatik medya işleminin** yürütülmesi:

* Reklam veren ve yayıncı bir insertion order (IO) imzalar.
* Reklam verenin AdOps ekibi, kampanyayı reklam verenin ad server’ında (third-party ad server) yapılandırır ve ad tag’leri yayıncıya gönderir.
* Yayıncının AdOps ekibi kampanyayı kendi ad server’ında (first-party ad server) kurar, reklam verenin ad tag’lerini ekler ve kampanyayı başlatır.

Yukarıdaki süreçler benzer görünse de, ad server kullanmanın temel avantajı; manuel medya satın almaya kıyasla sağladığı ek faydalardır. Bunlar arasında hedefleme, yerleşim kontrolü, raporlama ve rutin/tekrarlı işlerin ortadan kaldırılması yer alır.

Örneğin, yayıncının reklam verenin ad tag’ini doğrudan web sitesine ekleyip sadece sayfa yüklendiğinde reklamı göstermesi yerine, ad tag reklam verenin ad server’ına yönlenebilir. Bunun avantajı, ad server’ın; kullanıcının konumu, cihazı gibi birçok faktöre göre hangi reklamın gösterileceğine karar verebilmesidir.

---

Manuel ve programatik medya satın alma arasındaki bir diğer önemli fark, kampanyayı başlatma ve kampanya yayındayken değiştirme hızıdır.

Bir DSP gibi programatik bir AdTech platformunda kampanya oluşturmak ve yayına almak dakikalar sürebilir. Programatik teknolojiler olmadan ise kampanyanın başlaması birkaç gün alabilir.

Ayrıca, manuel medya satın alımında kampanyadaki her değişiklik yayıncının AdOps ekibi üzerinden geçmek zorundadır ve uygulanması birkaç gün sürebilir. Programatik platformlarda ise yapılan değişiklikler neredeyse gerçek zamanlı olarak yansıtılır.

Bu durum oldukça kritiktir; çünkü markaların değişimlere hızlı tepki vermesi gerekir ve kampanya optimizasyonu saatlik veya günlük bazda yapılabilir.

---

# Kampanya Optimizasyonu Temelleri: Manuel vs. Algoritmalar

Kampanya optimizasyonu, performansı artırmak ve medya satın alımını daha ekonomik hale getirmek için kampanyada değişiklikler yapılmasını ifade eder.

Bir kampanyada değiştirilebilecek birçok alan vardır; örneğin hedefleme kriterleri ve reklam kreatifleri.

Kampanyalar manuel olarak veya algoritmalar aracılığıyla optimize edilebilir.

---

## Manuel Optimizasyon

Manuel optimizasyon genellikle reklam verenlerin CPC, CPA ve CPM tekliflerini (bid) günlük bazda ayarlamasını içerir.

Temelde reklam veren, reklam platformunun sağladığı farklı boyutlara (dimension) göre ayrılmış verileri kullanır — örneğin coğrafi konum, cinsiyet, ilgi alanı, cihaz türü vb. — ve bu boyutları kullanarak belirli gruplara yönelik hedeflemeyi genişletir veya daraltır.

Bu sayede en optimal CTR, CPA veya dönüşüm oranını sağlayacak çok spesifik hedefleme kriterleri oluşturulur.

Optimizasyon yapabilmek için reklam verenler, hangi tekliflerin ayarlanacağına karar verirken şu verileri kullanır:

* Reklamların CTR’ları
* Reklamların ürettiği tıklama sayısı
* Reklamların ürettiği gösterim (impression) sayısı

Manuel olarak kampanya optimize etmek isteyen medya satın almacıların kullanabileceği bir süreç:

* Veriyi bir veya daha fazla boyuta göre kırılımlara ayırmak (örneğin coğrafi konum, cihaz, yayıncı domain’i, günün saati, operatör vb.).
* Anlamsız/istatistiksel olarak düşük verileri filtrelemek. Örneğin çok az gösterim veya tıklama üreten reklamları elemek ya da en çok gösterim/tıklama üreten reklamları incelemek.
* En iyi ve en kötü performans gösteren değerleri görmek (örneğin cihaz türü veya coğrafi konum).
* Optimize etmek istediğiniz metriğe göre belirli metrikleri incelemek. Örneğin bir e-kitap indirme için efektif CPM (eCPM) ya da satış hunisinin daha alt aşamasındaki bir metrik, örneğin nitelikli lead başına maliyet.
* Düşük performans gösteren alanları blacklist’e almak (hedeflemeden çıkarmak).

Reklam verenlerin kampanya optimizasyonu için kullanabileceği diğer teknikler:

* **A/B testleri yapmak:** Kreatiflerde değişiklik yapıp hangi varyantın daha iyi performans gösterdiğini test etmek.
* **Kreatifleri kişiselleştirmek (dynamic creatives):** Mesaj veya görsel unsurları farklı segmentler için daha alakalı hale getirmek. Örneğin kullanıcının bulunduğu şehrin adını kreatife eklemek.
* **Farklı trafik kaynaklarını denemek:** Farklı web siteleri, farklı reklam formatları (display, video vb.) ve farklı AdTech platformlarını bütçenin küçük bir kısmıyla (örneğin %5–10) test edip eCPA, eCPM gibi metrikleri karşılaştırmak.

---

## Otomatik (Automated) Optimizasyon

Otomatik optimizasyon, sürecin algoritmalar tarafından yürütülmesini ifade eder.

Birçok AdTech platformu, belirli seviyede otomatik optimizasyon sağlayan yerleşik algoritmalara sahiptir.

Başarılı bir otomatik optimizasyonun temel bileşeni geçmiş veridir (historical data). Algoritmalar ancak yeterli miktarda ve kaliteli veriyle beslendiklerinde doğru kararlar alabilir ve anlamlı optimizasyon yapabilirler.

---

# Programmatic Direct

**Programmatic direct** (programmatic guaranteed, programmatic reserved veya automated guaranteed olarak da bilinir), medya satın alım ve satım yöntemidir; ancak RTB’den farklı olarak açık artırma yapılmaz.

Bunun yerine reklam veren ve yayıncı, envanter ve CPM üzerinde anlaşır. Sürecin geri kalanı ise AdTech platformları aracılığıyla programatik olarak yürütülür.

Programmatic direct, internet öncesi dönemde ve online reklamcılığın ilk günlerinde yapılan medya satın alımına oldukça benzer; ancak reklam teknolojisi sayesinde çok daha büyük ölçekte gerçekleştirilebilir.

## Programmatic Direct (devam)

Programmatic direct süreci, bir e-ticaret platformunda sipariş vermeye benzer; ancak bir ürün satın almak yerine medya envanteri satın alırsınız.

Süreç şu şekilde işler:

* Reklam veren, web sitelerinin kataloglarını inceler.
* Yerleşimleri (placements), yayın tarihlerini (flight dates) ve gösterim hacmini (impression volume) seçer.
* Kreatifleri ve ek takip piksellerini (tracking pixels) yapılandırır.
* Platform üzerinden sipariş verir.
* Yayıncı kampanyayı denetler ve doğrular.
* Sipariş, AdOps ekibinin ek bir müdahalesi olmadan (denetim dışında) yürütülür.

Programmatic direct’in en büyük avantajı, premium envanteri premium bir fiyattan güvence altına alabilme imkânıdır.

Her ne kadar RTB gibi diğer satın alma yöntemlerine kıyasla daha yüksek CPM’ler ödenmesi gerekse de, reklam verenler açık artırmaya çıkmadan önce premium envanteri garanti altına alabilir. Bu da hedef kitleye, aksi halde ulaşamayacakları durumlarda ulaşmalarını sağlar.

Yayıncılar için bu model daha yüksek CPM anlamına gelir.

Reklam verenler açısından en büyük dezavantaj ise hedefleme seçeneklerinin daha sınırlı olmasıdır; çünkü reklamlar çoğunlukla sitenin bağlamı (context) ve bilinen kitlesine göre gösterilir.

Örneğin, bir banka yeni bir hesap ürünü için finans odaklı bir web sitesinde reklam yayınlayabilir.

RTB ile karşılaştırıldığında ise aynı banka, reklamını birçok farklı web sitesinde sadece kendi sitesini daha önce ziyaret etmiş kullanıcılara gösterebilir.

Yayıncılar için dezavantaj, tüm envanterlerini programmatic direct üzerinden satamayabilmeleridir. Bu nedenle birçok yayıncı, mümkün olduğunca fazla envanteri satabilmek için waterfall yapısı kurar (aşağıda detaylandırılacaktır).

---

# Real-Time Bidding (RTB)

90’ların ortası ile sonu arasında birçok reklam ağı (ad network) ortaya çıktı ve 2000’lerin ortasına gelindiğinde piyasada yüzlerce ad network bulunuyordu.

Ancak reklam ağları kısa süre içinde iki problemle karşılaştı:

* **Underfilling:** Ad network’lerin, yayıncının mevcut envanterini dolduracak yeterli alıcıya sahip olmaması (örneğin %50 fill rate).
* **Overfilling:** Reklam verenlerin, yayıncının sağlayabileceğinden daha fazla medya sipariş etmesi (örneğin %100’ün üzerinde fill rate).

Yayıncılar, ad network’lerinin tüm envanteri satamadığını fark edince birden fazla ad network ile çalışmaya başladı. Ancak bu durum web sitelerine daha fazla tag eklenmesine neden oldu; bu da gecikme (latency) ve kötü kullanıcı deneyimi yarattı.

Bu gecikme problemini çözmek için yeni bir platform türü ortaya çıktı: **Supply-Side Platforms (SSP’ler)**. İlk başta “network optimizers” olarak adlandırıldılar.

### İlk SSP’ler

Piyasaya çıkan ilk SSP’ler şunlardı: Collective, Pubmatic, Admeld ve Magnite (eski adıyla The Rubicon Project).

Bir web sitesine birden fazla tag eklemek yerine, yayıncılar artık sadece SSP’ye yönlendiren tek bir tag ekliyordu.

SSP, hangi ad network’lerin yayıncının envanterini satın almak istediğini belirliyor ve işlemi sonuçlandırıyordu.

2000’lerin ortası ve sonu sadece SSP’lerin değil, aynı zamanda **Demand-Side Platforms (DSP’lerin)** de yükselişine sahne oldu.

DSP’ler, medya satın almacıların (reklam verenler ve ajanslar) SSP’ler üzerinden sunulan yayıncı envanterine bağlanmasını sağlamak için ortaya çıktı.

### İlk DSP’ler

İlk DSP’ler arasında Invite Media (daha sonra Google Marketing Platform’un parçası oldu), DataXu ve MediaMath yer alıyordu.

Aynı dönemde online display reklamcılığında bir diğer devrimsel platform ortaya çıktı: **Ad Exchange**.

Ad exchange’ler, yayıncının envanterini impression bazında açık artırmaya çıkararak likidite sorunlarını çözmek amacıyla geliştirildi.

Ad exchange, reklam veren ile yayıncı arasındaki medya alım-satımını yönetir.

Ad exchange’i anlamanın en kolay yolu, onu bir borsaya benzetmektir.

Nasıl ki borsalar hisse senedi ve diğer menkul kıymetlerin alım-satımını kolaylaştırırsa, ad exchange’ler de reklam gösterimlerinin (impressions) reklam verenler ve yayıncılar arasında gerçek zamanlı alım-satımını sağlar.

---

## Biliyor muydunuz?

2007 yılında en büyük üç ad exchange — DoubleClick, AdECN ve RightMedia — sırasıyla Google, Microsoft ve Yahoo tarafından satın alındı.

Gösterimlerin (impressions) gerçek zamanlı olarak tek tek alınıp satılmasına **real-time bidding (RTB)** denir.

---

## Real-Time Bidding (RTB) Nedir?

RTB, 2000’lerin sonunda ortaya çıkan ve online medyanın satın alınma ve satılma şeklini kökten değiştiren bir protokoldür.

Başlangıçta yayıncıların remnant (satılamayan) envanteri reklam verenlere satmasına yardımcı olmak için tasarlanan RTB, bugün premium envanter dahil olmak üzere her tür envanterin satışında kullanılmaktadır.

RTB sayesinde reklam verenler, tek bir yayıncıdan binlerce gösterim satın almak yerine, birçok farklı yayıncıdan tekil gösterimleri satın alabilir ve o anda bilinen site ve kullanıcı bilgilerine göre teklif verebilir.

Yayıncılar da envanterleri için daha yüksek CPM’ler elde edebilir.

---

## RTB Projesi (OpenRTB) Nedir?

RTB Project, eski adıyla OpenRTB Consortium ve bugün OpenRTB olarak bilinen, IAB (Interactive Advertising Bureau) liderliğinde kurulmuş; talep ve arz tarafındaki AdTech şirketlerinden oluşan bir gruptur.

Kasım 2010’da başlatılan OpenRTB, AdTech sağlayıcılarına bir API spesifikasyonu sunar.

OpenRTB protokolü, platformların dijital medyayı alıp satabilmesi için ortak bir dil üzerinden birbirleriyle iletişim kurmasını sağlar.

---

## RTB Nasıl Çalışır?

RTB’nin teknik tarafı oldukça karmaşıktır ve birden fazla AdTech platformunu içerir.

Aşağıda RTB ad exchange sürecinin detaylı bir açıklaması ve diyagramı yer almaktadır.

## RTB Sürecine Detaylı Bakış

* Bir kullanıcı bir sayfayı ziyaret eder (örneğin example.com).
* Sayfada, first-party ad server’dan içerik talep eden bir JavaScript kodu içeren bir reklam alanı (ad slot) vardır. Bu talep bir **ad request** olarak adlandırılır. Talep, kullanıcının konumu, cihaz türü ve işletim sistemi gibi ek bilgileri de iletir.
* Ad server, kullanıcıyla eşleşen doğrudan (direct) kampanya olup olmadığını kontrol eder. Eğer yoksa, gösterimi RTB açık artırmasına sunacak olan SSP’nin ad tag’ini döner.
* Tarayıcı, SSP ad tag’inde bulunan script’i yükler. Kullanıcı bilgileri ve sayfa URL’si, boyut, kısıtlamalar gibi yerleşim detayları ad exchange’e iletilir.
* Ad exchange, mevcut reklam gösterimini tüm teklif verenlere bir **bid request** ile duyurur.
* Bidders (DSP’ler), bid request’i değerlendirir ve hedefleme parametreleri (sayfa domain’i, bağlam, konum ve kullanıcı hakkında toplanan diğer veriler) ile eşleştirir. Ardından tekliflerini iletirler — yani bu gösterim için ne kadar ödemek istediklerini belirtirler. Ayrıca göstermek istedikleri reklamın markup’ını da gönderirler. Teklif fiyatı ve ad markup, **bid response** adı verilen bir obje içinde iletilir.
* Ad exchange teklifleri toplar ve gösterim en yüksek teklifi verene gider. En yüksek teklif veren, ikinci en yüksek teklifin fiyatını küçük bir artışla (genellikle $0.01) öder. Bu modele **second-price auction** denir. Kazanan DSP’ye son fiyat bilgisi iletilir. Kazanan DSP’nin ad markup’ı tarayıcıya gönderilir.
* DSP’nin ad markup’ı tarayıcıda yüklenir ve kreatifi (reklam görseli/video vb.) almak için DSP’nin ad server’ına bir istek gönderir. Çoğu zaman kreatif, doğrudan ad server’dan değil bir CDN’den yüklenir. Aynı zamanda impression tracking pixel’i tetiklenir.
* DSP’nin ad server’ı kreatifi tarayıcıya gönderir ve reklam kullanıcıya gösterilir.

Tüm bu süreç gerçek zamanlı olarak, genellikle **100–150 milisaniye** içinde gerçekleşir. Karşılaştırma yapmak gerekirse, göz kırpmak yaklaşık **300 milisaniye** sürer.

Her sayfa yüklendiğinde veya yenilendiğinde yeni bir ad request oluşur ve yeni bir RTB açık artırması başlar.

---

## Bid Request ve Bid Response İçeriği

Bid request ve bid response mesajları genellikle JSON formatında iletilir.

### Örnek Bid Request (OpenRTB 2.5)

Bu tür bir bid request aşağıdaki bilgileri içerebilir:

* Gösterim bilgisi (imp)
* Site bilgisi (domain, page URL, publisher ID)
* Cihaz bilgisi (user agent, model, IP)
* Kullanıcı ID’si

---

### Örnek Bid Response

Bid response tipik olarak şu alanları içerir:

* Teklif ID’si
* Para birimi
* Seat ID
* Teklif edilen fiyat (price)
* Win notice URL (nurl)
* Kreatif URL’si
* Reklamveren domain’i
* Campaign ID
* Creative ID
* Özellikler (attr)

OpenRTB spesifikasyonları onlarca obje (örneğin BidRequest, Source, Device) ve obje attribute’ü tanımlar.

Bu objeler, DSP’lerin bir gösterime teklif verip vermemeye karar vermesine yardımcı olur ve reklam verene bilgi aktarımını sağlar.

---

## Başlıca OpenRTB Objeleri

### Imp (Impression)

* id
* banner
* video
* audio
* native

### Banner

* w (width)
* h (height)

### Video

* minduration (minimum süre)
* maxduration (maksimum süre)
* skip (atlama mümkün mü?)

Diğer objeler audio, native ve in-app mobil reklamlar için de vardır.

---

### Publisher

* id
* name
* domain

### Device

* ua (user agent)
* geo (konum)
* devicetype
* make
* model
* os
* language
* carrier

### Geo

* lat (enlem)
* lon (boylam)
* country
* region
* city
* zip

### User

* id
* yob (doğum yılı)
* gender

### Data

* id
* name
* segment

### Segment

* id
* name
* value

Detaylı liste için OpenRTB 2.5 ve 3.0 spesifikasyonlarına bakılabilir.

---

# RTB’nin Reklam Verenler ve Yayıncılar İçin Faydaları

## Reklam Verenler İçin

**Artan reklam etkinliği:** Reklam verenler kampanya sonuçlarını gerçek zamanlı görebilir ve performansı artırmak için değişiklik yapabilir. Bu değişiklikler manuel veya DSP algoritmaları aracılığıyla yapılabilir.

**Fraud tespiti:** Gerçek zamanlı raporlar sayesinde anormal derecede yüksek CTR gibi sahte aktiviteleri tespit etmek daha kolaydır. Birçok RTB platformu ad-fraud tespiti ve önleme yazılımları içerir.

---

## Yayıncılar İçin

**Artan gelir:** RTB, yayıncının envanterini onlarca hatta yüzlerce reklam verene açar ve daha iyi eşleşme ile daha yüksek CPM’ler sağlar.

**Optimize edilmiş floor fiyatı:** Yayıncılar gerçek zamanlı analizle CPM floor fiyatlarını ayarlayarak gelirlerini artırabilir.

---

# RTB Ekosisteminde Komisyon ve Görünürlük (Transparency) Problemleri

Eskiden reklam veren ile yayıncı arasındaki süreç doğrudan yürütülürdü ve her iki taraf da medyanın hangi fiyata alınıp satıldığını bilirdi.

Bugün ise DSP’ler, SSP’ler, DMP’ler gibi platformlar sürece dahil olmuş ve programmatic medya satın alma hem remnant hem premium envanterde artmıştır.

Ancak bu platformlar süreci kolaylaştırırken aynı zamanda aracı konumuna gelmiş ve gerçek medya maliyetinin şeffaflığını azaltmıştır.

Bir reklam veren ajansı üzerinden medya satın aldığında, bütçesinin kaç farklı katmandan geçtiğini ve kullanıcıya ulaşmadan önce kaç komisyon ödendiğini çoğu zaman bilmez.

Bir reklamın yayıncıya ulaşmadan önce beş farklı taraf üzerinden geçmesi yaygın bir durumdur. Bu da beş farklı aracı ve beş farklı komisyon anlamına gelebilir.

## Aracı Komisyonları ve Ücretler

Her bir teknoloji platformunun (DSP, Ad Exchange, SSP) tam olarak ne kadar komisyon aldığını bilmek son derece zordur. Bu bilgi reklamverene aktarılsa bile, doğrulamak ve teyit etmek daha da zor olabilir.

Ancak PwC ve İngiliz Reklamverenler Birliği (ISBA) tarafından 2020 yılında yayımlanan **Programmatic Supply Chain Transparency Study** adlı rapor, ortalama olarak yayıncıların reklam harcamasının yalnızca %51’ini aldığını ortaya koymuştur. Harcamanın %35’i ajanslar ve AdTech şirketleri gibi aracı kurumlara gitmiştir. Ayrıca reklam harcamasının %15’lik kısmı (unknown delta) ise izah edilememiştir.

Rapordan öne çıkan bazı bulgular:

* Talep tarafı teknoloji ücretleri (ad serving, doğrulama araçları, veri vb.) reklamveren harcamasının ortalama %10’unu oluşturmuştur.
* SSP ücretleri, yayıncı gelirlerinin ortalama %14’üne (reklamveren harcamasının yaklaşık %8’i) denk gelmektedir.
* Yayıncıların aldığı pay %49 ile %67 arasında değişmektedir.

PwC tarafından 2014’te yapılan ve IAB tarafından sponsor olunan başka bir araştırma da, reklamveren bütçesinin yaklaşık %50’sinin ücret ve komisyonlara gittiğini göstermiştir.

Sektör yöneticileriyle yapılan görüşmelerde, programatik reklam teknolojisi ücretlerinin “ad tech tax” olarak adlandırıldığı ve çoğu zaman %50 veya daha fazlasına ulaştığı belirtilmiştir. Bu bağlamda “ad tech tax”, ATD’ler, DSP’ler, SSP’ler, ad server’lar ve reklam ağları gibi platformların sunduğu teknoloji ve katma değer hizmetler karşılığında hem alıcıdan hem satıcıdan aldığı ücretleri ifade eder. Çoğu durumda bu ücretler zincir boyunca katlanarak artar; bir tedarikçinin ücreti, bir sonraki tedarikçinin maliyetine eklenir.

Çalışma ayrıca bu oranın şirketten şirkete değiştiğini ve reklamverenin kaç farklı AdTech platformu kullandığına bağlı olarak daha düşük olabileceğini belirtmiştir.

Örneğin yalnızca tek bir DSP üzerinden bir ad exchange’ten medya satın alan bir reklamveren, hem ajans hem ATD hem de DSP kullanan bir reklamverene kıyasla daha az ücret ödeyecektir.

Günümüzde programatik sistemde reklamverenler genellikle yalnızca medya fiyatını (örneğin 1.000 gösterim için 10$ = CPM) bilir. Ancak bu tutarın yüzde kaçının teknoloji platformlarına gittiğini ve yayıncının gerçekte ne kadarını aldığını net biçimde göremezler.

---

Reklamverenler ayrıca ana platform ve aracıların yanı sıra üçüncü taraf veri sağlayıcılarına (davranışsal ve demografik doğrulama verileri gibi) bir veri yönetim platformu (DMP) üzerinden ödeme yapabilirler. Bunun yanında viewability, brand safety doğrulaması gibi ek hizmetler için de ücret ödenebilir.

Veri maliyeti genellikle reklamveren tarafından bilinse de, DSP kendi marjını ekleyebilir.

---

## Sektör Buradan Nereye Gidiyor?

Şeffaflık eksikliği acil çözüm gerektiren bir sorundur. İlk adım olarak reklamverenlerin teknoloji platformlarının iç işleyişi konusunda bilinçlendirilmesi ve sağladıkları değerin netleştirilmesi önemlidir.

Neyse ki birçok AdTech sağlayıcısı ücret ve komisyon yapıları konusunda daha şeffaf olmaya başlamıştır.

---

# Private Marketplace (PMP)

RTB yayıncıların remnant envanterini açık pazarda satmasına yardımcı olmuş olsa da, birçok premium yayıncı en değerli envanterlerinde gelir kaybı yaşadığını fark etmiştir.

Reklamverenler de premium envanteri kaçırdıkları ve reklamlarının görünmediği konusunda endişelenmeye başlamıştır.

Bu sorunları çözmek için **Private Marketplace (PMP)** modeli ortaya çıkmıştır.

Private marketplace, RTB modelinin yalnızca davet usulü çalışan bir varyasyonudur. Yayıncılar en premium envanterlerini seçilmiş alıcılara sunar.

PMP anlaşmalarına katılan reklamverenler, yayıncı envanteri açık RTB müzayedesine çıkmadan önce teklif verebilir.

---

Premium RTB açık artırmalarına kıyasla CPM daha yüksek olsa da, PMP üzerinden satın alan reklamverenler yayıncının premium envanterine herkesten önce erişim sağlar.

Yayıncılar PMP envanterini, bid request içinde bir **Deal ID** göndererek işaretler. Reklamverenin bu envanteri satın alabilmesi için eşleşen bir Deal ID’ye sahip olması gerekir.

---

# Yukarıdaki Medya Satın Alma Süreçlerinin Karşılaştırma Tablosu

Aşağıdaki tablo, üç farklı medya satın alma yönteminin karşılaştırmasını göstermektedir:

### Fiyatlandırma

* RTB (Public Auctions): Açık artırma
* PMP (Deal ID): Açık artırma ve/veya anlaşma şartları
* Programmatic Direct: Önceden belirlenmiş
* Non-Programmatic (Direct Campaigns): Önceden belirlenmiş

### Reklamveren-Yayıncı Doğrudan İlişki

* RTB: Hayır
* PMP: Evet
* Programmatic Direct: Evet / sınırlı
* Direct Campaigns: Evet

### Envanter Hacmi

* RTB: Garantili değil
* PMP: Garantili değil
* Programmatic Direct: Garantili
* Direct Campaigns: Garantili

### Envanter Türü

* RTB: Yayıncının açık artırmaya sunduğu tüm envanter
* PMP: Premium envanter
* Programmatic Direct: Tüm envanter (premium dahil)
* Direct Campaigns: Tüm envanter (premium dahil), ancak sınırlı hedefleme

---

### Avantajlar

**RTB (Public Auctions):**

* Gösterim bazlı satın alma
* Tek panel üzerinden yönetim
* Kolay test ve optimizasyon
* Veri içgörüleri
* Remnant envanteri satabilme

**PMP:**

* Satın alınan envanter ve fiyat konusunda şeffaflık
* Aracı sayısını azaltma
* Endüstri standardı haline gelme
* Doğrudan satış ekibine olan ihtiyacı azaltma

**Programmatic Direct:**

* Şeffaflık
* Otomasyon
* Daha iyi içgörü ve kontrol
* Garantili envanter hacmi

**Direct Campaigns:**

* Şeffaflık
* Doğrudan ilişki
* İçgörü ve kontrol
* Garantili envanter hacmi

---

### Dezavantajlar

**RTB:**

* Premium envantere sınırlı erişim

**PMP:**

* Daha pahalı envanter

**Programmatic Direct:**

* Önceden belirlenen fiyat nedeniyle fazla ödeme riski

**Direct Campaigns:**

* Ölçeklenebilir değil
* Yavaş süreç

---

# Publisher’ın Waterfall Süreci

Waterfall (daisy chain veya waterfall tags olarak da bilinir), yayıncının remnant envanterini satmak için kullandığı bir yöntemdir. Premium alanlar doğrudan satış ekibi tarafından satılamadığında devreye girer.

Waterfall adını, talep kaynaklarının sırayla — birer birer — tetiklenmesinden alır.

Avantajı: Envanterin satılma ihtimali artar.
Dezavantajı: Zincirde aşağı indikçe ortalama CPM düşer.

---

## Yayıncının İkilemi: Yüksek CPM mi, Yüksek Fill Rate mi?

Yayıncı şu soruyla karşı karşıyadır:

* Yüksek CPM’den satıp bazı gösterimleri boş mu bırakmalı?
* Yoksa tüm envanteri doldurup daha düşük CPM mi kabul etmeli?

---

Görselde görüldüğü gibi:

1. Önce doğrudan satış (yüksek CPM, düşük fill rate)
2. Sonra RTB açık artırması (orta CPM, orta fill rate)
3. Son olarak remnant ad network (düşük CPM, yüksek fill rate)

Örnek fill dağılımı:

* Direct Campaigns: %30
* RTB Auction: %30
* Remnant Network: %40

---

## Waterfall Nasıl Uygulanır?

AdOps ekibi, bir gösterim dolmadığında tetiklenecek bir takip etiketi (tracking tag) kurar.

Bu yapı genellikle yayıncının ad server’ında ve çalıştığı her reklam ağında “Fallback Ads”, “Passbacks”, “Redirects”, “Default Ads” gibi alanlarda yapılandırılır.

Her ağ için ayrı passback tanımlanır. Örneğin premium ad network dolmazsa, remnant ad network’e paslanır.

---

## Waterfall Nasıl Çalışır?

Doğrudan satış gerçekleşmezse, ad server ilk reklam ağının etiketini çalıştırır.

### Senaryo 1

Advertiser #1 ile yapılan doğrudan anlaşma gösterimi karşılayabiliyorsa, reklam doğrudan kullanıcının tarayıcısına gönderilir.

### Senaryo 2

Doğrudan anlaşma karşılayamazsa, RTB açık artırması (Ad Exchange #1 ve #2) denenir.
Eğer burada da karşılanmazsa, remnant ad network #1 devreye girer ve gösterimi sağlar.

Reklam son olarak kullanıcının tarayıcısında görüntülenir.


---

## Private Marketplace (PMP)

RTB, yayıncıların remnant (artan) envanteri açık pazarda satmasına yardımcı oldu. Ancak premium yayıncılar en değerli envanterlerini açık artırmada satarken gelir kaybı yaşadıklarını fark etti.

Ayrıca reklam verenler de premium envantere erişemediklerinden veya reklamlarının görünür olmadığından endişe etmeye başladılar.

Bu sorunları çözmek için PMP (Private Marketplace) modeli doğdu.

### PMP Nedir?

PMP, RTB modelinin davet usulü çalışan bir versiyonudur. Yayıncılar premium envanterlerini seçilmiş alıcılara sunar.

* Reklam verenler, açık RTB açık artırmasından önce teklif verebilir.
* PMP envanteri bid request içinde bir **Deal ID** ile işaretlenir.
* Reklam verenin bu envanteri satın alabilmesi için eşleşen bir Deal ID’ye sahip olması gerekir.

CPM genellikle açık RTB’den daha yüksektir, ancak premium envantere ilk erişim sağlanır.

---

## Medya Satın Alma Yöntemlerinin Karşılaştırması

### RTB (Public Auction)

* Fiyat: Açık artırma
* Doğrudan ilişki: Hayır
* Hacim: Garantili değil
* Avantaj: Impression bazlı satın alma, kolay optimizasyon
* Dezavantaj: Premium envantere sınırlı erişim

### PMP (Deal ID)

* Fiyat: Açık artırma ve/veya anlaşmalı
* Doğrudan ilişki: Var
* Hacim: Garantili değil
* Avantaj: Şeffaflık, premium envantere erişim
* Dezavantaj: Daha pahalı

### Programmatic Direct

* Fiyat: Önceden belirlenmiş
* Hacim: Garantili
* Avantaj: Otomasyon + kontrol + garanti
* Dezavantaj: Aşırı ödeme riski

### Non-Programmatic (Direct Campaign)

* Fiyat: Önceden belirlenmiş
* Hacim: Garantili
* Avantaj: Doğrudan ilişki ve kontrol
* Dezavantaj: Ölçeklenmesi zor, yavaş süreç

---

## Publisher’ın Waterfall Modeli

Waterfall (daisy chain), yayıncının satılamayan envanteri katmanlı şekilde farklı talep kaynaklarına sırayla sunmasıdır.

Akış:

1. Önce direct sales (yüksek CPM, düşük fill rate)
2. Sonra RTB
3. Son olarak remnant ad network

Avantaj:

* Satılamayan envanteri elden çıkarır

Dezavantaj:

* Katman ilerledikçe CPM düşer
* Gerçek zamanlı piyasa fiyatını yansıtmaz
* Gecikme (latency) yaratır

### Publisher’ın İkilemi

* Yüksek CPM mi? (düşük fill rate riski)
* Yüksek fill rate mi? (daha düşük CPM)

---

## Header Bidding

Header bidding (pre-bidding, advance bidding), yayıncının ad server çağrılmadan önce birden fazla talep kaynağından aynı anda teklif toplamasını sağlar.

Bu işlem, web sayfasının `<head>` bölümündeki JavaScript kodu ile yapılır.

### Nasıl Çalışır?

1. Kullanıcı sayfayı açar.
2. Header JS kodu SSP’lere ve ad exchange’lere bid request gönderir.
3. SSP’ler DSP’lere iletir.
4. En yüksek teklif belirlenir.
5. Bu teklif ad server’daki direct kampanyalarla rekabete girer.
6. En yüksek değerli kampanya gösterilir.

Latency önemli bir sorundur:

* Desktop: 400–800 ms
* Mobile: 800–1200 ms

Prebid.js, header bidding’i kolaylaştıran açık kaynak bir framework’tür.

---

## Client-Side vs Server-Side Header Bidding

### Client-Side (CSHB)

Avantaj:

* Daha iyi cookie matching
* Daha fazla şeffaflık
* Wrapper kontrolü yüksek

Dezavantaj:

* Sayfa yükleme süresi uzar
* Tarayıcı limitleri (istek sayısı)
* Browser uyumluluk sorunları

### Server-Side (SSHB)

Avantaj:

* Daha düşük latency
* Daha fazla talep kaynağına erişim

Dezavantaj:

* Daha az şeffaflık
* Cookie matching zor

---

## Auction Dynamics

### Second-Price Auction (2PA)

* En yüksek teklif kazanır.
* Ancak ikinci en yüksek teklif + $0.01 öder.
* Clearing price = ödenen fiyat

### First-Price Auction (1PA)

* En yüksek teklif kazanır.
* Verdiği fiyatı aynen öder.

2017/2018 sonrası birçok SSP ve exchange first-price modeline geçti.

---

## Bid Shading

First-price modelinde reklam verenler tam tekliflerini ödemek zorunda kaldığı için bid shading geliştirildi.

Bid shading:

* Tarihsel verileri analiz eder
* Reklam verene “gerçek” kazanma fiyatına daha yakın bir teklif önerir
* Ancak şeffaf değildir

Sonuç:

* Reklam veren tasarruf eder
* Yayıncı daha az gelir elde edebilir

---

## Floor Prices

Floor price = Yayıncının kabul edeceği minimum CPM.

### Hard Floor

* Minimum kabul edilen fiyat
* Altındaki teklifler otomatik reddedilir

### Soft Floor

* Hard floor’dan biraz daha esnek
* Hard ile soft arasındaki teklifler first-price açık artırmaya girer
* Soft üzerindeki teklifler second-price mantığına göre çalışabilir

---

## Bölüm Özeti

Reklam verenler medya satın alabilir:

* Direct deals
* Programmatic direct
* RTB
* PMP

Waterfall:

* Sırayla talep kaynağı çağırır

Header bidding:

* Aynı anda birden fazla talep kaynağından teklif toplar
* Daha yüksek CPM potansiyeli

RTB’de iki açık artırma türü vardır:

* Second-price
* First-price

Floor price:

* Yayıncının minimum kabul ettiği CPM

---

[⬅️ Bölüm 08: İzlenim, Tıklama ve Dönüşüm Takibi](/The-AdTech-Book/bolumler/08-izlenim-tiklama-donusum-takibi) | [🏠 Ana Sayfa](/The-AdTech-Book/) | [➡️ Bölüm 10: Kullanıcı Kimliklendirme](/The-AdTech-Book/bolumler/10-kullanici-kimliklendirme)
